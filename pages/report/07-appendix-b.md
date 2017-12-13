---
layout: base

appendix: true

title: "Appendix B: Principles of Cloud-Oriented Security Protections"
permalink: /report/appendices/cloud-security-protections/

subnav:
  - text: Government-Wide Visibility and Classified Indicators
    href: "#government-wide-visibility-and-classified-indicators"
  - text: Proportionate Security
    href: "#proportionate-security"
---

As noted in this Report, the Federal Government has traditionally
focused its Government-wide information security efforts on protecting
network boundaries; however, instead of emphasizing physically
consolidated security at the perimeter, such as in the current Trusted
Internet Connections (TIC) model, a data-centric approach emphasizes
placing protections closer to the services and information systems in
which sensitive data is stored and accessed. This gives agencies
flexibility in the approaches they choose. For modern services hosted in
the cloud, agencies can place security protections directly in front of
each service and allow direct connections from the public internet. For
services hosted in legacy data centers, such capabilities may not be
available, in which case the agency can still rely on perimeter security
as they pursue options to modernize their system architecture.

There is no one right way for an agency to operationalize security
protections in Cloud Service Providers (CSPs), and some features and
approaches may need to be optimized for the particular cloud service
provider in use. Agencies should ensure any CSP they choose meets the
security capabilities outlined by FedRAMP. The approach in this appendix
applies to cases wherein an agency is directly operationalizing software
in a cloud-hosting environment. This does not apply to Software as a
Service (SaaS) applications operated in full by vendors, as their
security approaches will be vendor-specific.

Agencies could take the following approach to designing security
protections in a cloud-based application stack:

-   An agency could separate their security stack from their application
    stack within their cloud provider. In whatever way this separation
    occurs, agencies should maintain the principle that a compromise of
    the application being protected should not automatically lead to
    compromise of the security stack being used to protect that
    application and vice versa;

-   Incoming traffic could be routed through the cloud provider’s
    commodity virtualized load balancers, used to obtain a carbon-copy
    of the data, to a set of virtual security appliances. These virtual
    security appliances would process incoming traffic “on path,”
    meaning that incoming requests are blocked on the ability of the
    security appliances to process them. Since putting any devices “on
    path” of existing traffic has significant reliability, security, and
    performance implications, the choice of security functions for this
    purpose must be warranted by the sensitivity of the application.
    Lower sensitivity applications likely warrant few, if any, “on path”
    request processing services;

-   These virtual appliances could themselves implement most of the
    security functions described by existing TIC policy, including
    intrusion detection, filtering, and logging. Importantly, these
    virtual appliances must be horizontally scalable so that any number
    of instances can handle as much traffic as the service might
    receive; and

-   After the traffic is processed by the virtual security appliances,
    it exits the segregated security zone. It is then sent to the
    application’s load balancer to be processed normally by the
    application.

An example diagram showing data-centric security in a cloud provider is
shown in **Figure 1**.

![ATC Networks - Cloud Moderate]({{ site.baseurl }}/assets/img/image1.png)

**Figure 1**

This data-centric application security layer could be implemented
directly by an application team, or it could be run by an agency as an
internal shared service for all applications hosted within a particular
cloud provider. It could also be possible for a sufficiently responsive
agency team to provide this layer as a shared service to multiple
agencies who utilize the same cloud provider.

To achieve centralized visibility for agency security teams, this
data-centric application security layer should send logs and alerts in
real time to centralized aggregation systems that process security
information and events. These centralized aggregation systems could be
co-located in the same cloud provider as the applications from which
they are aggregating information. They could also aggregate logs and
network flow information received from the cloud service provider
itself. One operational approach for doing this is described in the
Security Operations Center as a Service section of this report.

### Government-Wide Visibility and Classified Indicators

Some Government-specific security functions, such as the intrusion
detection and prevention capabilities of 6 U.S.C. § 151, currently
offered as EINSTEIN, would not be automatically fulfilled by commodity
solutions. Some needs, for example, can only be addressed with
classified indicators. This produces a challenge for agencies, as these
classified indicators can only be stored in data centers meeting very
specific security requirements. For most systems, however, these
Government-specific functions, such as EINSTEIN 1 and EINSTEIN 2, do not
leverage classified indicators or need to be physically “on path” for
network traffic and incoming requests. Instead, the virtual appliances
in the data-centric security layer could create a copy of relevant
traffic or logs and send a stream to a nearby location (perhaps operated
by DHS as part of the intrusion detection and prevention capabilities of
6 U.S.C. § 151) where these Government-specific security functions can
be performed in the background. The original copy of the traffic
continues to flow to the cloud provider unless, depending on the
capability at issue, an alert is generated from the intrusion prevention
system. This achieves visibility and detection of classified threats
without sacrificing the major benefits of adopting modern cloud
architectures. A diagram of how this may look is represented in Figure
2.

![ATC Networks - Cloud High]({{ site.baseurl }}/assets/img/image2.png)

**Figure 2**

DHS should also consider evolving NCPS’s intrusion prevention
capabilities program to include the ability to receive and act on
additional application layer traffic. In its current form, EINSTEIN 3A
does not process most web traffic, because it only examines email and
domain name server.

The data-centric approach outlined above also allows a more nuanced
approach to protection, allowing security teams to focus their efforts
on the systems that need it most. For low-impact systems that only store
public data, it is likely unnecessary to split off traffic for
classified analysis. For high-sensitivity systems with very valuable
private data, it may be useful to require more security measures, such
as waiting for classified analysis to be complete before passing traffic
along to the application.

### Proportionate Security

While the protections described in this appendix can be useful to many
applications, the Federal Government should focus its limited security
resources on its highest-value assets. All security protections come
with a cost: any security services “on path” can impact reliability and
performance, add complexity to system operations, and could have
vulnerabilities that would be used against the applications they are
intended to defend. Even “off path” security services that do not
process data in real time, such as classified indicators and services
that provide Government-wide visibility, add complexity as well as
oversight and compliance costs to system operation.

For the Government’s security protections to be most effective, they
should be deployed on systems whose data is worth such a sustained and
sophisticated defense, such as HVAs. Systems that contain information
that would have a low impact if compromised should instead be optimized
for agility and availability, thus freeing security resources for more
sensitive systems.

An isolated system with no sensitive information therefore might merit a
more streamlined architecture. **Figure 3** shows how a low-impact
system may serve requests directly:

![ATC Networks - Cloud Low]({{ site.baseurl }}/assets/img/image3.png)

**Figure 3**

---
layout: base

appendix: true

title: "Appendix A: Data-Level Protections and Modernization of Federal IT"
permalink: /report/appendices/data-level-protections/

subnav:
  - text: Foundational Capabilities
    href: "#foundational-capabilities"
  - text: Risk-Based Capabilities
    href: "#risk-based-capabilities"
  - text: Leveraging Modern Deployment Solutions
    href: "#leveraging-modern-deployment-solutions"
---

The provision of appropriate protections begins with ensuring that
foundational information security capabilities are in place. These
capabilities should be implemented for all Federal IT systems; and any
IT Modernization efforts should leverage the below principles as a core
component of their upgrades. As agencies look to prioritize their
modernization efforts, they are encouraged to focus first on deployment
of these principles for high value assets.

High value assets (HVAs) are assets, Federal information systems, and
data, for which the unauthorized access, use, disclosure, disruption,
modification, or destruction could cause a significant impact to the
United States' national security interests, foreign relations, economy,
or to the public confidence, civil liberties, or public health and
safety of the American people. This definition is codified in OMB
Memorandum M-17-09, *Management of Federal High Value Assets*. As such,
the protection of HVAs should be among the highest priority
cybersecurity activities for Federal agencies.

## Foundational Capabilities

**Multi-Factor Authentication**. The goal of multi-factor authentication
is to make remote attacks unattractive, typically by requiring the
production of a credential that is specifically connected to a user in a
physical manner in order to grant the user access to a system. Recent
Federal efforts have focused on multi-factor authentication for
privileged users, or those with elevated access privileges, but thus far
has largely centered on network access rather than system and
application-level access.

**Least Privilege.** The principle of least privilege states that users
should only be granted access to the specific systems and information
they need in order to execute their official duties. In practice, this
is achieved by limiting administrative privileges. Mature privilege
management programs may also be able to leverage policy- or
attribute-based access controls, wherein sophisticated rules-based
policies (which can be dynamically updated and enforced) can support a
system that makes privilege escalation more expensive and difficult for
an attacker.

**Timely Patching.** One of the most significant threats to IT systems
remains unpatched software vulnerabilities. For that reason, OMB, under
OMB Memorandum M-15-01, *Fiscal Year 2014-2015 Guidance on Improving
Federal Information Security and Privacy Management Practices*, required
agencies to sign memorandums of agreement or understanding to allow the
DHS to scan their external-facing systems for unpatched vulnerabilities.
Under Binding Operational Directive 15-01, DHS then required agencies to
patch critical vulnerabilities within 30 days of being notified of such
vulnerabilities. Agencies should prioritize the creation of routine, and
ideally automated, patching processes for their HVAs that ensure that
critical vulnerabilities are resolved much more rapidly than the
required 30 days.

## Risk-Based Capabilities

In addition to the above capabilities that all agencies are expected to
adopt, there are numerous information security capabilities which
agencies are advised to deploy pursuant to assessments of the risk posed
to a certain system or set of information. In the context of HVAs, the
systems and information are, by definition, highly sensitive and/or
impactful. As such, agencies should seriously consider the value of
these capabilities in terms of better defending their “crown jewels.”

**Encrypting Data at Rest**. Data at rest is data in a database or other
storage areas, as opposed to in transit between systems. Encrypting that
data makes it inaccessible should an attacker manage to make a physical
copy of it. Effective encryption of data at rest requires sufficiently
strong encryption keys with sufficient randomness in key
generation.[^23]

**Encrypting Data in Transit.** Encrypting data as it transits from one
device or system component to another protects data from modification or
interception from an attacker with a network vantage point. Network
routes that transit data between information system components, or
between information systems and their users, should generally be treated
as untrusted, even within agency-operated networks. In general, though
particularly for HVAs, systems should rely only on protocols that can
safely “fail closed,” or default to denying network access, under attack
scenarios. Examples include Secure Shell (SSH) or Hyper Text Transfer
Protocol Secure (HTTPS).

**Secure Application Development.** Security must be a regular, ongoing
part of the software development process, not simply a paperwork
exercise completed prior to production deployment. Security teams should
be integrated throughout the software development process, starting from
its earliest stages. Such an approach can alleviate the characterization
of security personnel as impediments, but, rather, as essential members
of the larger development team.

**Security Testing.** Penetration testing, phishing tests, and database
assessments should be incorporated into the testing regimen for agency
HVAs. Agencies should establish a vulnerability disclosure policy for
public-facing services so that security researchers and members of the
public can report vulnerabilities they discover. Teams wishing to go
further should consider running bug bounty programs, such as those run
by the Department of Defense or GSA.[^24]

**Threat Modeling.** Engineering teams should use threat modeling to
understand and drive improvements in the security of the HVA. Threat
models help identify the most vulnerable parts of an application. This
focuses resources in the areas where risk reduction is needed the most,
and forms a cornerstone of implementing a risk-based practice of
security like the NIST Cybersecurity Framework.

**Application Whitelisting.** The purpose of application whitelisting is
to allow only approved applications and application components
(libraries, configuration files, etc.) to run on a host according to a
well-defined baseline, while preventing all other applications from
running by default. When implemented, application whitelisting is an
effective security technique that helps stop the execution of malicious
malware and other unauthorized software.[^25]

**Mobile Device Management.** Mobile devices often need additional
protection because their nature generally places them at higher exposure
to threats than other devices typically used within Government
facilities, such as desktops and laptops. When planning mobile device
security policies and controls, agencies should assume that mobile
devices will be acquired by malicious parties who will attempt to
recover sensitive data either directly from the devices themselves or
indirectly by using the devices to access the organization’s remote
resources. Therefore, a layered mitigation strategy should be used that
includes user authentication to the device, protection of data either
through encryption or by not storing data on the device, and user
training and awareness to reduce the frequency of insecure physical
security practices. Additionally, agencies should plan their mobile
device security on the assumption that unknown third-party mobile device
applications downloadable by users should not be trusted. Risk from
these applications can be reduced in several ways, such as prohibiting
all installation of third-party applications, implementing whitelisting
to allow installation of approved applications only, verifying that
applications only receive the necessary permissions on the mobile
device, or implementing a secure sandbox/secure container that isolates
the organization’s data and applications from all other data and
applications on the mobile device.[^26]

## Leveraging Modern Deployment Solutions

In addition to the solutions described above, agencies should consider
how best to take advantage of protections afforded by modern deployment
patterns (e.g. “DevOps”) and cloud-based architectures in the defense of
their HVAs.

**Automated Deployments.** System deployments should be automated to the
greatest extent possible, removing the potential for errors caused by
breakdowns in internal processes. To support this, configuration and
environmental details that support system deployment should be versioned
and managed similarly to the software that comprises the system itself.
This practice is necessary to achieve long-term consistency among
critical system components, maintain adequate patching, and update
velocity.

**Immutable Deployments.** By building on automation, production
environments should be designed so that components are not modified in
place subsequent to being deployed. Modification should be technically
constrained wherever possible; for example, deployed servers should not
allow remote logins. By taking advantage of virtualized infrastructure,
new deployments can create brand new instances of deployed system
software and supporting components, rather than updating the existing
environment in place. This approach allows system owners to design their
security architecture and monitoring to treat any in-place modification
as a potential attack, and to use more comprehensive technical
constraints on modification that remove opportunities for attackers to
persist in a deployed environment.


[^23]: See NIST SP 800-133, *Recommendation for Cryptographic Key
    Generation*.

[^24]: United States Digital Service, *July 2017 Report to Congress,*
    “Hack the Pentagon.” July 2017.

[^25]: See NIST SP 800-167, *Guide to Application Whitelisting*.

[^26]: See NIST SP 800-124, *Guidelines for Managing the Security of
    Mobile Devices in the Enterprise*.

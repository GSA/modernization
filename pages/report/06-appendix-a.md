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

**Appendix A: Data-Level Protections and Modernization of Federal IT**

This report envisions a modern Federal IT enterprise that relies on
**logical protections** and **automation**, and is focused on
**empirical evidence** and **security outcomes**.

Below are some capabilities and approaches Federal agencies are expected
to use to improve the agility of their enterprise and the security of
their IT systems.

**Logical Protections**

Agencies should rely principally on logical protections, such as
encryption and granular permissions, to protect data. When designing
mitigations, networks should be considered untrusted, and system
components should be assumed to be potentially compromised.

**Encrypting Data in Transit.** Encrypting data as it transits from one
device or system component to another protects data from modification or
interception from an attacker with a network vantage point. Network
routes that transit data between information system components, or
between information systems and their users, should generally be treated
as untrusted, even within agency-operated networks. In general, systems
should rely only on protocols that can safely “fail closed” (default to
connection failure), under attack scenarios. Examples include Secure
Shell (SSH) or Hyper Text Transfer Protocol Secure (HTTPS).

**Encrypting Data at Rest**. Encrypting data using tools that implement
NIST standards and guidelines, when stored, whether in a database or
some other persistent storage, is designed to make that data useless to
an attacker, should an attacker gain access to that storage system and
copy the data. Effective designs for encryption of data at rest should
consider how to limit an attacker’s options both during and after the
attacker maintains control of the information system, such as by
requiring the presence of a hardware security module to perform (and
rate limit) decryption actions. Like encryption in other areas,
encryption at rest generally requires sufficiently strong encryption
keys with sufficient randomness in key generation.[^25]

**Multi-Factor Authentication**. The goal of multi-factor authentication
is to make remote attacks unattractive, typically by requiring the
production of a credential that is connected to a specific user in a
physical manner in order to grant the user access to a system. Recent
Federal efforts have focused on multi-factor authentication for
privileged users, or those with elevated access privileges, but thus far
has largely centered on network access rather than system and
application-level access.

**Least Privilege.** The principle of least privilege is intended to
prevent the compromise of individual users and information system
components to lead to the total compromise of an information system.
This principle can be applied both to users and to components of
information systems. Privileged users should only be granted privileged
access to the system components they need to perform their job, which
can require richer permissions models than simply designating “admins.”
Similarly, system components, such as individual servers and endpoints,
should themselves be limited in their ability to connect or exchange
information to only the components they need in order to perform their
function. Mature privilege management programs may also be able to
leverage policy- or attribute-based access controls, wherein
sophisticated rules-based policies (which can be dynamically updated and
enforced) can support a system that makes privilege escalation more
expensive and difficult for an attacker.

**Application Whitelisting.** The purpose of application whitelisting is
to allow only approved applications and application components
(libraries, configuration files, etc.) to run on a host according to a
well-defined baseline, while preventing all other applications from
running by default. When implemented, application whitelisting is an
effective security technique that helps stop the execution of malicious
malware and other unauthorized software.[^26]

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
applications on the mobile device.[^27]

**Automation and outcome-oriented security**

Agencies should gain confidence in their security posture through
empirical evidence and measurable improvement over time. To do this,
agencies must take an iterative approach to security, and have the
agility to change their practices to adapt to the threats they and other
agencies observe. Automation is a critical tool to maintain agility in
system design and to make the best use of finite human resources.

**External Security Testing.** Agencies must take a layered approach to
penetration testing and system assessments that incorporates as much
ongoing external review as possible. At a bare minimum, agencies should
establish vulnerability disclosure policies for at least their
public-facing services, so that security researchers and other members
of the public can report vulnerabilities they discover. Agencies should
also identify systems that are appropriate to place under public bug
bounty programs, such as those run by the [Department of Defense][HACK-THE-PENTAGON] or
GSA. Private bounty programs, where researchers may be vetted,
monitored, and given credentialed access, can be an additional useful
tool for building confidence in a system, and can be run in parallel to,
or in advance of, a public program. Bounty programs require
vulnerabilities to be fixable in a reasonably rapid time frame, and can
be implemented for specific systems, for short periods of time or on an
ongoing basis. Agencies have many options for incorporating external
security testing of their systems, and should bring as many as feasible
to bear on their most important systems.

**Avoiding security through obscurity.** Internet-wide scanning and
discovery is commonplace and effective. Agencies must assume that their
publicly accessible systems are trivially publicly discoverable to
adversaries, and prioritize the sharing of information about their
systems with defenders inside and outside the Federal enterprise.
Similarly, agencies should support the use and release of open-source
software where it improves agency agility and resilience.

**Threat Modeling.** Agencies should use threat modeling to understand
and drive improvements in the security of their systems. Threat models
define what threats a system is designed to mitigate, and what threats
the system is not designed to mitigate. This focuses resources in the
areas where risk reduction is needed the most, and forms a cornerstone
of implementing a risk-based practice of security, as described in the
NIST Cybersecurity Framework.

**Continuous integration and code review.** Agencies should follow a
“DevSecOps” model, using automated unit and integration tests to aid the
code review process and maintain ongoing confidence in the system.
Rather than onerous change control boards, agencies should employ
automatic testing and widely visible code review to measure and
accelerate the time it takes for code changes to be deployed to
production.

**Automated Deployments.** System deployments should be automated to the
greatest extent possible, removing the potential for errors caused by
breakdowns in internal processes. To support this, configuration and
environmental details that support system deployment should be versioned
and managed similarly to the software that comprises the system itself.
This practice is necessary to achieve long-term consistency among
critical system components, maintain adequate patching, and update
velocity.

**Immutable Deployments.** Production deployments should be automated
and designed so that components are not modified in place between
deployments. Modification should be technically constrained wherever
possible; for example, deployed servers should not allow remote logins.
By taking advantage of virtualized infrastructure, new deployments can
create brand new instances of deployed system software and supporting
components, rather than updating the existing environment in place. This
approach allows system owners to design their security architecture and
monitoring to treat any in-place modification as a potential attack, and
to use more comprehensive technical constraints on modification that
remove opportunities for attackers to persist in a deployed environment.

**Timely Patching.** Unpatched software vulnerabilities remains one of
the most significant threats to Federal IT systems. DHS currently scans
external-facing agency systems for known unpatched vulnerabilities, and
agencies are currently required to patch critical vulnerabilities within
30 days; however, depending on the severity and ease of exploitation,
unpatched vulnerabilities in public-facing systems can lead to
compromise in weeks, days, or even hours of public disclosure. Agencies
should consider patching agility and responsiveness to be a critical
security metric and modernization goal. Automated scanning, consistent
software baselines, and easy and immutable deployments are all critical
to bringing expected patch times down to acceptable levels.


[^25]: See NIST SP 800-133, [*Recommendation for Cryptographic Key Generation*][SP-800-133].

[^26]: See NIST SP 800-167, [*Guide to Application Whitelisting*][SP-800-167].

[^27]: See NIST SP 800-124, [*Guidelines for Managing the Security of Mobile Devices in the Enterprise*][SP-800-124].

[HACK-THE-PENTAGON]: https://www.usds.gov/report-to-congress/2017/07/hack-the-pentagon/

[SP-800-133]: http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-133.pdf

[SP-800-167]: http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-167.pdf

[SP-800-124]: http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-124r1.pdf

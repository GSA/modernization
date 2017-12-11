---
layout: base

appendix: true

title: "Appendix C: Challenges to Implementing Federal-Wide Perimeter-Based
Security"
permalink: /report/appendices/challenges-to-perimeter-security/

subnav:
  - text: Cloud Security and Situational Awareness
    href: "#cloud-security-and-situational-awareness"
  - text: Encrypted Network Traffic
    href: "#encrypted-network-traffic"
  - text: Overreliance on Static Signatures
    href: "#overreliance-on-static-signatures"
  - text: Use and Value of Classified Indicators
    href: "#use-and-value-of-classified-indicators"
---

Today, the Federal Government applies a defense-in-depth strategy to
protect its systems that includes agency and DHS-provided protections at
various levels. But, at the same time, Government-wide programs overly
rely on a perimeter-based security model to protect the Government’s
networks and information systems. This model, formalized in OMB
Memorandum M-08-05, *Implementation of Trusted Internet Connections
(TIC)*, focuses on standardizing security at the network boundary
through consolidation of external access points. Under this model, the
Government has required agencies to reduce external connections, to a
target of 50, and route their traffic through this limited number of
secure gateways. These gateways apply common intrusion detection and
prevention capabilities under DHS’s National Cybersecurity Protection
System (NCPS). NCPS consists of three sensor capabilities (collectively
referred to as EINSTEIN), as well as a set of analytic tools used by
cyber analysts to find, identify and categorize cyber threat activity.
[^29]

The NCPS sensor suite is deployed in three iterations: EINSTEIN 1 (E1),
which captures and analyzes network flow information; EINSTEIN 2 (E2),
which incorporates intrusion detection technology that scans the content
of network communications to identify and alert to known indications of
malicious activity; and EINSTEIN 3-Accelerated (E3A), which detects and
blocks malicious activity through DNS sinkholing and email filtering.

This perimeter-based architecture has created several challenges,
specifically regarding adoption of commercial cloud and mobile
technologies. Additionally, signature-based detection and protections
systems provide value, but are not enough to combat the full spectrum of
advanced persistent threats that rapidly change attack vectors, tactics,
techniques, and procedures.[^30] [^31] All of these challenges are
acknowledged and understood by DHS, and efforts are underway to address
these specific issues.

As an overarching effort, DHS has undertaken a cybersecurity
architectural review of Federal, Civilian, and Executive Branch
infrastructure to capture empirical data, which will be used to
determine the efficacy of individual and collective groupings of
capabilities against specific threats to that architecture. This data
will then be used to guide the evolution of DHS cyber program
capabilities, to include NCPS and the CDM program.

In addition to the holistic architecture review, DHS has continuously
assessed its programs to determine if the program investments they are
making are appropriate. As part of this continuous assessment, DHS has
identified several challenges that must be addressed to improve and
deliver value to its Federal Executive Branch stakeholder community.
These challenges include:

1.  Cloud Security and Situational Awareness

2.  Encrypted Network Traffic

3.  Overreliance on Static Signatures

4.  Use and Value of Classified Indicators

## Cloud Security and Situational Awareness

Federal agencies have started to embrace the use of cloud services to
include Infrastructure as a Service (IaaS), Platform as a Service
(PaaS), and Software as a Service (SaaS), which has the promise to move
much of the Federal Executive Branch’s computing and data to
commercially available cloud environments, outside of traditional
network boundaries. In doing so, the emphasis on protecting and
monitoring perimeter connections of trusted networks at a limited number
of physical TIC access points has introduced performance degradation.
This has discouraged agencies from fully adopting cloud services, and
undermines many of their key benefits such as reducing costs,
flexibility, time-to-deploy, and availability and reliability. An
example of a current network routing challenge for agencies that have
adopted cloud services is an agency that has implemented a public-facing
web service must route user traffic through a limited number of physical
TIC access points for inspection, which in turn introduces latency. The
diagram below illustrates how this approach is currently implemented, in
a phenomenon known as “the network trombone,” which constrains the
benefits of cloud services by forcing users to route traffic through a
physical network location rather than being able to connect directly to
the cloud service.

![ATC Networks - TIC Trombone]({{ site.baseurl}}/assets/img/image4.png)

To address this situation, DHS has engaged with three large cloud
service providers to determine how DHS may gain the insight and
situational awareness from within the cloud that is similar to the
information that is gained from its E1 and E2 sensors that are deployed
at the TICs. The focus of this engagement thus far has been the
collection of internal cloud log data, specific to the agency
application and data that could be fed back to DHS to provide a similar
level of situational awareness to DHS cyber analysts.

## Encrypted Network Traffic

As the use of cloud and web services continues to expand, so has the use
of network transport security in the form of encrypted tunnels between
end users and their applications and data. The use of transport
encryption is critical for secure communications, but limits what is
visible to a perimeter-based monitoring system such as E1 or E2. The
amount of network traffic that is encrypted that passes through E1 and
E2 sensors has increased over time, with 47 percent of all traffic being
encrypted as of December 2016. This continued growth of encrypted
network traffic has limited the functionality and usefulness of E1 and
E2 sensors and has made it difficult for DHS to inspect this traffic for
cyber threats. For DHS E2 sensors, this means that DHS signatures are
unable to inspect the content of network communications and alert on
malicious content.

Continued growth in encryption is both beneficial and inevitable, and
DHS has commissioned research to determine potential architectural,
technical, and policy mitigation strategies that could provide DHS with
both the protection and situational awareness for encrypted traffic.
Some of the mitigation strategies currently under evaluation include:

1.  **Sensor Placement**. This involves relocating the E1 and E2 sensors
    where the traffic is decrypted (e.g., endpoints of an encrypted
    tunnel). In the cases of virtual private network tunnels, one could
    place sensors outside of encrypted areas. For cloud environments,
    investigation is needed to determine how these sensors could be
    virtualized and placed in physical or virtual locations where
    Government applications and data exist.

2.  **Man-In-The-Middle (MITM) Interception**. This involves deploying
    MITM technologies that decrypt traffic, inspect it, and re-encrypt
    it, by placing a proxy along the network path. This proxy falsely
    pretends to each side to be the other side of the communications.
    Network proxies that intercept Transport Layer Security (TLS)
    traffic via MITM are commercially available. Usually this requires
    local clients to have blanket trust of this proxy.

3.  **Key Escrow**. This involves gaining access to decryption keys
    (e.g., as part of a broader certificate management system and
    architecture). A key escrow approach requires clients to register
    keys with a trusted third party.

## Overreliance on Static Signatures

The use of signatures, or software code that inspects network traffic to
look for known content, ports, and protocols, has been a fundamental
part of cybersecurity practice. Similar to how anti-virus software
works, intrusion detection and prevention technologies inspect traffic
to look for matches against signatures of known malicious content or
behavior. Although signature-based technology is widely accepted as an
effective and necessary piece of cyber defense, it is not enough to
protect against the most advanced and persistent threats facing the
Government today. NCPS uses signatures within their E2 intrusion
detection and E3A prevention capability areas. In recognition of the
limitations of signature-only systems, DHS has been piloting an
anomalous analytics capability that leverages artificial intelligence to
detect malicious activity across networks that will allow DHS to both
respond to previously unidentified incidents. DHS can then rapidly
generate new signatures for both EINSTEIN sensors and agency defenses to
protect the Government from those threats. DHS has seen some early
success from this pilot and is planning to build a production-grade
system that could be deployed at various points across the .gov
architecture, both inside and outside agency network and computing
enclaves.

## Use and Value of Classified Indicators

The use of signatures in intrusion detection and prevention systems are
based on pieces of information known as cyber threat indicators. These
“indicators” can be any piece of observable information about the
network traffic such as an Internet Protocol (IP) address, domain name,
or file hash, that may indicate whether the traffic entering or exiting
a network may be suspicious or malicious. DHS sources its indicators
from multiple sources to include in-house analysis of Government
traffic, commercial and open-source cyber threat data, and the
intelligence community. Although all of the signatures within the E2
system are unclassified, significant portions of the signatures in the
E3A intrusion prevention capability are classified. The use of
classified indicators and signatures within the E3A system has been a
long-standing challenge for the NCPS program because of the
unprecedented way in which classified information is placed on
unclassified networks for the purposes of protecting unclassified .gov
network traffic. The continued use of classified information in E3A has
been recognized as a cost and schedule driver, as well as limiting the
range of technical capabilities available. Moreover, the use of
classified information has limited the ability of DHS to engage and
communicate with the agencies it helps to protect because not all
agencies have personnel with the appropriate security clearances to
discuss the indicators or the alerts that are generated by the system.
To address this issue, DHS has commissioned a study to understand the
value of using classified indicators within E3A to determine if their
use should be continued, or if DHS and the agencies would be better
served by using only unclassified information.

[^29]: See Footnote 9.

[^30]: DHS Office of the Inspector General, *Implementation Status of
    EINSTEIN 3 Accelerated*. March 2014.

[^31]: U.S. Government Accountability Office, Report 16-294, *DHS Needs
    to Enhance Capabilities, Improve Planning, and Support Greater
    Adoption of its NCPS*. January 2016.
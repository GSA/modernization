---
layout: base

appendix: true

title: "Appendix E: Legal Considerations"
permalink: /report/appendices/legal-considerations/

---

## Introduction

Executive Order 13800, [*Strengthening the Cybersecurity of Federal Networks and Critical Infrastructure*][EO13800] requires this report to “describe the legal...considerations...relevant to...” transitioning
agencies to consolidated network infrastructures or shared services.
Exec. Order No. 13,800, 82 FR 22391, § 1(c)(vi)(B)(2) (May 11, 2017).
This appendix, along with the report itself, does so. The report
suggests increased use of consolidated network architectures and shared
services. Generally, Federal law contemplates that agencies control
their own systems and information either directly or through contract.
Moving to consolidated network architectures, commercial cloud and
shared services generally involves moving away from agency control and
thus tends to increase tension with relevant law and requires greater
analysis and legal documentation. While additional legal review and
documentation would need to be performed during any eventual development
of the consolidated network architectures, commercial cloud, and shared
services based on their exact facts, implementation of the report’s
recommendations can likely be achieved within existing law in most
instances, as long as they are designed with a view toward satisfying
applicable legal requirements. A summary of some of the main areas of
law and legal issues implicated by this report are discussed below.

## The Federal Information Security Modernization Act of 2014 (FISMA)

The Federal Information Security Modernization Act of 2014 (FISMA) and
later amendments are codified in subsection II of chapter 35 of title 44
of the U.S. Code. These provisions, which we will refer to here as
FISMA, create a whole-of-Government approach to Federal information
security[^32] pursuant to which OMB oversees agency information security
policies and practices; DHS administers implementation of these policies
and practices for Federal, civilian, executive-branch agencies,
including by assisting agencies and providing certain Government-wide
protections; and agencies are responsible for providing information
security protections commensurate with the risk and magnitude of the
potential harm to their agency information and information systems.
*See* 44 U.S.C. §§ 3551-3558. FISMA also requires agencies to implement
a minimum set of information security controls and techniques, assess
the effectiveness of these controls, comply with NIST standards, DHS
directives, and OMB policies, and report certain cybersecurity
information to DHS, OMB and to Congress. The consolidated network
architectures, commercial cloud, and shared services recommended in this
report will need to provide levels of security and transparency that
enable agency heads to ensure compliance with FISMA and its related
requirements, while also providing technical solutions that fit the
needs of multiple agencies.

## The Homeland Security Act’s Federal Intrusion Detection and Prevention System

The Homeland Security Act, as amended, requires DHS to “deploy, operate,
and maintain” and “make available for use by any agency” capabilities to
detect cybersecurity risks in agency network traffic and take actions to
mitigate those risks. 6 U.S.C. § 151(b)(1). DHS currently provides these
capabilities through its EINSTEIN program and, as required by law,
ensures all retention, use, and disclosure of information obtained
through EINSTEIN occurs only for the purpose of protecting information
and information systems from cybersecurity risks. *See id*. § 151(c)(3).
Federal law also requires agencies to apply these capabilities to “all
information traveling between an agency information system and any
information system other than an agency information system.” *Id.*
§ 151, note. Because this statutory mandate defines “agency information
system” as any “system owned or operated by an agency,” the statutory
mandate itself does not always require agencies to apply those
capabilities to systems operated by contractors. But existing policy
requires broader application of EINSTEIN, and DHS and agencies can
choose to apply the capabilities to contractor-operated systems.

## Privacy Statutes

There are many provisions of law and regulation that that protect
personally identifiable information by, for example, limiting access.
*See, e.g.*, U.S. Const. amend IV; Fed. R. Crim. Pro. 6(e)(2)(B) (grand
jury confidentiality rule); 5 U.S.C. § 552a (Privacy Act of 1974); 26
U.S.C. § 6103 (restrictions on access to tax return information); 13
U.S.C. § 9(a) (Census confidentiality statute); 18 U.S.C. § 2511
(Wiretap Act); 6 U.S.C. § 151 (DHS’s Federal Intrusion Detection and
Prevention System). Personnel operating consolidated network
architectures, commercial cloud, and shared services described in this
report will sometimes require access to such information. Technical
capabilities and administrative processes will need to be developed to
enable compliance with the laws and regulations applicable to each type
of information. This will require a significant role for SAOPs and
agency privacy programs.

## Request for Information from Third Parties

Agencies receive requests for information in their possession through
various means, including, for example, Freedom of Information Act (FOIA)
requests, Privacy Act requests, congressional requests, Government
Accountability Office audits, Inspector General inquiries, court
proceedings, requests from the White House or other agencies, and other
legal process. Legal agreements between shared service providers and
client agencies will be required to define who will be responsible for
responding to such requests when the information resides in a shared
service in a way that satisfies legal requirements and provides agencies
with sufficient control over their own information. Likewise, agency
notices and regulations should adequately inform the public and others
who might make requests of the appropriate procedures for accessing
information.

## The Federal Information Technology Acquisition Reform Act (FITARA)

The Federal Information Technology Acquisition Reform Act (FITARA)
increases the authority of agency Chief Information Officers to play a
significant role in the planning, programming, budgeting, management,
governance and oversight of Federal information technology. 40 U.S.C. §
11319(b)(1)(A). FITARA is consistent with a move toward consolidated
network architectures, commercial cloud, and shared services and
enhances the legal authority for agency CIOs move in that direction.
Among other actions, FITARA and associated policy require agencies to
implement data center consolidation strategies that support (i) movement
of information technology infrastructure to the as-a-service model and
(ii) transition to the cloud. *See* 44 U.S.C. § 3601, note.

## Procurement and Fiscal Considerations

Transitioning to consolidated network architectures and shared services
requires consideration of how those products or services will be
acquired and funded. In order to consolidate and share services with
each other, Federal agencies will need to enter into Interagency
Agreements or other appropriate agreements with each other that outline
the parameters of their relationship and the applicable authorities that
govern, for example, the acquisition of the products or services, how
they will be shared and utilized by the parties, and how they will be
funded and reimbursed. The specific authorities may vary depending on
the circumstances and agencies affected, but may include:

-   The Economy Act, 31 U.S.C. § 1535, which authorizes Federal agencies
    to enter into agreements to obtain supplies or services from
    another Federal agency and requires full reimbursement.

-   Agency-specific authorities. For example, 40 U.S.C. § 501 authorized
    GSA to procure and supply property and services for executive
    agencies. The funding source utilized in conjunction with 40
    U.S.C. § 501 will depend on which office within GSA is providing
    the property and services, but may include the Acquisition
    Services Fund (40 U.S.C. § 321), a Working Capital Fund, or other
    specific authorities. In general, full reimbursement will be
    required unless specifically authorized otherwise. In an example
    of such a specific authorization, 44 U.S.C. § 3553(b)(6)(B)
    authorizes DHS to “upon request by an agency, deploy\[\],
    operate\[\], and maintain\[\] technology to assist the agency to
    continuously diagnose and mitigate against cyber threats and
    vulnerabilities, with or without reimbursement.”


[^32]: In FISMA, the term “information security” means protecting
    information and information systems from unauthorized access, use,
    disclosure, disruption, modification, or destruction in order to
    provide—

    \(A) integrity, which means guarding against improper information
    modification or destruction, and includes ensuring information
    nonrepudiation and authenticity;

    \(B) confidentiality, which means preserving authorized restrictions on
    access and disclosure, including means for protecting personal privacy
    and proprietary information; and

    \(C) availability, which means ensuring timely and reliable access to and
    use of information.

[EO13800]: https://www.whitehouse.gov/the-press-office/2017/05/11/presidential-executive-order-strengthening-cybersecurity-federal

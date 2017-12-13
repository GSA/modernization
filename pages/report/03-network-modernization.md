---
layout: base

title: Network Modernization & Consolidation
permalink: /report/network-modernization/

subnav:
  - text: Summary of Efforts to Date
    href: "#summary-of-efforts-to-date"
  - text: Current State
    href: "#current-state"
  - text: Future State & Objectives
    href: "#future-state--objectives"
  - text: Implementation Plan
    href: "#implementation-plan"
---

## Summary of Efforts to Date

The Federal Government has engaged in several efforts to modernize
existing IT systems, to improve processes for the acquisition and
development of new solutions, and to restructure underlying frameworks
for service and lifecycle management. The [*E-Government Act of 2002*][EGOV2002] recognized the importance of a well-managed, modern, and secure Federal IT ecosystem, building upon concepts captured in the Clinger-Cohen Act, the *Paperwork Reduction Act*, and OMB Circular A-130, [*Managing Information as a Strategic Resource*][A-130].[^6] Additionally, the [*Federal Information Security Management Act of 2002*][FISMA2002] and, subsequently, [*the Federal Information Security Modernization Act of 2014*][FISMA2014], serve as the governing authority for OMB to provide overall guidance and policy for Government-wide Federal cybersecurity.

Pursuant to these authorities, OMB established the IT Infrastructure
Optimization Line of Business, which developed common Government-wide
performance measures for service levels and costs, identified best
practices, and provided guidance for agency IT infrastructure transition
plans. An Enterprise Architecture and Centralizing Infrastructure was
constructed some years later, and in 2010, the Federal Data Center
Consolidation Initiative (FDCCI) directed agencies to inventory their
data centers, develop consolidation plans, and assess virtual or cloud
alternatives.[^7]

Between the launch of the FDCCI and its conclusion in 2015, the Cloud
First Initiative and the Federal Risk and Authorization Management
Program (FedRAMP) were activated in 2011, with FedRAMP providing a
standardized approach to security assessment, authorization, and
continuous monitoring for cloud products and services. Driven by the
momentum of these and other efforts, in 2016 the Data Center
Optimization Initiative arose as an update to the FDCCI based on
requirements of the *Federal IT Acquisition Reform Act* (FITARA).[^8]
These efforts have helped agencies to begin modernizing their IT and
this Report is intended to help resolve some of the impediments surfaced
throughout implementation of those efforts and further accelerate
Federal IT modernization.

Transitioning to consolidated network architectures and shared services
requires consideration of how these products or services will be
acquired. Current challenges associated with use of commercial
acquisition practices limit the Federal Government’s ability to achieve
the modernization goals.

There are statutory and regulatory requirements that prevent the use of
accepted commercial best acquisition practices. Changes and
modifications to the existing acquisition requirements could be
implemented to achieve efficiencies while maintaining the core tenet of
fairness.

## Current State

In recent years, Government-wide initiatives and policies have focused
on the transition to a more efficient, more secure, and customer-focused
IT environment. The preponderance of efforts to protect Federal IT
systems to date have been focused at the network level. This drove
agencies to consolidate human and technical resources around a limited
number of connections and standardized physical access points, with the
intent of producing more robust security management.

Current policy, agency prioritization, and associated investments
prioritized through the budget process have emphasized perimeter
network-based security protections. This is manifested most visibly
through the Trusted Internet Connections (TIC) and National
Cybersecurity Protection System (NCPS) programs.[^9] This report
recommends emphasizing a layered defensive strategy in Government-wide
programs, through increasing emphasis on application and data-level
protections. This shift in focus, coupled with lessons learned from the
current implementation and advances in technology will drive strategic
changes to the NCPS program, as described in Appendix C. It will also
provide greater defense-in-depth capabilities that will help prevent
malicious actors from moving laterally across linked networks to access
large amounts of valuable information.

These well-intentioned initiatives have resulted in security
implementations that negatively affect performance and create barriers
to use of commercial technology. As an example, policy and existing
implementation of enterprise cybersecurity tools drives the physical
consolidation of all network traffic to and from Federal information
systems. This hampers agencies’ ability to acquire new technologies like
commercial cloud, which rely on a distributed network model and
emphasize optimization of virtual rather than physical controls of data.
In this case, policies and supporting capabilities which require routing
all traffic through a limited number of on premise access points not
only impacts service performance and availability, but it also
undermines the value proposition of a distributed cloud architecture and
flexible mobile access to services.

Consequently, in order to successfully meet their mission and business
objectives, agencies often circumvent network-based security protections
to use commercial cloud. Another negative consequence of overreliance on
network-based protections is the emergence of operational capability
gaps at other levels, such as the data and application levels. This has
resulted in overlooked areas of the IT ecosystem, which are more
vulnerable and at higher risk of attack or exploit.

Additionally, when individual agencies issue
agency-specific IT contracts, they reinforce the current emphasis on
boundary protections and limit opportunities for applying economies of
scale in provisioning common network and security services for the
Federal Government. Small agencies, especially, often lack staff
resources and technical expertise to securely manage existing networks,
migrate to new computing models, and navigate security acquisition
processes. Enabling a new approach to modernization and consolidation of
networks requires a strategy that addresses each of these challenges
with associated recommendations for legal, policy, resource allocation,
acquisition, and workforce interventions, as detailed further below.

## Future State & Objectives

The future of Federal IT is one in which agencies move further toward a
risk-based approach to securing their systems that places appropriate
emphasis on data-level protections and that fully leverages modern
virtualized technologies. This renewed focus on data-level protections
for managing risk must be accepted and driven by agency leadership,
mission owners, IT practitioners, and oversight bodies. Specific
recommendations that will bridge to this future state are detailed in
the next section, titled “Implementation Plan.” The following broad
objectives will drive momentum toward the future state of IT:

### Reduce the Federal attack surface through enhanced application and data-level protections.

Rather than treating Federal networks as trusted entities to be defended
at the perimeter, agencies should shift their focus to placing
protections closer to data, specifically through improved management and
authentication of devices and user access, as well as through encryption
of data – both at rest and in transit. This approach curtails an
attacker’s likelihood of gaining access to valuable data solely by
accessing the network, and it has the potential to better block and
isolate malicious activity. As agencies prioritize their modernization
efforts, they should implement the capabilities that underpin this model
to their high value assets first.

### Improve visibility beyond the network level.

Agencies will gain greater visibility and resilience against more
sophisticated attacks, including insider threats that may have access to
agency-owned networks by enhancing protections closer to the data.
Expanding visibility beyond the network level – for instance, through
collecting security logs at the application level or establishing a
vulnerability disclosure policy and placing systems or applications
under a bug bounty program – provides security teams with other
information feeds, which they can use to better understand, process, and
triage information security events and possible incidents. This
information can provide insight into the gaps in security that agencies
are experiencing, which informs the types of investments they should
make to defend against modern threats. Maximizing the effectiveness of
this approach requires updating tools and models by which staff conduct
operational security to detect and prevent intrusions. It also requires
risk-proportionate application of security practices and maintenance of
situational awareness, particularly in scenarios in which Federal
information resides in an off-premises environment, such as in
commercially-provided clouds. Government-wide programs designed to
deliver these tools and services must evolve, as must the operational
culture by which agencies collect and analyze logs and interact with the
security research community.

### Ensure that policy, resource allocation, acquisition, and operational approaches to security enable use of new technology without sacrificing reliability or performance.

Information technology policy, resource allocations, acquisition
processes, and operational guidance must enable the achievement of
security objectives while also allowing agencies to take advantage of
newer approaches to technology, such as commercial cloud-based services
and mobile devices. Agencies should prioritize the IT resources and
technical personnel they need to implement necessary data protections
and provide situational awareness in their daily operations, whether
information is stored on premises or in a commercial cloud. While some
successes have occurred in the Federal Government, many real or
perceived impediments remain to accelerating network consolidation and
optimization on a Government-wide scale. The recommendations in this
report collectively address and seek to remedy impediments to
modernizing Federal IT. Addressing these barriers will enable agencies
to accelerate toward a new era of modernization without sacrificing
security or performance.

## Implementation Plan

This section outlines immediate next steps and long-term considerations
related to the modernization of Federal networks. The focus areas below
accelerate Federal efforts on three core concepts: (1) prioritizing high
value assets; (2) adopting security frameworks that better protect
systems at the data level; and (3) consolidating and standardizing
network acquisitions and management wherever possible.

### 1.  Prioritize the Modernization of High-Risk High Value Assets (HVAs)

The HVA Initiative, which began in 2015, was a seminal step in helping
the Federal Government recognize, categorize, and prioritize
modernization and security improvements for the primary benefit of its
“crown jewel” systems.[^10] The implementation plan outlined below goes
a step further by recommending specific policy, resource allocation, and
other interventions to provide near-term assistance to agencies as they
strengthen their ability to protect these assets, which are susceptible
to the greatest amount of cybersecurity risk. It leverages the current
ATC supported efforts to improve the Authority to Operate (ATO) process,
and it corresponds with the direction set forth in Section 1 of EO
13800, which mandates that all agencies perform a risk assessment and
identify areas in which additional attention is needed. This is
consistent with agency responsibilities under FISMA.

Simply applying the next set of patches to these systems and tacking on
additional tools is no longer sufficient; rather, HVAs must be driven
toward implementation of modern architectures that are based on
data-level protections. Systems that are most important to the Federal
Government, yet are also most vulnerable, should be addressed first.

Next steps to support this recommendation are as follows:

**Immediate Action:**

It is recommended that the President direct the implementation of the
plan outlined below to improve the security of high-risk HVAs by
migrating to a modernized architecture and employing security best
practices.

**Within 30 days of the date of issuance of this final report:**

Consistent with relevant portions of the enterprise risk management
plan to be developed pursuant to Section 1(c)(iv) of EO 13800,
Commerce’s National Institute of Standards and Technology (NIST) will
provide OMB with a plan to promote a risk management culture that
focuses agency effort on the operational performance and compliance of
their most valuable systems, while simultaneously allowing for the
deployment of low-impact systems in a less burdensome and less costly
manner. This plan will include a process and timeline for revising
Federal Information Processing Standard (FIPS) Publication 199,
*Standards for Security Categorization of Federal Information and
Information Systems*, and FIPS Publication 200, *Minimum Security
Requirements for Federal Information and Information Systems*. The
plan should also include proposed updates to any other relevant NIST
Special Publications (SPs) to enable and support improvements in
agency risk management processes that lead to the appropriate
selection, implementation, and continuous monitoring of controls and
capabilities commensurate with the risk to information, systems,
agency missions, and individuals. These updates should include the use
of the NIST Framework for Improving Critical Infrastructure
Cybersecurity (Cybersecurity Framework), and, where appropriate,
incorporate lessons from other control and compliance frameworks, such
as ISO, SOC 2 Compliance Audits, and Payment Card Industry. These
updates should review the security requirements for these other
frameworks and system approval processes used, and assess the use of
overlays of these frameworks as a viable approach and intended for
inclusion into the proposed updates of the relevant Special
Publications.

**Within 60 days of the date of issuance of this final report:**

Consistent with Section 1(c)(iv)(B) of EO 13800, DHS, in consultation
with OMB, will provide a report which identifies common areas of
weakness in Government HVAs. The report will include recommendations
for addressing these risks Government-wide, informed by agency risk
assessments, as well as past and current Risk Vulnerability
Assessments (RVAs), and Security Architecture Reviews (SARs) DHS has
performed on various agency HVAs.

NIST will provide OMB with a plan to improve cryptographic agility in
the Federal enterprise. This plan will include a process and timeline
for revising FIPS Publication 140-2, *Security Requirements for
Cryptographic Modules*, as well as plans for future cryptographic
transitions. The plan will describe how the Federal Government can
maintain strong standards for the cryptographic hardware and software
modules it uses, while ensuring that associated processes help the
Federal Government make rapid use of new cryptographic primitives and
advances.

**Within 90 days of the date of issuance of this final report:**

Pursuant to its statutory authorities and in execution thereof, OMB
will update the annual FISMA metrics as well as the Cybersecurity
Cross-Agency Priority (CAP) Goal metrics to focus on those critical
capabilities that are most commonly lacking among agencies. OMB will
focus oversight efforts, including CyberStat Reviews and President’s
Management Council (PMC) Cybersecurity Assessments, on driving
progress on these capabilities, with a specific focus on HVAs.

DHS, in consultation with OMB, will work with agencies, including by
issuing direction when appropriate, to support mitigation actions to
address common areas of risk identified in the Report to the President
on Risk Management in accordance with their authorities.

**Within 120 days of the date of issuance of this final report:**

Consistent with Section 1(c)(iv)(B) of EO 13800 and in execution of
their independent statutory authorities, OMB and DHS, will develop a
strategy for an approach that clearly describes the lines of authority
and operating procedures necessary. This strategy will optimally
realign resources across agencies to reduce the risk to HVAs across
the Federal enterprise and respond to cybersecurity incidents for
those assets. These efforts should align with the recommendations
identified in the plan to adequately protect the executive branch
enterprise in response to agency risk management reports, per Section
(1)(c)(iv) of EO 13800.

**Within 150 days of the date of issuance of this final report:**

CIOs, Chief Information Security Officers (CISOs), and SAOPs will
review their latest submission of HVAs to DHS and OMB, and will make
any necessary changes to reflect the latest information on system
prioritization in tandem with the assessments made under their risk
assessments as part of Section 1 of Executive Order 13800.

**Within 180 days of the date of issuance of this final report:**

DHS, OMB, and the National Security Council (NSC) will review HVA
lists submitted to DHS by Federal agencies and will produce a
prioritized list of systems for Government-wide intervention. Six HVAs
will be selected to receive centralized interventions in staffing and
technical support, and the broader, prioritized list will be vetted by
the PMC. Additionally, agencies will work with OMB to reallocate their
IT resources appropriately in order to align and adequately resource
the modernization of HVAs.

Consistent with the current HVA Program that is administered by DHS
and overseen by OMB, any agency that has an HVA that has been
identified as having a major or critical weakness in either a risk
assessment, RVA, SAR, or an agency-sponsored review will identify a
remediation plan. Where the corrective action for a critical weakness
for an HVA can be attributed to obsolete or unsupported technology, or
critical deficiencies in the solution architecture, the remediation
plan shall include a proposal for accelerating modernization within
one year and identification of impediments in policy, resource
allocation, workforce, or operations. This plan should maximize use of
shared IT services, implement application and data-level protections,
and emphasize appropriate use of FedRAMP authorized cloud-based
architectures. Specific recommendations for modern security approaches
are described in Appendix A. Agencies should prioritize existing
financial and human resources and should identify other systems of
concern that may suffer from similar issues, but that are not
categorized as HVAs.

Where possible and subject to funding, OMB, through the U.S. Digital
Service (USDS), and GSA will support DHS in providing hands-on
technical assistance to agencies in bolstering protections for systems
identified through this process as having the greatest need for
modernization.

Additionally, DHS will work to expand the availability of RVAs and
SARs for agency HVAs. OMB will also work with DHS to refocus these
assessments to concentrate on hands-on technical engineering
interventions, de-emphasizing the review of system documentation and
policies. In addition, OMB and DHS will work with GSA to expand the
visibility, offerings, and agency use of the Highly Adaptive
Cybersecurity Services Special Item Numbers (HACS SINs) on IT Schedule
70.

**Within 365 days of the date of issuance of this final report:**

Pursuant to its statutory authorities and in execution thereof, OMB
will work with DHS, GSA, and other stakeholders to capture standard
operating procedures for the protection of HVAs and will develop a
playbook that agencies can leverage to expand this approach to other
systems in a prioritized, risk-based fashion in accordance with FISMA.

### 2. Modernize the Trusted Internet Connections (TIC) and National Cybersecurity Protection System (NCPS) to Improve Protections, Remove Barriers, and Enable Commercial Cloud Migration.

The perimeter-based security model employed by Federal agencies today,
formalized in OMB Memorandum M-08-05, *Implementation of Trusted
Internet Connections (TIC)*, focuses on standardizing security at the
network boundary by consolidating external access points. Under this
model, agencies are required to reduce external connections to a target
of 50 and route their traffic through this limited number of secure
gateways. These gateways apply common security protections, as well as
common intrusion detection, information sharing, and prevention
capabilities under DHS’s NCPS. NCPS consists of three sensor
capabilities, collectively referred to as EINSTEIN, as well as a set of
analytic tools used by cyber analysts to find, identify and categorize
cyber threat activity.[^9]

The NCPS sensor suite is deployed in three iterations: EINSTEIN 1, which
captures and analyzes network flow information; EINSTEIN 2, which
incorporates intrusion detection technology that scans the content of
network communications to identify and alert users to known indications
of malicious activity; and EINSTEIN 3-Accelerated (E3A), which detects
and blocks malicious activity through domain name systems (DNS)
sinkholing and email filtering. The TIC policy, and subsequently the
*Federal Cybersecurity Enhancement Act of 2015*, requires agencies to
utilize these capabilities, which are currently provided through NCPS,
to protect all information traveling between an agency information
system and any external information system.[^12] This perimeter-based
model sought to provide a means to aggregate all Federal Executive
Branch traffic so that the Government can apply common methods, such as
classified indicators, to protect against information security threats
and maintain consistent situational awareness.

This approach of perimeter-based network security has created several
challenges for agencies wishing to take advantage of commercial cloud
services.[^13] DHS recognizes these challenges, and has articulated
initial steps toward addressing these specific challenges in Appendix C
of this report. DHS will provide recommendations on how the NCPS and
Continuous Diagnostics and Mitigation (CDM) programs can be updated to
enable a layered security architecture that facilitates transition to
modern computing in the commercial cloud.

Next steps to support this recommendation are as follows:

**Immediate Action:**

It is recommended that the President direct the implementation of the
plan outlined below to accelerate secure use of commercial cloud
through the modernization of the NCPS Program and TIC capabilities,
policies, reference architectures, and associated cloud security
authorization baselines. This effort will support the prioritization
of security resources from lower-value assets to higher-value assets,
enabling agencies to build out data-level protections in furtherance
of a layered security architecture, and directly accelerating
commercial cloud adoption. This effort will be driven by agency use
cases, which will also be used to inform rapid updates to policy. This
modernization effort will prioritize work to focus on cloud-ready
projects and target agencies struggling to comply with the TIC policy
and cloud adoption efforts to provide more immediate relief. The goal
is to accelerate migration on three cloud-ready systems within the
next year. OMB will codify this plan in an update to TIC policy, to
provide agencies clear direction on the path forward. The entire
process described below will be overseen directly by the ATC,
including weekly status updates to the Director of the ATC regarding
progress.

**Within 30 days of the date of issuance of this final report:**

Pursuant to its statutory authorities and in execution thereof, OMB
will submit a data call to agencies requesting submission of both
in-progress and pending projects for cloud migration. Agencies should
focus submissions on projects that have experienced delays due to
constraints in current TIC policy and NCPS program implementation, and
should propose a migration plan that highlights needed changes to
requisite policies and capabilities to facilitate faster migration.

**Within 60 days of the date of issuance of this final report:**

The ATC, supported by GSA, will include the FedRAMP project management
office (PMO) and the Technology Transformation Service (TTS), DHS, OMB
to include USDS, NSC, and other relevant parties will review these
submissions and bucket them into three categories:

1.  Systems that are sufficiently low risk to migrate to cloud
    immediately. These systems will be migrated to the cloud, and
    lessons learned will be captured and used to pilot further changes
    to existing policy. These systems will also be the focus of
    additional updates to the FedRAMP baselines to explore further
    tailoring of controls for low-risk systems.[^14]

2.  Systems that are high-priority cloud migration candidates but
    present a level of risk significant enough that external assistance
    is necessary to ensure secure migration. This will represent a small
    number of “implementation validation case studies” that will receive
    technical assistance in support of their migrations. Lessons learned
    from these case studies will be used to inform new approaches to TIC
    and NCPS policy and operations.

3.  Systems that are such high risk that they should not be migrated
    until further policy direction is given or capability enhancements
    are made. These systems will be assessed to evaluate whether there
    are common features or capabilities that could be provided
    efficiently, effectively, and securely by cloud service providers
    (CSPs). This analysis will serve as an input to the FedRAMP Joint
    Authorization Board (JAB) prioritization of high-baseline CSP
    offerings available to agencies wanting to migrate high-impact data
    to the cloud.

To codify this approach, OMB will provide a preliminary update to the
TIC policy that introduces a 90 day sprint during which projects
approved by OMB will pilot proposed changes in TIC requirements. This
update will also formalize the approach outlined above and in the
subsequent two sections.

**Within 90 days of the date of issuance of this final report:**

1.  For Category 1 of projects above, agencies will be given approval to
    begin cloud migration by following their proposed migration plans.
    GSA, DHS, OMB, and NSC will require collection of metrics, which
    will be used to ensure that the proposed changes to policy do not
    introduce an unacceptable level of cybersecurity risk. Agency
    project teams would capture these metrics and lessons learned from
    these migrations and submit initial findings to GSA, DHS, and OMB.
    These inputs will inform changes to the TIC policy, Reference
    Architecture (RA), and NCPS operational model and outcomes and to
    further tailoring of the FedRAMP baselines. These activities will be
    undertaken within the understanding that agency heads still own the
    risk for the system authorizations and control decisions they are
    making.

2.  For category 2 projects above, GSA, DHS, OMB, NSC, USDS, and other
    relevant parties will kick off a 90-day sprint to validate
    particular case studies. The exact number of engagements will be
    driven by staffing considerations from these organizations, but will
    consist of at minimum three test cases. These test cases will be
    operational in nature, and will validate a subset of implementation
    plans for improving the TIC policy, RA, and NCPS operational model
    and outcomes in commercial cloud.

3.  For category 3 projects above, GSA, DHS, and OMB will work with
    agencies to evaluate whether there are common features or
    capabilities that could be provided efficiently, effectively, and
    securely by CSPs. This analysis will serve as an input to the
    FedRAMP JAB’s prioritization of high-baseline CSP offerings
    available to agencies wanting to migrate high-impact data to the
    cloud.

**Within 180 days of the date of issuance of this final report:**

DHS, GSA, and OMB will use the information gathered from the
activities listed in the section immediately preceding to inform rapid
draft updates to the TIC policy, the associated reference
architectures (RA), and any appropriate NCPS operational models to
facilitate outcomes in commercial cloud. The updated draft will codify
the findings from these case studies, as well as holistically address
incentives and barriers for agencies in securely migrating to
commercial cloud solutions. Example areas that we plan to look at as
part of the case studies may include the following:

-   A recommendation as to whether (1) “all information” traveling to
    and from agency information systems hosted by commercial cloud
    providers warrants scanning by DHS through NCPS; (2) which NCPS
    capabilities are most applicable in commercial cloud environments of
    differing asset value; and (3) what new NCPS capabilities may be
    required to maximize effectiveness in a commercial cloud
    environment;

-   How the current NCPS model could be adapted to accommodate a larger
    number of access points per agency, including any number of
    virtualized access points for agencies who are migrating their
    services to cloud environments;

-   Requirements to enable lifting the constraint of two TIC Access
    Points per agency with assurance that consistent configuration
    management is applied, information is shared, and new updates are
    deployed rapidly;

    -   How agencies can best incorporate intrusion detection and
        prevention capabilities into their use of cloud services in a
        way that ensures adequate visibility to agency operators and
        helps DHS to protect Federal information. Updates to the
        capabilities outlined in applicable OMB Memoranda and DHS’s
        TIC RA to revisit the critical capabilities for boundary
        protection, de-emphasize the prescribed architectural
        implementation, and focus on capabilities, especially those
        that serve as compensating controls for commercial cloud
        environments;

    -   Which TIC capabilities, if any, are appropriate for traffic
        associated with systems protecting FISMA-Low data, or any
        lower impact data as aligned with the tasking for Commerce’s
        proposed revisions to FIPS Publication 199 and 200;

    -   The impact of allowing traffic associated with systems deployed
        to commercial cloud to not employ physical TIC protection if
        those systems meet the appropriate operational security
        capabilities for cloud described in the updated RA;

    -   Best practices agencies should follow in implementing
        protections at other levels beyond the network, including how
        these practices should be integrated with the agencies’
        network security program;

    -   Elimination of the existing TIC-related FISMA metrics and manual
        TIC Compliance Validation (TCV) process, replacing both with
        automated metric collection, to the extent possible, with a
        primary focus on both security and availability measures. This
        should leverage, to the extent possible, existing capabilities
        under the CDM program and build on previous research DHS has
        undertaken to automate TIC compliance using this program; and

    -   Options for the reallocation, if necessary, of current
        TIC-related DHS personnel and resources toward helping
        agencies resolve operational issues in cloud migration.

### 3. Consolidate Network Acquisitions and Management

The current model of IT acquisition wherein each agency, and often
multiple components within a single agency, purchase goods and services
independently has contributed to a fractured IT landscape. This creates
an inconsistent security posture and fails to maximize the buying power
of the Federal Government. To alleviate this problem, the Federal
Government is implementing category management principles to consolidate
and standardize network and security service acquisitions to take full
advantage of economies of scale, reduce burden, and dramatically improve
technical development and operations. The Enterprise Infrastructure
Service (EIS) contract is the vehicle the Government will use to
implement the strategy that achieves these goals.

Currently, GSA is transitioning agencies from the legacy Networx
contract, under which agencies purchased \$1.79 billion in network and
telecommunications services in fiscal year (FY) 2016, to a comprehensive
solution-based contract vehicle called Enterprise Infrastructure
Solutions (EIS).[^15] The purpose of EIS is to address all aspects of
agency telecommunications and network infrastructure requirements while
also leveraging the bulk purchasing power of the Federal Government. EIS
can be leveraged to help address some of the unique challenges faced by
small agencies, a community that typically lags behind the large
agencies in terms of cybersecurity capabilities.[^16] Smaller and
non-CFO Act agencies struggle to attract and retain top information
security personnel and often lack the expertise to fully manage their
information security programs. This impedes the Federal Government’s
ability to gain a full understanding of the risk to Federal networks.
EIS can be leveraged to consolidate acquisition activities and other
security services for small agency networks by focusing on the
objectives below.

***Reduce Wasteful Spending on Duplicative Security Capabilities.***
Under the current Networx contract, agencies who do not have their own
TIC capabilities must procure TIC services by purchasing the full suite
of Managed Trusted Internet Protocol Services (MTIPS) services,[^17] the
bundling of which prohibits agencies from procuring only those tools
they need, thereby increasing cost. EIS will allow agencies the
flexibility to choose *a la carte* the managed security services tools
they need to comply with MTIPS requirements, while still being protected
by the intrusion detection and prevention capabilities DHS
provides.[^18] Though a positive and cost-saving step for many agencies,
some small agencies may still struggle to procure TIC-like capabilities
in this manner due to the complexity of managing the procurement and
integration of multiple vendors; however, when paired with the proposed
revisions to the existing TIC policy and RA, agencies will be able to
make cost-effective acquisition decisions based on their existing tools
and overall risk tolerance.

***Decrease Risk by Improving Situational Awareness of Managed External
Network Connections to the Internet**.* Approximately 40 of the 102
small agencies supported by the Networx contract currently receive MTIPS
services. The result of this gap in MTIPS capabilities is a lack of
shared situational awareness regarding the network traffic traversing
Federal network boundaries. This lack of awareness makes it difficult to
conduct enhanced monitoring of network traffic and ultimately makes it
harder to perform incident response activities. Increasing this
visibility is critical to the defense of the .gov environment, and the
additional flexibilities noted above will enable the remaining agencies
to provide the requisite information.

Next steps to support the objectives outlined above are as follows:

**Immediate Action:**

It is recommended that the President direct implementation of the plan
outlined below. This plan will leverage the consolidated buying power
of the Federal Government to procure more cost effective and secure
network services.

**Within 60 days of the date of issuance of this final report:**

DHS to provide GSA and agencies with baseline configuration guidance
for Managed Security Services (MSS) capabilities offered under EIS in
order to maximize the return on investment for the security
capabilities procured by agencies and to ensure compliance with
current TIC policy.

**Within 90 days of the date of issuance of this final report:**

GSA, in coordination with DHS, shall develop a comprehensive
acquisition strategy that provides a feasibility assessment and
roadmap to accomplish the following tasks:

-   Provide a path for all small agencies to more easily and cost
    effectively utilize EIS services. This strategy should ensure the
    Federal Government is maximizing its buying power when competing
    contracts under EIS;

-   Review current security capabilities currently
    offered under MTIPS, as defined by the TIC RA, to ensure the
    capabilities provide adequate security within the current threat
    environment, and determine if any security capabilities need to be
    added or removed from the existing MTIPS baseline. This should
    include an examination, including cost analysis, of the feasibility
    of providing a service consisting only of traffic aggregation in
    order to decrease the cost burden on small agencies;

-   Identify additional areas of opportunity outside of EIS, such as bug
    bounty platforms, to consolidate acquisition of cybersecurity
    services and products; and

-   Determine the feasibility of establishing a centralized acquisition
    support function within GSA that is capable of performing
    cybersecurity-related contract management activities for small
    agencies.

**Other High-Level Actions:**

***Increase Economies of Scale through Consolidation of Contracts for
Small Agencies***. Currently, 102 Federal small agencies are supported
by the legacy Networx contract, each on separate task orders. GSA will
support these small agencies in the transition to EIS by consolidating
requirements for small agencies and is considering the best approach
to leverage a limited number of task orders to purchase the majority
of services these agencies need. Through the consolidation of common
requirements across small agencies, GSA can leverage one or a small
number of task orders under EIS to purchase the majority of services
needed for all small agencies, with an option to provide additional
specific language focused on agency-specific requirements, in order to
realize economies of scale.

***Improve Acquisitions Support for Small Agencies to Maximize the Use
of MTIPS and other Cybersecurity Services.*** For small agencies,
there are often barriers to acquiring and maximizing the benefits of
MTIPS. In addition to high costs, many small agencies lack the
appropriate expertise to draft effective task orders and the resources
to manage their MTIPS contract and hold vendors accountable for
accomplishing the work specified in Service Level Agreements (SLAs).
As such, GSA will provide guidance to small agencies on how best to
leverage its cross-agency acquisition in order to optimize their IT
investments and management throughout the procurement process. GSA
will also provide a menu of products and services to meet small agency
IT needs, leveraging GSA’s buying power and unique position in the
marketplace to transfer cost savings to small agencies.


[^6]: [*E-Government Act of 2002*][EGOV2002] (Pub. L. No. 107-347); *Information
    Technology Management Reform Act of 1996*, “Clinger-Cohen Act
    (CCA),” ([Pub. L. 104-106][PL-104-106], Division E); and *Paperwork Reduction Act of 1995* (Pub. L. No. 96-511).

[^7]: *State of Federal IT Report*, Public Release Version 1.0.

[^8]: *Federal IT Acquisition Reform Act* (included in the *National
    Defense Authorization Act for Fiscal Year 2015* – Pub. L. 113-291).

[^9]: The TIC and NCPS initiatives are further described in the
    Comprehensive National Cyber Security Initiative (CNCI), established
    by Joint Presidential Directive NSPD-54/HSPD-23; OMB Memorandum
    M-08-16, Guidance for TIC Statement of Capability Form (SOC); OMB
    Memorandum M-08-26, [*Transition from FTS 2001 to Networx*][M-08-26]; OMB
    Memorandum M-08-27, [*Guidance for TIC Compliance*][M-08-27]; OMB Memorandum
    M-09-32, [*Update on the TIC Initiative*][M-09-32]; and DHS’s TIC Reference
    Architecture. These documents provide further details on agency,
    OMB, and DHS responsibilities and reporting requirements,
    acquisition vehicles, and technical capabilities under the TIC
    initiative. The *Homeland Security Act*, as amended by section 223
    of the *Federal Cybersecurity Enhancement Act of 2015*,
    [*Consolidated Appropriations Act of 2016*][APPROPS2016] (Pub. L. No. 114-113, 129
    Stat. 2242, Division N, Title II, Subtitle B), requires DHS to
    “deploy, operate, and maintain” and “make available for use by any
    agency” capabilities to detect cybersecurity risks in agency network
    traffic and take actions to mitigate those risks (6 U.S.C.
    § 151(b)(1)). DHS currently provides these capabilities through its
    NCPS program and, as required by law, ensures all retention, use,
    and disclosure of information obtained through NCPS occurs only for
    protecting information and information systems from cybersecurity
    risks (*See id*. § 151(c)(3)). The *Federal Cybersecurity
    Enhancement Act of 2015* also requires agencies to apply these
    capabilities to “all information traveling between an agency
    information system and any information system other than an agency
    information system.” *Id.* § 151, note. Notably, these statutory
    provisions have flexibility regarding the technological means
    through which DHS offers these intrusion detection and prevention
    capabilities and is not tied to the current NCPS implementation.
    Indeed, the Homeland Security Act encourages development of these
    capabilities by requiring DHS to “regularly assess through
    operational test and evaluation in real world or simulated
    environments available advanced protective technologies to improve
    detection and prevention capabilities, including commercial and
    noncommercial technologies and detection technologies beyond
    signature-based detection, and acquire, test, and deploy such
    technologies when appropriate.” *Id*. § 151(c)(4).

[^10]: OMB Memorandum M-17-09, [*Management of Federal High Value Assets*][M-17-09].

[^12]: *Federal Cybersecurity Enhancement Act of 2015*, [*Consolidated
    Appropriations Act of 2016*][APPROPS-2016] (Pub. L. No. 114-113, 129 Stat. 2242,
    Division N, Title II, Subtitle B).

[^13]: DHS Office of the Inspector General. [*Implementation Status of EINSTEIN 3 Accelerated.*][DHS-OIG-EINSTEIN] March 2014. U.S. Government Accountability Office (GAO) Report 16-294, *DHS Needs to Enhance Capabilities, Improve Planning, and Support Greater Adoption of its NCPS*. January 2016.

[^14]: This approach was originally piloted by the FedRAMP Tailored
    baseline, which is designed to increase FedRAMP’s flexibility to
    rapidly authorize and use low-risk applications. FedRAMP Tailored
    was finalized in September 2017, and can be seen at
    https://tailored.fedramp.gov/policy/.

[^15]: The recently rescinded OMB Memorandum M-08-26, [*Transition from FTS 2001 to Networx*][M-08-26] stated that all agencies should use Networx to acquire telecommunications connectivity, including the option to
    purchase Trusted Internet Connections solutions from vendors as a
    managed service, called Managed Trusted Internet Protocol Services
    (MTIPS). As of July 2017, an OMB Memorandum mandating a similar use
    under the EIS contract does not exist.

[^16]: In this report, “large” agencies refer to the 24 agencies
    required to appoint agency Chief Financial Officers (CFOs) (i.e.,
    “CFO Act agencies”) under the *Chief Financial Officers Act of 1990*
    (31 U.S.C. §901). All other agencies aside from these 24 are
    referred to as “small” agencies.

[^17]: MTIPS providers supply small agencies with a vendor-managed
    solution that ensures compliance with OMB’s Trusted Internet
    Connection policy.

[^18]: Pursuant to 6 U.S.C. § 151.


[EGOV2002]: https://www.gpo.gov/fdsys/pkg/PLAW-107publ347/html/PLAW-107publ347.htm

[M-08-26]: https://www.whitehouse.gov/sites/whitehouse.gov/files/omb/memoranda/2008/m08-26.pdf

[M-08-27]: https://www.whitehouse.gov/sites/whitehouse.gov/files/omb/memoranda/2008/m08-27.pdf

[M-09-32]: https://www.whitehouse.gov/sites/whitehouse.gov/files/omb/memoranda/2009/m09-32.pdf

[M-17-09]: https://www.whitehouse.gov/sites/whitehouse.gov/files/omb/memoranda/2017/m-17-09.pdf

[DHS-OIG-EINSTEIN]: https://www.oig.dhs.gov/assets/Mgmt/2014/OIG_14-52_Mar14.pdf

[APPROPS-2016]: https://www.gpo.gov/fdsys/pkg/PLAW-114publ113/html/PLAW-114publ113.htm

[FISMA2002]: https://www.gpo.gov/fdsys/pkg/PLAW-107publ347/html/PLAW-107publ347.htm

[FISMA2014]: https://www.congress.gov/113/plaws/publ283/PLAW-113publ283.pdf

[A-130]: https://www.whitehouse.gov/sites/whitehouse.gov/files/omb/circulars/A130/a130revised.pdf

[PL-104-106]: https://www.govinfo.gov/content/pkg/PLAW-104publ106/html/PLAW-104publ106.htm

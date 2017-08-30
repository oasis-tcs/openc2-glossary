<p align="center">
<img src="https://www.oasis-open.org/sites/www.oasis-open.org/files/logo.png">
</p>


# OpenC2 Glossary
Version 0.1.01

27-August-2017 

## 0. Preface

### 0.1 Technical Committee:
OASIS OpenC2 Technical Committee
Chair:
  * Joe Brule (jmbrule@nsa.gov), National Security Agency
  * Sounil Yu (sounil.yu@bankofamerica.com), Bank of America

### 0.2 Editors:
  * Duncan Sparrell (duncan@sfractal.com), sFractal Consulting LLC

### 0.3 Related Work:
This glossary is related to:
  * OASIS OpenC2 Language Specification<sup>[1](#footnote01)</sup>
  * OASIS OpenC2 Firewall Acutator Profile<sup>[2](#footnote02)</sup>
  * OASIS OpenC2 SDN Acutator Profile<sup>[3](#footnote03)</sup>
  * OASIS OpenC2 Information Assurance Implementation Considerations<sup>[4](#footnote04)</sup>

Because of the use of OpenC2 in the STIX Course of Action (CoA), this glossary is also related to:
  * OASIS STIX-v2.0-Pt1-Core<sup>[5](#footnote05)</sup>
  * OASIS STIX-v2.0-Pt2-Objects<sup>[6](#footnote06)</sup>
  * OASIS STIX-v2.0-Pt3-Cyb-Core<sup>[7](#footnote07)</sup>
  * OASIS STIX-v2.0-Pt4-Cyb-Objects<sup>[8](#footnote08)</sup>
  * OASIS STIX-v2.0-Pt5-Patterning<sup>[9](#footnote09)</sup>

### 0.4 Abstract:

This Glossay is non-normative and is to inform readers 
of the OpenC2 specifications.

Cyberattacks are increasingly sophisticated, less expensive to execute, 
dynamic and automated. 
The provision of cyberdefense via statically configured products 
operating in isolation is no longer tenable. 
Standardized interfaces, protocols and data models 
will facilitate the integration of the functional blocks 
within a system or enterprise. 
Open Command and Control (OpenC2) is a concise and extensible language 
to enable the command and control of cyber defense components, 
subsystems and/or systems in a manner 
that is agnostic of the underlying products, 
technologies, transport mechanisms or other aspects of the implementation. 
The motivation behind OpenC2 was to enable 
command and control of cyber defense and recognizes it should 
be understood that a language such as OpenC2 is necessary 
but insufficient to enable coordinated cyber response. 
Other aspects of coordinated cyber response such as sensing, 
analytics, and selecting appropriate 
courses of action are beyond the scope of OpenC2.

This glossary is an informative, non-normative document to aid in the understanding of OpenC2 specifications.

### 0.5 Version:
The versioning pattern for this document will be T.L.C where:
  * T - incremented each time the OpenC2 Technical Committee approves this document as a Committee Note Draft
  * L - incremented each time the OpenC2 Language Subcommittee reviews this document and agrees to the content
  * C - incremented each time the OpenC2 GitHub as a commit to it, ie the wording is changed.

This document is a draft of 0.1.01 - ie:
* T=0 ie no drafts have yet been approved by the OpenC2 TC
* L=1 ie based on the baseline 0.1 draft imported from openc2 forum at OpenC2 TC startup
* C=1 ie this draft contains the first set of changes to the 0.1 version

Note versions can be compared on github.

### 0.6 Status:

This Working Draft (WD) has been produced by one or more TC Members; 
it has not yet been voted on by the TC 
or approved as a Committee Draft 
(Committee Specification Draft or a Committee Note Draft). 
The OASIS document Approval Process begins officially with a 
TC vote to approve a WD as a Committee Draft. 
A TC may approve a Working Draft, revise it, 
and re-approve it any number of times as a Committee Draft.


### 0.7 URI patterns

Initial publication URI:
* TODO

Permanent “Latest version” URI:
* TODO

### 0.8 Citation format
When referencing this specification the following citation format should be used:
[OpenC2 Glossary]
OpenC2 Glossary. Edited by Duncan Sparrell and TODO. Date-TODO. OASIS TODO. link TODO.

### NOTICES
(Managed by OASIS TC Administration; please don’t modify.)
Copyright © OASIS Open 2017. All Rights Reserved.
All capitalized terms in the following text have the meanings assigned to them in the 
OASIS Intellectual Property Rights Policy (the "OASIS IPR Policy"). 
The full Policy may be found at the OASIS website.
This document and translations of it may be copied and furnished to others, 
and derivative works that comment on or otherwise explain it 
or assist in its implementation may be prepared, copied, published, and distributed, 
in whole or in part, without restriction of any kind, 
provided that the above copyright notice and this section are included 
on all such copies and derivative works. However, this document itself 
may not be modified in any way, including by removing the copyright notice 
or references to OASIS, except as needed for the purpose of developing any 
document or deliverable produced by an OASIS Technical Committee 
(in which case the rules applicable to copyrights, 
as set forth in the OASIS IPR Policy, must be followed) 
or as required to translate it into languages other than English.
The limited permissions granted above are perpetual 
and will not be revoked by OASIS or its successors or assigns.
This document and the information contained herein is provided on an 
"AS IS" basis and OASIS DISCLAIMS ALL WARRANTIES, EXPRESS OR IMPLIED, 
INCLUDING BUT NOT LIMITED TO ANY WARRANTY THAT THE USE OF THE INFORMATION 
HEREIN WILL NOT INFRINGE ANY OWNERSHIP RIGHTS OR ANY IMPLIED WARRANTIES OF 
MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE.

**Table of Contents**  *generated with [DocToc](http://doctoc.herokuapp.com/)*

- [0. Preface](#0-preface)
	- [0.1 Technical Committee:](#01-technical-committee)
	- [0.2 Editors:](#02-editors)
	- [0.3 Related Work:](#03-related-work)
	- [0.4 Abstract:](#04-abstract)
	- [0.5 Version:](#05-version)
	- [0.6 Status:](#06-status)
	- [0.7 URI patterns:](#07-uri-patterns)
	- [0.8 Citation format](#08-citation-format)
	- [Notices](#notices)
- [1. Introduction](#1-introduction)
	- [1.1 Goal](#11-goal)
	- [1.2 Purpose and Scope](#12-purpose-and-scope)
	- [1.3 Terminology](#13-terminology)
	- [1.4 Normative References](#14-normative-references)
	- [1.5 Non-normative References](#15-non-normative-references)
	- [1.6 Conformance](#16-conformance)
	- [1.7 Acknowledgments](#17-acknowledgments)
- [2. Context](#2-context)
- [3. Glossary](#)
	- [3.1 A-E](#31-a-e)
	- [3.2 F-I](#32-f-i)
	- [3.3 J-N](#33-j-n)
	- [3.4 O-R](#34-o-r)
	- [3.5 S-Z](#35-s-z)
- [4. Bibliography and Endnotes](#4-bibliography-and-endnotes)

(Editor's note - remember to update ToC and ToF with each version TODO)

**Table of Figures**  

add tof here TODO

## 1. Introduction

This glossary is an informative, non-normative document to aid in the understanding 
of the OpenC2 specifications.

### 1.1 Goal

The goal of this glossary is to contain definitions for all words that 
have specific meanings in the context of OpenC2. 
This goal can be considered met if all of the terms in any of the OpenC2 Specifications or Documents
can be found in this glossary.

### 1.2 Purpose and Scope

The purpose of this document is solely informational.
The following two sections approach defining the terms from different perspectives.
Section 2 provides context in prose form since many of the words are defined with respect to each other.
Section 3 contains a list of every word in the glossary with it's definition.

Whenever a word from the glossary is used in either Section 2 or Section 3, 
it is hotlinked to it's definiton in Section 3.
Where possible, the definitions in Section 3 will mention which OpenC2 documents the term is used in.

Where possible, the definitions in Section 3 will contain 
both the OpenC2 definition as well as alternative definitions when used in other contexts.
For example the term **Action** contains both the Webster Dictionary definition 
as well the very specific OpenC2 meaning as a field in an OpenC2 command.

### 1.3 Terminology

The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”, 
“RECOMMENDED”, “MAY”, and “OPTIONAL” in this document are to be interpreted as described in 
RFC2119<sup>[10](#footnote10)</sup>.

### 1.4 Normative References
This glossary is non-normative and there are no normative references.

### 1.5 Non-normative References
This Glossary attempts to make use of definintions from other sources where possible.
The [Endnotes](#4-bibliography-and-endnotes) contain the full reference and 
endnotes are used when a definition is quoted from another source.

References cited in this glossary:

  * Webster
  * IEEE Dictionary - http://ieeexplore.ieee.org/xpls/dictionary.jsp
  * ISO
  * IETF
  * ITU
  * NIST
    * NISTIR 7298 Revision 2
  * OASIS
  * OpenC2 specs


### 1.6 Conformance
This document is informational only and is intended to help in the 
understanding of the other OpenC2 specifications.
As such, it does not play a direct role in conformance.

### 1.7 Acknowledgments
TODO
* Dave Lemire

## 2. Context
TODO text
* prose to help understand terms in context. 
* Chicken and egg on understanding terms in context of other terms. 
* Not intended to be requirements style use cases but instead just explanations to help in understanding of the words

## 3. Glossary

The words being defined are in alphabetical order, and are in **bold**. 
Where possible, definitions from other sources will be used and cited.
But the purpose of this glossary is to define terms in the context of OpenC2 
and some overloading of meanings may be necessary.
The glossary will attempt to explain the context 
- ie when OpenC2 meaning may differ from meanings in other contexts.
Acronyms will be treated like words to define.
I.e. acronyms will not be in a separate list.
When other glossary words are used in a defintion, they will be hotlinked to the glossary definition.


### 3.1 A-E

**Action** - 
(A) In context of openC2, “action” is sometime used as part of normal english e.g. 
“and deployment of automated actions in cyber relevant time.” 
(B) the first field of the openC2 command. 
The ACTUATOR executes the ACTION on the TARGET.  
The action is the verb that is what the command is to do. 
See Language Specification Section 3.3 (TODO check still that number) for the ?36? actions in openC2. 
In the example below the firewall is told to block (action=deny) an ip.
````
    {
    "action": "deny",
    "target": {
        "type": "ipv4-address",
        …
    “actuator”: {
        “type”: “firewall”,
        ...
````

**Active Defense Harbinger Distribution** - a purple team unix distro

**Actuator** - A specific field in the openC2 language. The ACTUATOR executes the ACTION on the TARGET. In the example below the firewall (an ACTUATOR) is told to block an ip
````
    {
    "action": "deny",
    "target": {
        "type": "ipv4-address",
        …
    “actuator”: {
       “type”: “firewall”,
       ...
````

**Acting** - part of IACD

**ADHD** - see Active Defense Harbinger Distribution

**Adversary** - 

**Alert** - 

**Application** - “A computer program that performs some desired function.” 
(IEEE Std 1003.5 - 1999. POSIX ADA)

**Black List** - 

**C2** - 

**C3I** - 

**CND** - 

**COA** - see Course of Action 

**Command** - in openc2 see link

**CTI** - 

**Course of Action** - get from STIX?

**Decision Making** - part of IACD

**Enclave** - 

**Enterprise** - 

### 3.2 F-I


**Firewall** -in the context of openC2, firewall denotes the firewall functionality of an actuator ie hardware and/or software system that monitors incoming and outgoing network traffic and controls that traffic (eg logs, blocks, allows) based on security policy defined by a set of rules.

**Hacker** - White or Black Hat, Red/Blue/Purple Team

**Honeypot** - 

**Host** - 

**IACD** - see Integrated Active Cyber Defense

**IDS/IPS**- 

**IEEE** - 

**Integrated Active Cyber Defense** - say something. 
See https://secwww.jhuapl.edu/iacdcommunityday/Resources/IACD%20Baseline%20Reference%20Architecture%20-%20Final%20PR.pdf

**ISO** - 

**ITU** - 

### 3.3 J-N

**JADN** - 

**JAEN** - 

**JSON** - 

**Linux** - 

**Malware** - 

**Mitigate** - one of the 37? Openc2 commands (put them all in?)

**Mitigation System Manager** - used in figure. Is it in-scope?

**Modifier** - part of OpenC2

**Module** - “ (A) A program unit that is discrete and identifiable with respect to compiling, 
combining with other units, and loading; 
for example, input to or output from an assembler, 
compiler, linkage editor, or executive routine.  
(B) A logically separable part of a program.” (IEEE Std 1633-2008 Software Reliability)

**NIST** - National Institute of Standards - an agency of the US federal government

### 3.4 O-R

**OASIS** - duh?

**Ocas** - link to a particular openC2 simulator implemented in erlang

**OpenC2** - duh?

**Orchestrator - In IT and security there are many types of orchestrators. 
in the context of openC2 the word orchestrator is defined more narrowly to mean “what goes here”

**OrchID** - 

**Peer2Peer** - 

**Point2Point** - 

**Program** - “A combination of computer instructions and data definitions 
that enable computer hardware to perform computational or control functions.” 
(The IEEE Standards Dictionary: Glossary of Terms & Definitions, IEEE Std 610.12-1990 )

**Proxy** - 

**Publish** - Subscribe - also known as Pub/Sub - 

**NixOS** - 

**Reference Implementation** - 

**Response** - 


### 3.5 S-Z

**SDN** - Software Defined Network

**Security** - ?

**Security Onion** - a blue team unix distro

**Sense Making** - part of IACD. Sense Making is the act of taking a cyber event from sensing, enriching it with meta-information, and passing the enriched information as an Action Alert to Decision Making.

**Sensing** - part of IACD. Sensing is the act a sensor creating a cyber event and passing that event to the Sense Making analytics.

**Software** - currently a ‘target’???
ISO/IEC 24765:2009 defines software as:

> (1) all or part of the programs, procedures, rules, and associated documentation of an information processing system.
> (2) computer programs, procedures, and possibly associated documentation and data pertaining to the operation of a computer system.

**Specifier** - part of OpenC2

**STIX** - 

**Target** - part of OpenC2. The ACTUATOR executes the ACTION on the TARGET. In the example below the firewall is told to block an ip (the TARGET).
````
    {
    "action": "deny",
    "target": {
        "type": "ipv4-address",
        …
        }
    “actuator”: {
        “type”: “firewall”,
        ...
        }
    }
````

**Threat** - 

**Virtual Machine** - 

**Whitelist** - 

**Yuuki** - 

## 4. Bibliography and Endnotes
1. Working Draft of <a name="footnote01">OASIS OpenC2 Language Specification</a> ;change this to proper reference format; hotlink to draft; this will be updated as LS moves thru standardization
2. Working Draft of <a name="footnote02">OASIS OpenC2 Firewall Acutator Profile</a> ;change this to proper reference format; hotlink to draft; this will be updated as profile moves thru standardization
3. Working Draft of <a name="footnote03">OASIS OpenC2 SDN Acutator Profile</a> ;change this to proper reference format; hotlink to draft; this will be updated as profile moves thru standardization
4. Working Draft of <a name="footnote04">OASIS OpenC2 Information Assurance Implementation Considerations</a> ;change this to proper reference format; this will be updated as profile moves thru standardization; hotlink to https://www.oasis-open.org/apps/org/workgroup/openc2-imple/download.php/61449/OpenC2%20IA%20Implementation%20Considerations_RCv1.0.pdf
5. STIX-v2.0-Pt1-Core - <a name="footnote05">STIX™ Version 2.0. Part 1: STIX Core Concepts</a>. Edited by Rich Piazza, John Wunder, and Bret Jordan. 03 May 2017. OASIS Committee Specification Draft 02 / Public Review Draft 02. http://docs.oasis-open.org/cti/stix/v2.0/csprd02/part1-stix-core/stix-v2.0-csprd02-part1-stix-core.html. Latest version: http://docs.oasis-open.org/cti/stix/v2.0/stix-v2.0-part1-stix-core.html.
6. STIX-v2.0-Pt2-Objects - <a name="footnote06">STIX™ Version 2.0. Part 1: STIX Core Concepts</a>. Edited by Rich Piazza, John Wunder, and Bret Jordan. 03 May 2017. OASIS Committee Specification Draft 02 / Public Review Draft 02. http://docs.oasis-open.org/cti/stix/v2.0/csprd02/part1-stix-core/stix-v2.0-csprd02-part1-stix-core.html. Latest version: http://docs.oasis-open.org/cti/stix/v2.0/stix-v2.0-part1-stix-core.html
7. STIX-v2.0-Pt3-Cyb-Core - <a name="footnote07">STIX™ Version 2.0. Part 3: Cyber Observable Core Concepts</a>. Edited by Trey Darley and Ivan Kirillov. 03 May 2017. OASIS Committee Specification Draft 02 / Public Review Draft 02. http://docs.oasis-open.org/cti/stix/v2.0/csprd02/part3-cyber-observable-core/stix-v2.0-csprd02-part3-cyber-observable-core.html. Latest version: http://docs.oasis-open.org/cti/stix/v2.0/stix-v2.0-part3-cyber-observable-core.html.
8. STIX-v2.0-Pt4-Cyb-Objects - <a name="footnote08">STIX™ Version 2.0. Part 4: Cyber Observable Objects</a>. Edited by Trey Darley and Ivan Kirillov. 03 May 2017. OASIS Committee Specification Draft 02 / Public Review Draft 02. http://docs.oasis-open.org/cti/stix/v2.0/csprd02/part4-cyber-observable-objects/stix-v2.0-csprd02-part4-cyber-observable-objects.html. Latest version: http://docs.oasis-open.org/cti/stix/v2.0/stix-v2.0-part4-cyber-observable-objects.html.
9. STIX-v2.0-Pt5-Patterning - <a name="footnote09">STIX™ Version 2.0. Part 5: STIX Patterning</a>. Edited by Trey Darley and Ivan Kirillov. 03 May 2017. OASIS Committee Specification Draft 02 / Public Review Draft 02. http://docs.oasis-open.org/cti/stix/v2.0/csprd02/part5-stix-patterning/stix-v2.0-csprd02-part5-stix-patterning.html. Latest version: http://docs.oasis-open.org/cti/stix/v2.0/stix-v2.0-part5-stix-patterning.html.
10. RFC2119 - <a name="footnote10">“Key words for use in RFCs to Indicate Requirement Levels”</a>. S Bradner, BCP 14, RFC 2119, March 1997. [Online]. Available: http://www.ietf.org/rfc/rfc2119.txt
1. =*=*=*=*=*=*=*=*=*=*=*=* need to fill in after this as refs added to document
1. make this a list of anything referenced
1. and any endnotes
1. will need to keep in sync unless MD can do it automagically
1. Webster
1. IEEE Dictionary - http://ieeexplore.ieee.org/xpls/dictionary.jsp
1. ISO
1. IETF
1. ITU
1. NIST
  * NISTIR 7298 Revision 2

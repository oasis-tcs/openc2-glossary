<p align="center">
<img src="https://www.oasis-open.org/sites/www.oasis-open.org/files/logo.png">
</p>


# OpenC2 Glossary
Version 0.1.05

19-Sep-2017 

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

This document is a draft of 0.1.05 - ie:
* T=0 ie no drafts have yet been approved by the OpenC2 TC
* L=1 ie based on the baseline 0.1 draft imported from openc2 forum at OpenC2 TC startup
* C=5 ie this draft contains the fifth set of changes to the 0.1 version

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
Substantial contributions to this specification from the following individuals are gratefully acknowledged:
* Dave Lemire
* Duncan Sparrell

## 2. Context
Section 3 is organized similar to a typical dictionary 
with the terms to be defined listed alphabetically.
Sometimes it is also helpful to understand the terms in context of other terms.
This section is an attempt to use the terms 
as they would be used in the OpenC2 context.
It is not intended to be requirements style use cases 
but instead just explanations to help in understanding of the words.
However it does attempt to be accurate.
I.e. the examples used should be valid.

_**OpenC2**_<sup>[def](#oc2)</sup> 
_**commands**_ <sup>[def](#command)</sup>
are sent from a _**producer**_<sup>[def](#producer)</sup>
 to a _**consumer**_<sup>[def](#consumer)</sup>
as shown in Figure 1.

![Producer Consumer](https://raw.githubusercontent.com/oasis-tcs/openc2-glossary/master/images/producer.png)

Figure 1

The original impetus for OpenC2 came out of the
_**Integrated Adaptive Cyber Defense**_<sup>[def](#iacd)</sup>
(IACD) work going on within the US Government, academia, and industry.
Since IACD terminology is used in some OpenC2 use cases, it will
be included here.
By leveraging automation, IACD moves human defenders from 'in the loop' 
to 'on the loop'.
IACD functionally decomposes cyber defense funtions into
_**Sensing**_<sup>[def](#sense)</sup>,
_**Sense-Making**_<sup>[def](#makesense)</sup>,
_**Decision-Making**_<sup>[def](#decide)</sup>, and
_**Acting**_<sup>[def](#act)</sup>.

## 3. Glossary

The words being defined are in alphabetical order, and are in **bold**. 
Where possible, definitions from other sources will be used and cited.
But the purpose of this glossary is to define terms in the context of OpenC2 
and some overloading of meanings may be necessary.
The glossary will attempt to explain the context 
- ie when OpenC2 meaning may differ from meanings in other contexts.
Acronyms will be treated like words to define.
I.e. acronyms will not be in a separate list.
When other glossary words are used in a defintion, 
they will be _**bold-italics**_ and hotlinked to the glossary definition by a superscript "def".
Some extremely common terms (eg. OpenC2) will not be highlighted/linked beyong the first use.


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

**Actuator** - <a name="actuator">A</a> specific field in the openC2 language. The ACTUATOR executes the ACTION on the TARGET. In the example below the firewall (an ACTUATOR) is told to block an ip
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

**Acting** - <a name="act">part</a> of IACD<sup>[def](#iacd)</sup>.
Acting is executing the commands sent by 
_**Decision Making**_<sup>[def](#decide)</sup> 
to change the state of the system.
Acting is performed by _**Actuators**_<sup>[def](#actuator)</sup>.

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

**Command** - <a name="command">From</a> the Language Specification<sup>[1](#footnote01)</sup>, "The OpenC2 Command communicates an action to be performed on a target and may include the entity that is to execute the action." See section 2 for example.

**Consumer** - <a name="consumer">The</a> entity that receives an OpenC2 command. See section 2 for example.

**CTI** - 

**Course of Action** - get from STIX?

**Decision Making** - <a name="decide">part</a> of IACD<sup>[def](#iacd)</sup>. 
Decison making is deciding what to do based on 
_**Sensing**_<sup>[def](#sense)</sup> and 
_**Sense-Making**_<sup>[def](#makesense)</sup> data, 
and on security policies. 
The decision reached result in 
_**Acting**_<sup>[def](#act)</sup> ie the sending of OpenC2 commands. 
For example sensing may detect beaconing, 
sense making augments the ip with the domain evildomain.com. 
Decision making decides to send the "mitigate evildomaing.com" 
OpenC2 command to Acting.

**Enclave** - 

**Enterprise** - 

### 3.2 F-I


**Firewall** -in the context of openC2, firewall denotes the firewall functionality of an actuator ie hardware and/or software system that monitors incoming and outgoing network traffic and controls that traffic (eg logs, blocks, allows) based on security policy defined by a set of rules.

**Hacker** - White or Black Hat, Red/Blue/Purple Team

**Honeypot** - 

**Host** - 

**IACD** - see Integrated Active Cyber Defense<sup>[def](#iacd)</sup>

**IDS/IPS**- 

**IEEE** - 

**Integrated Active Cyber Defense** - 
<a name="iacd">(IACD)</a> - is a program among the US Government, 
academia, and industry to leverage automation
to move human defenders from 'in the loop' to 'on the loop'.
See https://secwww.jhuapl.edu/IACD/ for more information.

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

**OpenC2** - <a name="oc2">In</a> the context of the OASIS OpenC2 Specifications<sup>[1](#footnote01),[2](#footnote02),[3](#footnote03),[4](#footnote04)</sup>, OpenC2 used alone is generally shorthand for the OpenC2 Language. OpenC2 used as an adjective can usually be inferred by context to mean the some aspect from the collection of the specifications.

**Orchestrator - In IT and security there are many types of orchestrators. 
in the context of openC2 the word orchestrator is defined more narrowly to mean “what goes here”

**OrchID** - 

**Peer2Peer** - 

**Point2Point** - 

**Producer** - <a name="producer">The</a> entity that sends an OpenC2 command. See section 2 for example.

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

**Sense Making** - <a name="makesense">part</a> of IACD<sup>[def](#iacd)</sup>. Sense Making is 
making sense of the data. Sense Making using involves data analytics and augmentng the data from _**Sensing**_<sup>[def](#sense)</sup>. For example adding the geolocation and netlocation of an ip address or adding reputation to the ip. The enriched data is passed to 
_**Decision-Making**_<sup>[def](#decide)</sup>.


**Sensing** - <a name="sense">part</a> of IACD<sup>[def](#iacd)</sup>. 
Sensing is the function performed by sensors in creating security data 
and passing that data to 
_**Sense-Making**_<sup>[def](#makesense)</sup>.

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

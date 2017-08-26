<p align="center">
<img src="https://www.oasis-open.org/sites/www.oasis-open.org/files/logo.png">
</p>


# OpenC2 Glossary

<p align="center">
Version 0.1.2
</p>

# 0. Preface

25-August-2017 (update once 0.1.2 stable)

## 0.1 Technical Committee:
OASIS OpenC2 Technical Committee
Chair:
  * Joe Brule (jmbrule@nsa.gov), National Security Agency
  * Sounil Yu (sounil.yu@bankofamerica.com), Bank of America

## 0.2 Editors:
  * Duncan Sparrell (duncan@sfractal.com), sFractal Consulting LLC

## 0.3 Related Work:
This glossary is related to:
  * TODO: reference language spec
  * TODO: reference profiles
  * TODO: reference implementation docs

## 0.4 Abstract:

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

## 0.5 Status:

This Working Draft (WD) has been produced by one or more TC Members; 
it has not yet been voted on by the TC 
or approved as a Committee Draft 
(Committee Specification Draft or a Committee Note Draft). 
The OASIS document Approval Process begins officially with a 
TC vote to approve a WD as a Committee Draft. 
A TC may approve a Working Draft, revise it, 
and re-approve it any number of times as a Committee Draft.


## 0.6 URI patterns:

Initial publication URI:

Permanent “Latest version” URI:

## 0.7 Copyright
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

## 0.8 Table of Contents

**Table of Contents**  *generated with [DocToc](http://doctoc.herokuapp.com/)*

- [0. Preface](#)
	- [0.1 Technical Committee:](#)
	- [0.2 Editors:](#)
	- [0.3 Related Work:](#)
	- [0.4 Abstract:](#)
	- [0.5 Status:](#)
	- [0.6 URI patterns:](#)
	- [0.7 Copyright](#)
	- [put in table of contents](#)
	- [put in table of Figures](#)
- [1. Introduction](#)
	- [1.1 Goal](#)
	- [1.2 Purpose and Scope](#)
	- [1.3 Terminology](#)
	- [1.4 Normative References](#)
	- [1.5 Non-normative References](#)
	- [1.6 Conformance](#)
	- [1.7 Acknowledgments](#)
- [2. Context](#)
- [3. Glossary](#)
	- [3.1 A-E](#)
	- [3.2 F-I](#)
	- [3.3 J-N](#)
	- [3.4 O-R](#)
	- [3.5 S-Z](#35S-Z)
- [4. Bibliography and Endnotes(#4bibliographyandendnotes)

------
put in table of Figures
------

# 1. Introduction

blah

## 1.1 Goal

blah

## 1.2 Purpose and Scope

blah

## 1.3 Terminology

blah

## 1.4 Normative References

## 1.5 Non-normative References

## 1.6 Conformance

## 1.7 Acknowledgments

# 2. Context

# 3. Glossary







This is the OpenC2 dictionary/glossary.

It is in very draft form - don’t look at it yet


Some caveat about definitions in context of openc2

Mixed definitions and abbreviations

Reference other definitions where possible
  * Webster
  * IEEE - http://ieeexplore.ieee.org/xpls/dictionary.jsp
  * ISO
  * IETF
  * ITU
  * NIST
    * NISTIR 7298 Revision 2
  * OASIS
  * OpenC2 specs

Mark each definition whether normative 
(ie for openc2 this matters) 
or informative (might help with reading explanatory information). 
Btw normative defintions need to be in a normative document 
and copied here since this will be an informative document (I assume). 
Mark normative with *.

Make in html and filterable (eg only IACD or only normative or only “keyword”)

Need style guide for glossary

Should it be wiki instead of google doc?

## 3.1 A-E

**Action** - 
(A) In context of openC2, “action” is sometime used as part of normal english e.g. 
“and deployment of automated actions in cyber relevant time.” 
(B) the first field of the openC2 command. 
The ACTUATOR executes the ACTION on the TARGET.  
The action is the verb that is what the command is to do. 
See LDD Section 3.3 for the ?36? actions in openC2. 
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

## 3.2 F-I


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

## 3.3 J-N

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

## 3.4 O-R

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


## 3.5 S-Z

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

# 4. Bibliography and Endnotes
  1. make this a list of anything referenced
  1. and any endnotes
  1. will need to keep in sync unless MD can do it automagically

Other than these first few lines, the document below is the same
as the document appoved by the OpenC2 forum.
For OASIS OpenC2 TC, this will be considered version 0.1.0
and considered the baseline.

------

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



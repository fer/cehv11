# Module 01: Introduction to Ethical Hacking

{% hint style="info" %}
**Objectives**

* Understanding the Elements of Information Security
* Understanding Information Security Attacks And Information Warfare
* Overview of Cyber Kill Chain Methodology, TTPs and IoCs
* Folder View of Hacking Concepts, Types and Phases
* Understanding Ethical Hacking Concepts and its Scope
* Overview of Information Security Controls
* Overview of Information Security Act And Laws
{% endhint %}

## 1. Information Security Overview

### Elements of information security

Information security is a state of well being of information and infrastructure in whch the possibility of theft, tampering and disruption of information and services is low or tolerable.

* **Confidentiality**: assurance that information is accessible only to those _authorized to have access_.
* **Integrity**: the _trustworthiness of data or resources_ in terms of preventing improper or unathorized changes.
* **Availability**: Ensure systems responsible for delivering, storing and processing information are accessible when _required by the authorized users_. Think of hashing algorithms.
* **Authenticity**: This refers to the characteristic of a communication, document or any data that ensures _the quality of being genuine_. Think of the digital signatures.
* **Non-repudiation**: A _guarantee_ that the sender of a message cannot later deny having sent the message and that the recipient cannot deny having received the message.

> Classic triad: CIA

### Motives, Goals and Objectives of Information Security Attacks

1. A motive originates out of the notion that the _target system stores or processes_ something valuable, and this leads to the threat of an attack on a system.
2. Attackers try various tools and attack techniques to _exploit vulnerabilities_ in a computer system or its security policy and controls in order to fulfill their motives.

#### Motives behind information security attacks

> Attacks = Motive (Goal) + Method + Vulnerability

* Disrupting business continuity
* Stealing information and manipulating data
* Creating fear and chaos by disrupting critical infrastructures
* Causing financial loss to the target
* Propagating religious or political beliefs
* Achieving a state's military objectives
* Damaging the reputation of the target
* Taking revenge
* Demanding ransom

#### Classification of attacks

* **Passive**:
  * Do not tampoer iwth the data and involve intercepting and _monitoring network traffic_ and data flow on the target network.
  * Examples: Sniffing, eavesdropping.
* **Active**:
  * Tamper with the data in transit or _disrupt the communication_ or services between the systems to bypass or break into secured systems.
  * example: DoS, MITM, Session Hijacking, SQL Injection.
* **Close-in**:&#x20;
  * They are performed with the attacker is in close physical proximity with the target system or network in order to gather, modify or _disrupt access_ to information.
  * Examples: Social Engineering, eavesdropping, shoulder surfing, dumpster diving.
* **Insider**:
  * They involve using privileged access to _violate rules_ or intentionally cause a threat to the organizations information or information systems.
    * Examples: theft of physical devices, planting keyloggers, backdoors, malware.
* **Distribution**:
  * Attackers tamper with hardware or software prior to installation, at its source of in transit.

#### Information warfare

This term refers to the _use of ICT_ to gain competitive advantages of an opponent.

**Defensive information warfare**

Refers to all the strategies and actions designed to _defend against attacks on ICT assets_.

* Prevention
* Deterrence
* Alerts
* Detection
* Emergency Preparedness
* Response

**Offensive information warfare**

Refers to information warfare that involves _attacks against the ICT assets_ of an opponent.

* Web Application Attacks
* Web Server Attacks
* Malware Attacks
* Man In The Middle Attacks&#x20;
* System Hacking

## 2. Cyber Kill Chain Concepts

* It is a component of intelligence-driven defense for the identification and _prevention of malicious intrusion activities_.
* It provides greater insight into attack phases which helps security professionals to understand the adversary's tactics, techniques and procedures beforehand.
* **Reconnaisance**: gather data on the target to prove for weak points/
* **Weaponization**: create a deliverable malicious payload using an exploit and a backdoor.
* **Exploitation**: exploit a vulnerability by executing code on the victim system.
* **Installation**: install malware on the target system.
* **Command & Control**: create a command and control channel to communicate and pass data back and forth.
* **Actions on Objectives**: perform actions to achieve intended objectives.

### Tactics, Techniques and Procedures

Patterns of activities and methods assoiciated with specific threat actors or groups of threat actors.

**Tactics**

* Guidelines that describe their _way an attacker performs the attack_ (from beginning to end).
* This guideline consist of date various tactics for information gathering to perform initial exploitation, privilege escalation and lateral movement and to deploy mesaures for persistent access to the system and other purposes.

**Techniques**

* Techniques are the _technical methods used by an attacker_ to achieve intermediate results during the attack.
* These techniques include initial exploitation, setting up and maintaining command and control channels, accessing the target infrastructure and covering the tracks of data exfiltration among others.&#x20;

**Procedures**

* Step by step.&#x20;
* Organizational approaches that threat actors follow to launch an attack.
* Mumber for actions usuarlly differs depending on the objectives of theprocedure and thread after group.

### Adversary Behavioral Identification

* It involves the identification of the common methods or techniques followed by an adversary to launch attacks on or to penetrate an organisation's network.
* it gives the security professionals insight into upcoming threats and exploits.

Adversary Behaviors:

1. Internal Reconnaisance
2. Use of PowerShell
3. Unspecified Proxy Activities
4. Use of Command-Line Interface
5. HTTP User Agent
6. Command and Control Server
7. Use of DNS Tunneling
8. Use of Web Shell
9. Data Staging

### Indicators of Compromise (IoCs)

* IoCs are the _clues, artifacts and pieces of forensic data_ found on the network or operating system of an organization that indicate a potential intrusion or malicious activity in the organization's infrastructure.
* IoCs are not intelligence although the do _act as a good source of information_ regarding the threats that serve as data points in the intelligence process.
* Security professionals need to _perform continuous monitoring_ of IoCs to effectively and efficiently detect and _respond to ever been cyberthreats_.

#### IoCs Categories

Undestanding IoCs helps security professionals to quickly detect the threats and protect the organization from evolving threats.

4 categories:

* **Email indicators**
  * They are used to send malicious data to the target organization or individual.
  * Examples: sender's email address, email subject and attachments or links.
* **Network indicators**
  * Useful for command and control, malware delivery, identifying the operating system and other tasks.
  * Examples: URLs, domain names, IP addresses.
* **Host-Based indicators**
  * Found by performing an analysis of the infected system within the organizational network.
  * Examples: filenames, file hashes, registry keys, DLLs and mutex.
* **Behavioral Indicators**
  * Identify specific behavior related to malicious activities.
  * Examples: document executing PowerShell script and remote command execution.

## 3. Hacking Concepts

### What

* Exploiting vulnerabilities and compromising security controls To gain unathorized or inappropiate access to system's resources.
* Modifying a system or application features to achieve a goal outside of the creator's original purpose.
* Steal and distribute intellectual property, leading to business loss.

### Who

1. An Intelligent individual with **excellent computer skills** who can create and explore computer software and hardware.
2. **Hobbyst** probing how many computers or networks they can compromise.
3. Someone who wants to gain knowledge or to **probe and do illegal things**.

Someone with malicious intent such as to steal business data, credit card information, social security numbers, email passwords and other sensitive data.

### Classes

* **Black Hats**: Individuals with extraordinary computer skills, they resort to malicious or disruptive activities and are also known as crackers.
* **White Hats**: They used their professed hacking skills for defensive purposes are also known as security analyst; they have permission from the system owner.
* **Grey Hats**: offensively and defenisvey at times.
* **Suicide**: aim to bring down the critical infrastructure for a "cause" and are not worried about facing jail terms or any other kind of punishment.
* **Script Kiddies**: unskilled hacker who compromises a system by running scripts, tools and software that were developed by real hackers.
* **Cyber Terrorists**: wide range of skills, motivated by religious or political beliefs to create fear through the large-scale disruption of computer networks.
* **State-Sponsored Hackers**: emplyed by the government to penetrate and gain top-secret info from and do damage to the info system of other governments.
* **Hacktivist**: they promote a political agenda by hacking, especially by defacing or disabling websites.

### The 5 stages of the hacking cycle

#### (1/5) Reconnaisance

* Preparatory phase where an attacker seeks to gather information about a target prior to launching an attack.
* This information could be the future point of return, noted for ease of entry for an attack, when more about the target is known on a broad scale.
* Target range may include the target's organization's clients, employees, operations, network and systems.

Types

* **Passive**: Involves acquiring information without directly interacting with the target, as searching public records or news releases.
* **Active**: Involves directly interacting with the target by any means, as telephone calls to the target's help desk or tech department.

#### (2/5) Scanning

* **Pre-attack Phase**: pre-attack pahse when the attacker scans the network for specific information based on information gathered during reconnaisance.
* **Port Scanner**: scanning can include the use of dialers, port scanners, netowrk mappers, ping tools and vulnerability scanners.
* **Extract Information**: attackers extract information such as live machines, port, port status, OS details, device type and system uptime to launch attack.

#### (3/5) Gaining Access

1. It refers to the point where the attacker obtains access to the _operating system or applications_ on the target computer or network.
2. The attacker can gain access to the operating system, application or network levels.
3. The attacker can escalate privileges to obtain complete control of the system. in this process the target's connected intermediate systems are also compromised.
4. Example: Password cracking, buffer overflow, denial of service and session hijacking.

#### (4/5) Maintaining Access

Attackers can revisit the system at will.

* Attacker tries to retain their ownership of the system.
* Attacker prevents the system from being owned by other attackers by securing their exclusive access with backdoors, rootkits or trojans.
* Attackers can upload, download, manipulate data, applications and configurations on the owned system.
* Attackers can use the compromised system to launch further attacks.

#### (5/5) Clearing Tracks

Attackers always cover their tracks to hide their identity.

* Activities carried out by an attacker to hide malicious acts.
* Continue accessing to the victim's system, remaining unnoticed and uncaught and deleting evidence that might lead to their prosecution.
* The eye doctor overwrites the server, system and application logs to avoid suspicion.

## 4. Ethical Hacking Concepts

* It involves the use of tools, tricks and techniques to identify vulnerabilities and ensure system security.
* Simulating the techniques used by attackers to verify the existence of exploitable vulnerabilities in the system's security.
* Perform security assessments for an organization with the permission of concern authorities.

### Why is it necessary?

To beat a hacker you need to think like one.

* Allows for counter attacks against malicious attackers through anticipating the methods used to break into the system.
* Prevent hackers from gaining access to the organization's information systems.
* Uncover vulnerabilities in systems and explore their potential as a security risk.
* To analyze and strengthen an organization's security posture, including policies, network protection infrastructure and end-user practices.
* To provide adequate preventive measures in order to avoid security breaches.
* To help safeguard customer data.
* To enhance security awareness at out levels in a business.

### Questions to answer by an Ethical Hacker

What can I do with the system? What can I see? Is anybody watching?

1. what can an intruder see on the target system? (reconnaissance and scanning phases)
2. what can an intruder do with information? (gaining access and maintaining access phases)
3. does anyone at the target organization notice the intruders' attempts or successes? (reconnaissance and covering tracks phases)
4. Are all components of the information system adequeately protected, updated and patched?
5. How much time, effort and money are required to obtain adequate protection?
6. Are the information security measures in compliance with legal and industry standards?

### Scope And Limitations

We come, we assess, we report, we recommend, but we don't fix anything.

Scope:

* Ethical hacking is a crucial component of risk assessment, auditing, counter fraud and information system security best practices.
* it is used to identify risk and highlight remedial actions.&#x20;

Limitations:

* Unless the business already know what they are looking for and why they are hiring an outside vendor in to hack systems in first place, chances are there wouldn't be much to gain from experience.
* An ethical hacker can only help the organization to better understand its security system, it's up to the organization to place the right safeguards on the network.

### Skills of an Ethical Hacker

1. Technical Skills
2. In-depth knowledge of major operating environments.
3. In-depth knowledge of networking concepts, technologies and related hw & sw.
4. Computer expert.
5. Security areas & related issues.
6. High technical knowledge for launching sophisticated attacks.
7. Non-Technicall Skills
8. Ability to elarn.
9. Strong work ethics.
10. Good problem solving.
11. Communication skills.
12. Committed to the organization's security policies.
13. Aware of local standars and laws.

## 5. Information Security Controls

### Information Assurance (IA)

* IA refers to the assurance that the _integrity_, _availability_, _confidentiality_ and _authenticity_ of information and information systems is protected during the **usage, processing, storage and transmission of the information**.

Some of the processes that help in achieving IA include:

1. Developing local policy, process and guidance.
2. Designing network and user authentication strategies.
3. Identifying network vulnerabilities and threats.
4. Identifying problem and resource requirements.
5. Creating plans for identified resource requirements.
6. Applying appropriate information assurance controls.
7. Performing certification and accreditation.
8. Providing information assurance training.

### Defense In-Depth

You never ever rely on one level of security.

* It's a security strategy in which _several protection layers_ are placed through an information system.
* It helps to prevent direct attacks against the system and its data because a break in one layer only leads the attacker to the next layer.

From outer to inner: 1. Policies, procedures and awareness. 2. Physical. 3. Perimeter. 4. Internal Network. 5. Host. 6. Application. 7. Data

### What is Risk?

* Degree of _uncertainty_ or expectation that an adverse event may cause damage to the system.
* Categorized into different levels according to their estimated impact on the system.
* A risk matrix is used to scale risk by considering the _probability_, _likelihood_ and _consequence of impact_ of the risk.
* It's not a function of the Ethical Hacker, but we need to have a global understanding about what risk is. We are reducing the risk for a customer, we are mitigating risk.&#x20;
* We'll look at vulnerability scoring systems valuing risk.

#### Risk Management

* Process of producing and maintaining risk at an acceptable level.
* Tool: actively security program.

**Phases**

* _risk identification_: identifies the sources, causes, consequences and other details of the internal/external risks affecting the security of the organization.
* _risk assessment_: assesses the organization's risk and provides an estimate of the likelihood and impact of the risk.
* _risk treatment_: selects and implements appropriate controls for the identified risks.
* _risk tracking_: ensures appropriate controls are implemented to handle known risks and calculates the chances of a new risk ocurring.
* _risk review_: evaluates the performance of the implemented risk managemente strategies.

What do we have? How bad is it? What we can do about it? How do we ensure this doesn't happen again? Is it still happenning?

#### Cyber Threat Intelligence (CTI)

* It is defined as the collection and analysis of information about threats and adversaries and the drawing of patterns that provide the ability to make knowledgeable decisions for preparedness, prevention and response actions against various cyber-attacks.
* It helps the organization to identify and mitigate various business risks by converting unknown threats into known threats.
* It helps in implementing various advanced and proactive defense strategies.

Types:

* Long-term use:
  * High-Level:
    * **Strategic**: high level information on changing risks. Consumed by high level executives and management.
  * Low-level:
    * **Tactical**: Information on attacker's TTPs. Consumed by IT Service and SOC Managers, Administrators.
* Short-term/immediate use:
  * High-level:
    * **Operational**: information on a specific incoming atack. Consumed by Security Managers and Network Defenders.
  * Low-level:
    * **Technical**: Information on specific indicators of compromise. Consumed by SOC Staff and IR Teams.

#### Threat Modeling

Risk assessment approach for analyzing the security of an application by capturing, organizaing and analyzing all the information that affects the security of an application.

1. Identify security objectives: Help to determine how much _effort needs to be put_ towards subsequent steps.
2. Application overview: Identify the _components,data flows_ and trust boundaries.
3. Decompose the application: help to find more relevant and more _detailed threats_.
4. Identify threats: Eyedentify threats relevant to the _control_ scenario and context using the information obtained in steps 2 and 3.
5. Identify vulnerabilities: _Identify weaknesses_ related to the threats found using _vulnerability categories_.

#### Incident Management

Incident management is a set of defined processes to identify, analyze, prioritize and resolve security incidents to restore normal services operations as quickly as possible and prevent future recurrence of the incident.

1. Vulnerability Handling
2. Artifact Handling
3. Announcements
4. Alerts
5. Incident Handling
   1. Triage
   2. Reporting and Detection
   3. Incident Response
   4. Analysis
6. Other Incident Management Services

#### Incident Handling and Response

* IH\&R is the _process of taking organizaed and careful steps_ when reacting to a security incident or cyberattack.

Steps involved in the IH\&R process:

1. Preparation
2. Incident Recording and Assignment
3. Incident Triage
4. Notification
5. Containment
6. Evidence Gathering and Forensic Analysis
7. Eradication
8. Recovery
9. Post-Incident Activities (review)
   * Incident Documentation
   * Incident Impact Assessment
   * Review and Revise Policies
   * Close the Investigation
   * Incident Disclosure&#x20;

#### Role of AI and ML in Cyber Security

* ML and AI are now vastly used across various industries and applications due to the increase in computer power, data collection and storage capabilities.
* ML is an unsupervised self-learning system that is used to define what the normal network looks like, along with its devices and then to backtrack and report any deviations and anomalies in real-time.
* AI and ML in cybersecurity helps in identifying new exploits and weaknesses, which can then be easily analyzed to mitigate further attacks.
* The cyber security market is to exceed $300billion by 2024 and the AI-related cyber security is predicted to reach a value of $38.2 billion by 2026.
* According to [CB Insights](https://www.cbinsights.com), alongside overall rising investment activity, many cybersecurity companies are emerging to offer novel solutions to cyber threats by leveraging the advantages of AI.
* Cybersecurity is the fourth most active industry that deals with companies applying AI.

ML classification techniques:

* **Supervised learning**: makes use of agorithms that input a _set of labeled training data_, with the aim of learning the differences between the labels.
  * Classification
  * Regression
* **Unsupervised learning**: makes use of algorithms that input _unlabeled training data_, with the aim of deducing all categories by itself.
  * Dimensionality Reduction
  * Clustering

**How do AI and ML prevent Cyber Attacks?**

1. Password protection and authentication
2. Phishing detection and prevention
3. Threat Detection
4. Vulnerability Management
5. Behavioral Analytics
6. Network Security
7. AI-based Antivirus
8. Fraud Detection
9. Botnet Detection
10. AI to Combat AI Threats

## 6. Information Security Laws and Standards

### PCI DSS: Payment Card Industry Data Security Standard

* Enforced by VISA/Mastercard
* It's a propietary _information security standard for organization_ that handle cardholder information for major debit, credit, prepaid, e-purse, ATM and POS cards.
* PCI DSS applies to all entities involved in payment card processing, including merchant, processors, acquirers, issuers and service providers, as well as all other entities that store process or transmit cardholder data.
* [https://www.pcisecuritystandars.org](https://www.pcisecuritystandars.org)

#### High Level Overview

* Build and Maintain a Secure Network
* Protect Cardholder Data
* Maintain a Vulnerability Management Program
* Implement Strong Access Control Measures
* Regularly Monitor and Test Networks
* Maintain an Information Security Policy

Failure to meet the PCI DSS requirements may result in fines or the termination of payment card processing privileges.

### ISO/IEC 27001:2013

* Specifies requirements for establishing, implementing, maintaining and continually improving an information security managemente system within the context of the organization.
* [https://www.iso.org](https://www.iso.org)&#x20;
* It's intended to be suitable for several different types of use, including:

1. Use within organizations to formulate security requirements and objectives.
2. Use within organizations to ensure that security risks are cost-effectively managed.
3. Use within organizations to ensure compliance with laws and regulations.
4. Definition of new information security management processes.
5. Identification and clarification of existing information security management processes.
6. Used by organization management to determine the status of information security management activities.
7. Implementation of business-enabling information security.
8. Use by organizations to provide relevant information about information security to customers.

### HIPAA - Health Insurance Portability And Accountability Act

* [https://www.hhs.gov](https://www.hhs.gov)

Statute and Rules:

1. Electronic Transaction And Code Set Standards: Requires every provider who does business electronically to use the same health care transactions, code sets and identifiers.
2. Privacy Rule: Provides federal protections for the personal health information held by covered entities and gives patients an array of rights with respect to that information.
3. Security Rule: Specifies series of administrative, physical and technical safeguards for covered entitities to use to ensure the confidentiality, integrity and availability of electronically protected health information.
4. National IDentifier Requirements: Requires that health care providers, health plans and employers have standard national numbers that identify them attached to standard transactions.
5. Enforcement Rule: provides the standards for enforcing all the Administration Simplification Rules.

### Sarbanes Oxley Act (SOX)

* Enacted in 2002, the Sarbanes-Oxley Acti is designed to protect investos and the public by increasing the accuracy and reliability of corporate disclosures.

The key requirements and provisions of SOX are organized into 11 titles:

* Title I: _Public Company Accounting Oversight Board (PCAOB)_ provides independent oversight of public accounting firms providing audit services ("auditors").
* Title II: _Auditor Independence_ Establishes the standards for external auditory independence, intended to limit conflicts of interest and address new auditor approval requirements, audit partner rotation and auditor reporting requirements.
* Title III: _Corporate Responsibility_ mandates that senior executives take individual responsibility for the accuracy and completeness of corporate financial reports.
* Title IV: _Enhanced Financial Disclosures_ describe enhacned reporting requirements for financial transactions, including off balance sheet transactions, pro-forma figures and the stock transactions of corporate officers.
* Title V: _Analyst Conflicts of Interest_ consist of measures designed to help restore investors confidence in the reporting of securities analysts.
* Title VI: _Commission Resources and Authority_ defines practices to restore investor confidence in securities analyst.
* Title VII: _Studies and Reports_ includes the effect of the consolidation of public accounting firms, the role of credit rating agencies in the operation of securities markets, securities violatioans and enforcement actions and whether investment banks assisted Enron, Global Crossing or others to manipulate earnings and obfuscate true financial conditions.
* Title VIII: _Corporate and Criminal Fraud Accountability_ Describes specific criminal penalties for fraud by the manipulation, destruction or alteration of financial records or other interference with investigations while providing certain protections for whistle-blowers.
* Title IX: _White Collar Crime Penalty Enhacement_ increases the criminal penalties associated with white-collar crimes and conspirancies. It recommends stronger sentencing guidelines and specifically adds the failure to certify corporate financial reports as a criminal offence.
* Title X: _Corporate Tax Returns_ states that the CEO should sign the company tax return.
* Title XI: _Corporate Fraud Accountability_ identifies corporate fraud and record tampering as criminal offenses and assigns them specific penalties. It also revises sentencing guidelines and strengthens their penalties. This enables the SEC to temporarily freeze large or unusual payments.

### The Digital Millennium Copyright Act (DMCA)

* The DMCA is a United States Copyright law that implements two 1996 treaties of the world intellectual property organization (WIPO).
* It defines the legal prohibitions against the circumvention of technological protection measures employed by Copyright owners to protect their works, and against the removal or alteration of copyright management information.
* [https://www.copyright.gov](https://www.copyright.gov)

### Federal Information Security Management Act (FISMA)

* Provides a comprehensive framework for ensuring the effectiveness of information security controls over information resources that support federal operations and assets.
* It includes:
  * Standards for categorizing information and information systems by mission impact.
  * Standards for a minimum security requirements for information and information systems.
  * Guidance for selecting appropriate security controls for information systems.
  * Guidance for assessing security controls in information systems and determining security control effectiveness.
  * Guidance for security authorization of information systems.
  * [https://csrc.nist.gov](https://csrc.nist.gov)

## Module Summary

* This module discussed elements of information security, information security attacks and information warfare.
* It discussed cyber kill cahin methodology, TTPs and IoCs in detail.
* It also discussed hacking concepts, types and phases.
* Covered ethical hacking concpets such as the scope and limitations of ethical hacking, skills and other pertinent information in detail.
* Information security controls such as defense-in-depth, risk managment, cyberthreat intelligence, threat modelling, incident management process and AI and ML.
* Detailed discussion of various information security acts and laws from around the world.

The next module will go into detail about how attackers (as well I ethical hackers and pentesters) perform footprinting to collect information about the target of an evaluation before an attack or audit.

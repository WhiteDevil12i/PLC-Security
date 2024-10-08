# Detection-of-Security-Exploitation-in-Programmable-Logic-Controllers

## Abstract
In an increasingly interconnected industrial landscape, the security of Programmable Logic Controllers (PLCs) is of paramount importance. This project addresses the vulnerability of PLCs, specifically focusing on the potential unauthorized modification of program parameters. To demonstrate the concept, we employed RSLogix Micro Starter Lite to program a PLC and created a Timer (TON) component in the control circuit. To enhance the security of PLCs, we developed a script capable of detecting changes in the timer values. When unauthorized modifications are detected, the script triggers an alert mechanism that sends an email notification to the administrator. This system acts as an intrusion detection and prevention mechanism, safeguarding the integrity of the PLC program. The project underscores the significance of proactively monitoring and securing PLCs, as they play a pivotal role in various industrial applications. By implementing such security measures, industries can fortify their critical infrastructure against potential
threats, ensuring the reliable and uninterrupted operation of automated systems.

## Introduction
ExploitV2 is meticulously engineered to spotlight vulnerabilities within SCADA systems
by enabling controlled manipulation of running projects. It functions as an indispensable
tool for identifying weak points, allowing operators to bolster the system’s security
proactively. On the other hand, PLCPrevent acts as a robust countermeasure, actively
detecting and preventing any unauthorized changes made to the SCADA system. It ensures
the system’s integrity and reliability, minimizing potential risks. Furthermore, it
instantly notifies relevant authorities through email alerts, ensuring a swift response to
any potential threats. The project report chronicles our comprehensive research and development
endeavors in the realm of SCADA (Supervisory Control and Data Acquisition)
system security, with a specific focus on RSLOGIX Micro Starter. Our primary objective
is to enhance the security of these critical systems. We’ve achieved this through the
creation of two pivotal Python scripts, ExploitV2 and PLCPrevent. In this report, we
will delve into the motivation behind our project, highlight our significant contributions
to the field, define the problems we aimed to address, and outline the report’s overall
structure, providing a comprehensive understanding of our efforts in SCADA system security
enhancement. The primary contributions include the development of ExploitV2,
a Python script that exposes vulnerabilities in RSLOGIX Micro Starter, and PLCPrevent,
a script designed to detect and prevent unauthorized changes in running SCADA
projects. These scripts collectively enhance the security of SCADA systems and provide
an effective means to mitigate the risks associated with IoT hacking in such environments.
To address these vulnerabilities and enhance the security of PLCs, we designed a script
capable of detecting changes in the timer values. When unauthorized alterations were
detected, the script efficiently triggered an alert system, sending email notifications to
the designated administrator. This proactive approach serves as a robust intrusion detection
and prevention mechanism, providing an additional layer of protection to the PLC
infrastructure.


## Proposed Methodology
The objective of our project on PLC (Programmable Logic Controller) security was to develop
a methodology to detect and prevent unauthorized modifications to PLC programs,
specifically focusing on a Timer (TON) component created using RSLogix Micro Starter
Lite. In this proposed methodology, we outline the steps taken to achieve this goal:
1. System Configuration: - Begin by setting up the PLC using RSLogix Micro
Starter Lite, configuring the necessary hardware and software components. - Create a
functional Timer (TON) component within the PLC program as a representative case for
our security analysis.
2. Script Development: - Develop a script to periodically compare the current PLC
program parameters, specifically Timer values, with a predefined baseline or expected
values. - The script will utilize a suitable programming language, such as Python, to
access the PLC program and extract relevant data.
3. Baseline Establishment: - Create a baseline dataset of authorized PLC program
parameters and Timer values. These values represent the expected, authorized state of
the system. - Store this baseline securely to ensure its integrity.
4. Change Detection: - If the script detects any discrepancies between the current
Timer values and the baseline values, it should trigger an alert mechanism. - This mechanism
could be designed to generate an alert message and send it to the administrator
via email.
5. Alert Configuration: - Configure the email alert system, specifying the recipient(
s), the content of the alert message, and the circumstances under which an alert
should be sent.
6. Testing and Validation: - Thoroughly test the entire system, including the script,
baseline, monitoring, and alert mechanisms, to ensure its accuracy and reliability. - Simulate
unauthorized changes to Timer values to validate the detection and alert processes.


## System Diagram
The system design and implementation of the following following flow diagram is as follows:
#### Step 1: PLC Programming: 
The project starts with programming the PLC using
RSLogix Micro Starter Lite to control a TON timer. The PLC executes the programmed
logic, including the timer.
#### Step 2: SCADA Interface: 
The SCADA interface serves as the gateway for authorized
users to interact with the PLC. It allows legitimate operators to change timer values as
needed.
#### Step 3: ExploitV2:
This Python script simulates a potential security breach. It
interacts with the SCADA interface to make unauthorized changes to the timer values.
Its purpose is to expose vulnerabilities in the system.
#### Step 4: PLCPrevent:
This script is the core of the security system. It continually
monitors the PLC and the SCADA interface for any changes to the timer values. If it
detects unauthorized alterations, it triggers the email alert module.
#### Step 5: Email Alert Module:
When PLCPrevent identifies unauthorized changes, it
immediately sends an email alert to the administrator. This alert includes information about the detected changes and the time of the event.
<img src="https://cdn.discordapp.com/attachments/1054801949146480694/1188189422873739294/system_flow_PLC.png?ex=65999ea1&is=658729a1&hm=7f1f8adce23d8f5bbe5eb54d160881d8012b60daabdab32ffac3adda24535cf9&">

## Implementation and Result
The programming of a PLC using RSLogix Micro Starter Lite, created a TON (Timer
On-Delay) component in the circuit, and implemented a script to detect and prevent
unauthorized changes to the timer values. Here are the results and analysis of our project:
1. Unauthorized Timer Value Changes:
• The script successfully detected any unauthorized changes made to the timer values
in the PLC.
• When an intruder attempted to modify the timer settings, the detection mechanism
immediately recognized the alteration.
2. Alert Mechanism:
• Once unauthorized changes were detected, the script initiated an alert mechanism.
• The system reliably sent alert emails to the designated administrator or security
personnel.
3. Analysis of Vulnerability:
• The project effectively demonstrated the potential vulnerability of PLC systems to
unauthorized modifications.
• It highlights the importance of safeguarding PLCs, as any unauthorized changes can
impact industrial processes, leading to production downtime, errors, or even safety
hazards.
4. Prevention of Unauthorized Access:
• While the project focused on detection and alerting, it’s important to consider how
to prevent unauthorized access in the first place.
• Future enhancements could include implementing role-based access control, strong
authentication mechanisms, and network segmentation to limit access to critical
PLC components.
6. Ongoing Monitoring and Adaptation:
• Security is an ongoing process, and our project highlighted the need for continuous
monitoring and adaptation to emerging threats.
• Regularly updating our security mechanisms and staying informed about new vulnerabilities
and exploits is essential.

## Conclusion
In today’s industrial landscape, the security of Programmable Logic Controllers (PLCs) is
a matter of critical importance. Our project on PLC security and vulnerability detection
has shed light on the potential risks associated with unauthorized modifications to PLC
programs. By programming a PLC using RSLogix Micro Starter Lite and implementing
a Timer (TON) component, we demonstrated the ease with which vulnerabilities can be
exploited.
To address these vulnerabilities and enhance the security of PLCs, we designed a
script capable of detecting changes in the timer values. When unauthorized alterations
were detected, the script efficiently triggered an alert system, sending email notifications
to the designated administrator. This proactive approach serves as a robust intrusion
detection and prevention mechanism, providing an additional layer of protection to the
PLC infrastructure.

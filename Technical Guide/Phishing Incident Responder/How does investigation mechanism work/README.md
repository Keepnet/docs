# How does investigation mechanism work?

<p align="center">
  <img src="https://www.keepnetlabs.com/wp-content/uploads/Ekran-G%C3%B6r%C3%BCnt%C3%BCs%C3%BC-2018-08-02-18-54-54.png"><br>
  Keepnet Labs Incident Responder
</p>

Keepnet Phishing reporter add-in takes suspicious email in 3 different ways:

A user reports a suspicious email with a single click using phishing reported add-in installed in Outlook and sends it to the analysis. Then according to the results, an incident response operation is started.

A SOC team member initiates a manual investigation and triggers an incident response operation. To do so, by using the interface of Keepnet Incident responder, the SOC team member investigates a suspicious email in the inbox of all users,  and deletes the emails that he believes to be malicious or sends a warning message to all users.

It carries out an investigation and response according to the data coming from the Indicator of compromise (IOC ). For example, feeds taken from popular phishing websites like phishthank, openphish and IBM Xforce, it triggers an automatic investigation and prevents the dangerous phishing attacks.

## How does analysis mechanism work?

With its existing analysis engines as well as its integrated 3rd party analysis services, Keepnet addresses an email component in three ways and performs detailed analysis according to the following steps:

	* Header

	1. Spam control with integrated antispam services
	2. Anomaly detection: It identifies evasion techniques1 performed to circumvent security measures and also blocks the emails outside of the RFC2 rules and standards.
	3. Typosquatting: It identifies the fake sender and prevents the user from fraud

	* Body

	1. URL reputation control
	2. Malicious content detection
	3. The detection of the suspicious content with the artificial intelligence.
	4. Domain Squatting

	* Attachment

	1. Known malware control with Antivirus services
	2. Detection of unknown malware with Anti Malware Sandbox technology
	3. Detection 0-day file format exploits with Anti Exploit technology

## The current technologies used for analysis

<table>
  <tbody>
    <tr>
      <th>Technology</th>
      <th align="center">Description</th>
    </tr>
    <tr>
      <td align="left">URL Reputation</td>
      <td align="left">It checks through multiple blacklist engines and online reputation tools to facilitate the detection of fraudulent and malicious websites. This integration helps you identify sites involved in malware incidents, fraudulent activities and phishing websites.</td>
    </tr>
        <tr>
      <td align="left">Sandbox</td>
      <td align="left">Sandboxing offers another way for antimalware software to detect malware. A sandbox is an isolated computing environment developed to run unknown applications and prevent them from affecting the underlying system. Antimalware programs that use sandboxing run suspicious or previously unknown programs in a sandbox and monitor the results. If the malware demonstrates malicious behaviour, the antimalware will terminate it.


      </td>
    </tr>
        <tr>
      <td align="left">File Reputation</td>
      <td align="left">It protects against zero-day and targeted file-based threats by:<br>
<li>Obtaining the reputation of known files.</li>

<li>Analyzing the behaviour of specific files that are not yet known to the reputation service.</li>

<li>Continuously evaluating emerging threats as new information becomes available</li></td>
    </tr>
    <tr>
      <td align="left">Antivirus Engines</td>
      <td align="left">It is a software module that is purpose-built to find and remove malicious code.</td>
    </tr>
        <tr>
      <td align="left">Investigative Engines</td>
      <td align="left">The services that allow you to do an in-depth incident investigation.</td>
    </tr>
        <tr>
      <td align="left">Forensic Engines</td>
      <td align="left">It includes various forensics methods regarding in-depth forensic analysis.</td>
    </tr>
        <tr>
      <td align="left">DNS Firewall</td>
      <td align="left">DNS Firewall works by employing DNS Response Policy Zones (RPZs) and actionable threat intelligence to prevent data exfiltration.</td>
    </tr>
  </tbody>
</table>

![](https://www.keepnetlabs.com/wp-content/uploads/Incident-Investigation-Workflow.png)
***Incident Investigation Workflow***

According to the investigation results, a response is performed in two ways:

1. **User Inbox Level:** It investigates the incident in the user’s inbox and takes action;
	
	* Delete email from Inbox
	* Send Warning to User

2. **Generate Attack Signatures:** To detect and prevent the malicious activities that are anticipated in your network, you should pass the necessary rules to Antispam, IPS, SIEM, DLP, Sandboxing etc. products. This issue, which requires severe expertise and consumes hours, is resolved in Keepnet’s interface with one click that it allows you to orchestrate your security solutions.

![](https://www.keepnetlabs.com/wp-content/uploads/Example-Scenarios-for-Active-Response-1024x429.png)
***Example Scenarios for Active Response***

To help you take precautions if the email you analyse is suspicious;

<table>
  <tbody>
    <tr>
      <th>Rule</th>
      <th align="center">Description</th>
    </tr>
    <tr>
      <td align="left">Snort Rule</td>
      <td align="left">Generate Snort rules that you can use this rules with the best-known IPS (intrusion prevention system) to block malicious activity.</td>
    </tr>
        <tr>
      <td align="left">Yara Rule</td>
      <td align="left">Yara is a tool designed to help malware researchers identify and classify malware samples. It’s been called the pattern-matching Swiss Army knife for security researchers (and everyone else). Many of cyber threat prevention tools or services compatible with Yara rules.
      </td>
    </tr>
  </tbody>
</table>

3. Call API: You can use APIs to integrate with various products.  For example, you can call the help desk, trigger the network access control and automatically take the risky user off the network.

	1. An advanced evasion technique (AET) is a type of network attack that combines several different known evasion methods to create a new procedure that’s delivered over several layers of the network simultaneously. The code in the AET itself is not necessarily malicious; the danger is that it provides the attacker with undetectable access to the network. For more details visit https://bit.ly/2J9O8uA
	2. An RFC is authored by engineers and computer scientists in the form of a memorandum describing methods, behaviours, research, or innovations applicable to the working of the Internet and Internet-connected systems. See in more detail https://bit.ly/2j85trk
	3. Typosquatting, also called URL hijacking, a sting site, or a fake URL, is a form of cybersquatting, and possibly brandjacking which relies on mistakes such as typos made by Internet users when inputting a website address into a web browser. More more information visit https://bit.ly/2D1rGfD
	4. With artificial intelligence, Keepnet determines the person whom the user corresponds, and according to their mail content, it stops the attack.
	5. Cybersquatting refers to illegal domain name registration or use. Cybersquatting can have a few different variations, but its primary purpose is to steal or misspell a domain name to profit from an increase in website visits, which otherwise would not be possible. Visit https://bit.ly/2HfrFXj for more information. 
# Installation

## Prerequisites

* Office 2010/2013/2016 (32-bit & 64-bit)
* .Net 3.5 or later version
* Installation rights user

## Local Installation

You can install the .msi package created in the Customisation section by double-clicking your mouse on the computer that meets the installation requirements.

After installation, it appears in the program manager as follows, you can find the installed version information here.

![](https://www.keepnetlabs.com/wp-content/uploads/Screen-of-the-add-in-installed-in-the-control-panel-1024x396.png)

***The screen of the add-in installed in the control panel***

## Centralised Installation

**Keepnet Labs Outlook add-in support 32 and 64-bit system which has unattended installation.**

The following methods can be used to set up with Group Policy over Active Directory. Depending on the version of the domain controller, the steps may differ. In this article, a description has been made on a DC with Windows 2012 R2 operating system.

To see the installation in Group policy visit https://youtu.be/_CHf8AkWB1E

Firstly, the executable file (.msi extension) must be shared. Below is the shared folder that contains this file.

![](https://www.keepnetlabs.com/wp-content/uploads/Sharing-authority-edit-screen-1024x772.png)

***Sharing authority edit screen***

The installation of the folder attachment containing the relevant file is shared with the desired group. In this example, the folder is shared with Everyone. It is recommended that this file is shared only with the ‘Read’ authority so that it will not cause any security weaknesses (such as escalation).

![](https://www.keepnetlabs.com/wp-content/uploads/Sharing-authorization-screen-1024x735.png)

***Sharing authorization screen***

Open the Server Manager, click on Tools on the right side of the screen, then open the Group Policy Management Console.

![](https://www.keepnetlabs.com/wp-content/uploads/Group-policy-manager-access-window-1024x355.png)

***Group policy manager access window***

Then create a Group Policy Object (GPO) on the domain.

![](https://www.keepnetlabs.com/wp-content/uploads/Group-policy-creation-screen-1024x717.png)

***Group policy creation screen***

Below is the Group Policy Object created with the name Keepnet Outlook Add-in.

![](https://www.keepnetlabs.com/wp-content/uploads/GPO-name-identification-1024x721.png)


***GPO name identification***

Then the group policy is edited and the corresponding executable file is added as a new package. Below is the display of this file being added to the policy.

![](https://www.keepnetlabs.com/wp-content/uploads/Screen-where-MSI-package-is-selected-1024x611.png)

***The screen where MSI package is selected***

Then you are asked how you want to distribute this file. The ‘Assigned’ option is selected. With this option, a computer in the domain will apply this policy to its first startup and will install the Keepnet Labs Outlook add-in.

![](https://www.keepnetlabs.com/wp-content/uploads/Deployment-Method-1024x503.png)

***Deployment Method***

Then the new policy is applied to the systems with the ‘gpupdate’ command. If this policy is applied, computers may need to be restarted. In this case, restarted computers will have  Keepnet Labs Outlook add-in installed.


![](https://www.keepnetlabs.com/wp-content/uploads/Screen-Shot-2018-06-02-at-18.14.32-1024x281.png)

***Implementation of the Gpupdate / force command***

The following plug-in has been installed in the Outlook application. With the help of this add-in, employees can report a suspicious email and send it for analysis.

![](https://www.keepnetlabs.com/wp-content/uploads/A-thank-you-message-appears-when-a-user-reports-a-suspicious-email-1024x548.png)

***A thank you message appears when a user reports a suspicious email***
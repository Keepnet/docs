# Adding a New Template

Template components are made up from email samples with .eml extension. In order to turn an email into a template, you should save it as .eml file format.

An example of creating a template is demonstrated below.

![Original email](https://www.keepnetlabs.com/wp-content/uploads/Original-email-1024x724.png)

<p align="center">
  <img src="https://www.keepnetlabs.com/wp-content/uploads/image8.png"><br>
  File with email.eml file extension content
</p>

As you can see, the email with eml. file extension can be used as the fake web page. Also, a fake page can be created upon request.

With your browser’s “view source” feature, you can access to the HTML code, and save it an as.html extension.

![Original webpage](https://www.keepnetlabs.com/wp-content/uploads/Original-webpage-1024x522.png)

<p align="center">
  <img src="https://www.keepnetlabs.com/wp-content/uploads/Source-code-of-the-original-file.png"><br>
  The source code of the original file
</p>

To get the information from fake page for phishing, open the  .html file via a text editor, and arrange it by typing to the input areas captured=”email”, captured = “password” (the content can be arranged based on template or desired information), and by writing  the captured button parameters to button part.

![Edits made in HTML file](https://www.keepnetlabs.com/wp-content/uploads/Edits-made-in-HTML-file-1024x668.jpg)

To create a new template,  Phishing Scenarios > New Template tab must be accessed by using the .eml and .html files created.

***Creating a new template***

![New Template](https://www.keepnetlabs.com/wp-content/uploads/New-Template.png)

![Template creation page](https://www.keepnetlabs.com/wp-content/uploads/Ekran-G%C3%B6r%C3%BCnt%C3%BCs%C3%BC-2018-07-20-16-18-56-1024x318.png)

The name of the template to be created is specified in this step. With Template Files step, click the Choose File button to add .eml file. Then, you can customise your phishing email as you desire. You can edit the visuals, sender information etc.

![Template Editing Page](https://www.keepnetlabs.com/wp-content/uploads/Template-Editing-Page-1024x505.png)

You can edit the links, name, mailing details in the e-mail content, and assign a Phishing URL by clicking on{PHISHING_URL}the link above box.

![Generating a phishing URL](https://www.keepnetlabs.com/wp-content/uploads/Ekran-G%C3%B6r%C3%BCnt%C3%BCs%C3%BC-2018-07-20-16-58-46-e1532095432776-1024x256.png)

If you click on {PHISHING_URL} the box like the picture above, you will see an empty phishing URL on the email content. When you right-click on the link you will see the edit the link or unlink options. 

![Editing the phishing URL](https://www.keepnetlabs.com/wp-content/uploads/Ekran-G%C3%B6r%C3%BCnt%C3%BCs%C3%BC-2018-07-20-17-06-13-e1532095883256-1024x430.png)

![Defining a phishing URL](https://www.keepnetlabs.com/wp-content/uploads/PHISHING_URL--1024x657.png)

After this editing, whatever the Phishing URL is to be defined in the Campaign Manager, the fake web page will be opened on that same URL.

Shortcuts contain abbreviations such as name, surname, and target e-mails. {TONAME} shortcut automatically adds the target users’ e-mails to each sent e-mail content. It is the same with {TO} parameter. Thus, whatever email, name and surname information is identified in Email Groups, it will appear in the phishing email you have created. 
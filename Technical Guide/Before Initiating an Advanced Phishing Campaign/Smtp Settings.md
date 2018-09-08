# SMTP Settings
You can define the email server that the phishing campaign will be sent. 

Visit Company > SMTP Setting List > New SMTP page and define the email servers to be used.

![SMTP Settings](https://www.keepnetlabs.com/wp-content/uploads/SMTP-Setting-1024x849.png)


<table>
  <tbody>
    <tr>
      <th>Settings</th>
      <th align="center">Description</th>
    </tr>
    <tr>
      <td align="left">SMTP Name</td>
      <td align="left">This is the name that will be listed in SMTP list page as a reminder name.</td>
    </tr>
        <tr>
      <td align="left">SMTP Type</td>
      <td align="left">This is the type of the SMTP. When using the corporate server, it may remain default. It can bring the settings of Gmail, Outlook etc. services predefined for convenience.</td>
    </tr>
        <tr>
      <td align="left">SMTP Server Address</td>
      <td align="left">SMTP server’s DNS name or IP address and port number.</td>
    </tr>
    <tr>
      <td align="left">Authenticatione</td>
      <td align="left">The field where the requested username and password values are defined. If your SMTP server requires authentication, you should mark the Authentication box.</td>
    </tr>
        <tr>
      <td align="left">Use SSL</td>
      <td align="left">If email service supports or necessitates SSL connection, you can use this option.</td>
    </tr>
        <tr>
      <td align="left">Reply To</td>
      <td align="left">It is the e-mail address for responses to return, except sender e-mail address.</td>
    </tr>
        <tr>
      <td align="left">Error To</td>
      <td align="left">The e-mail address errors will be delivered.</td>
    </tr>
        <tr>
      <td align="left">CC</td>
      <td align="left">E-mail address to keep in CC in the sent e-mails.</td>
    </tr>
        <tr>
      <td align="left">BCC</td>
      <td align="left">Blind carbon copy to tertiary recipients who receive the message. The primary and secondary recipients cannot see the tertiary recipients.</td>
    </tr>
        <tr>
      <td align="left">X-Mailler</td>
      <td align="left">The value to be selected as the sender e-mail.</td>
    </tr>
        <tr>
      <td align="left">Custom Header</td>
      <td align="left">Custom header option is there to add additional options to the sent e-mail header information.  Sometimes, security checks are needed.</td>
    </tr>
  </tbody>
</table>

Table 1. SMTP Settings and Descriptions

Important Note: During simulation activities, since sender domain names would be different, it is important for SMTP servers to authorise sending e-mail from different domains.  In this case, we suggest adding to the list relay-host of Keepnet’s IP address’ SMTP server.
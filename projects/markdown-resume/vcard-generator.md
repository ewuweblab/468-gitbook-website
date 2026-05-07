# vCard Generator

{% embed url="https://potpourri-mini-sites.pmanikoth.workers.dev/tools/vcard" %}

### Overview

* Headless content with a GUI
* Small portable and digestible content

### Application

While newer technologies like JSON Contact standard are emerging, vCard remains the de facto standard for contact information interchange across different platforms and devices.

vCard (Virtual Contact File, .vcf) is a (headless) microformat. vCard is still widely used today, particularly for:

1. Contact Exchange

* Default format for exporting/importing contacts on iOS and Android devices
* Standard contact format in email clients like Outlook, Gmail, Apple Mail
* Business card QR codes that create instant mobile contacts

2. Address Book Systems

* Microsoft Exchange/Office 365

3. Current Version Status

* vCard 4.0 is the latest standard (RFC 6350)

Example of a basic vCard format:

```
BEGIN:VCARD
VERSION:3.0
N:Doe;John;;;
FN:John Doe
ORG:Example Corp.
TITLE:Software Engineer
TEL;TYPE=WORK,VOICE:(555) 555-1234
EMAIL;TYPE=PREF,INTERNET:john.doe@example.com
END:VCARD
```

### Generator

{% embed url="https://potpourri-mini-sites.pmanikoth.workers.dev/tools/vcard" %}

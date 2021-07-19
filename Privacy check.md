# Privacy

Please, read [[Why privacy matter]] first.

# Company access check

Let's do a quick check about how companies care about our privacy. 

[[Clover]] says in their [FAQ](https://cloverapp.co/faqs):
> Clover uses Google Firebase to store all user data which is encrypted both at rest and in transit using HTTPS. For more information on how we store and secure your data please refer to the [Google Firebase Privacy and Security](https://firebase.google.com/support/privacy) page.

That means - your data is secured from your provider (by HTTPS) and from random Google Employee (by Firebase). Not from Clover employee. Not from anyone who can access the Clover app server or Firebase key. 

[[Craft]] has [data pollicy](https://www.craft.do/s/0L6qZ2ew0yQS1P)

Here is part of this document:

> You data is stored in the cloud (AWS), it's encrypted during transfer (TLS) and also at rest (default RDS encryption for document content and personal data, and SSE-S3 encryption for uploaded binary content). However at this point we do not provide end-to-end encryption of your data.

That means data is closed from your provider (by TLS) and from random AWS employees (by RDS encryption). It is not sealed from anyone who has access to RDS and KMS key. Not closed from Craft employees and anyone who can access their servers. 
The only exception is for data you stored locally ([[Craft]] allows you to keep data locally; enormous thanks for this option!)

[[HyperNotes]] has [security practices](https://zenkit.com/en/security-practices/) document

TLDR: HTTPS for securing data from your provider and encryption at AWS, same as Craft, but they are GDPR compliant, so it's a little better. 

[[Mem]] didn't have any information about encryption. In their [privacy policy](https://get.mem.ai/privacy-policy), they said

>We have implemented appropriate technical and organizational security measures designed to protect the security of any personal information we process. However, despite our safeguards and efforts to secure your information, no electronic transmission over the Internet or information storage technology can be guaranteed to be 100% secure, so we cannot promise or guarantee that hackers, cybercriminals, or other unauthorized third parties will not be able to defeat our security, and improperly collect, access, steal, or modify your information. Although we will do our best to protect your personal information, transmission of personal information to and from our Services is at your own risk. You should only access the Services within a secure environment.

[[Notion]] - has a [great document](https://www.notion.so/Security-6c56b4854b624b0d8f36711018647f68) about security.

Notes still not end-to-end encrypted, but security standards are high compared to others (completed a SOC2 Type 1 report, in the process of completing a SOC2 Type 2 report, [GDPR] (https://www.notion.so/GDPR-at-Notion-8952f065d96f4c18abf22fc3c85e272e)) 

[[Roam]] has a section in [faq](https://roamresearch.com/#/app/help/page/QWRPpk5H-) about security - same HTTPS and Firebase as [[Clover]]: data is not secured from employees or anyone who may access their servers. 

[[SimpleNote]] has [this section](https://simplenote.com/help/#encryption) in faq about encryption

>Notes are not encrypted at rest due to server side constraints. For this reason we recommend not using Simplenote to store anything particularly sensitive.

[[Obsidian#Sync]] provides AES-GCM end-to-end encryption. It's pretty ok. Still, they didn't make any audit, and we can't be sure that it's true and they are actually doing that. After audit — Obsidian Sync may become the best solution in terms of privacy. 

## But what about CloudKit apps like [[Apple Notes]], [[Bear]] or [[NotePlan]]
[[CloudKit]] uses [end-to-end encryption](https://support.apple.com/en-mn/guide/security/sec3d52c0374/web) and Apple has great (among SaaS) security policy. Their infrastructure and policies was audited multiple times ( [ISO 27001](http://bit.ly/2zFFVse) and [27018](http://bit.ly/2zJMDvg) certifications), GDPR complient. 

Still, there is a chance that something goes wrong. For now, it's one of the best options in terms of privacy and security. 

## What about iCloud and Dropbox?
ok, this topic is vast. 
iCloud and Dropbox are worse than end-to-end encryption and CloudKit. Still, Apple has an excellent security policy and was audited multiple times. 

Dropbox is ok too. At least they [certified](https://www.privacyshield.gov/participant?id=a2zt0000000GnCLAA0) under the EU-U.S. and Swiss-U.S. Privacy Shield Framework and GDPR compliant. 

# Private policy check

I'm not a lawyer. And for me, all services have a pretty straightforward and okay-ish privacy policy. 

You should read them before you start to use the application. 

If you independent lawyer and want to help the community by reading privacy policies and translating them to plain English — contact me! 

# In English, please!

SaaS companies provide you only a promise of privacy. They promise not to read your data. 
You can't check if they are reading data or not. 

As an exception, [[Notion]] tries to involve independent auditors to review their processes. That's appreciable. 

[[Obsidian#Sync]] defines end-to-end encryption, but without any audits

Try to use CloudKit apps or sync notes via iCloud/Dropbox. 
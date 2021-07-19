You are trying to create a massive database of notes. It's a significant amount of work. With thousands of hours spent, it may become a life work. 

I assume that you didn't want to lose it. 

And while companies come and go, your notes should be available even when laptops will be replaced for Smart Glasses or Direct Neural Connection.

!!! info inline end ""

[[Why data format and backups matter]]

If you have all your notes locally on your hard drive with regular backups to some encrypted cloud storage — you are fine. 

But with SaaS, things got complicated:

## Let's talk about SaaS

- SaaS may fail and shut down service
- SaaS may remove your account
- SaaS may be hacked
- SaaS may lose part of your data

## Fail and shutting down

Any company can die:

-   It can run out of money because their internal processes are not optimal, or they didn't have users or a new investment round. 
-   It can be bought by a big corporation, which may decide to shut it down (try to search for examples — it's a pretty typical scenario) 
-   It can pivot to another idea.

!!! warning "Why it's a problem?"

With SaaS, all your data is stored on remote servers. If SaaS closed, they would shut down their servers, and you will lose access to your data. 

If you are planning to grant a single copy of your notes to SaaS, you better be sure that they will be ok. 

Let's take a look at their statuses for Jul 2021:

- [[Clover]] — founded: 2020, beta, didn't support export, didn't have "about us" page, can't find information about financial status, Funding by YCombinator [link](https://www.ventureradar.com/organisation/Clover/b243e0a9-7148-4a09-9721-6ee7a26ef53c/)
- [[Craft]] — founded: 2019, release: Nov 2020, raised $8M in ****April 2021**** [link](https://www.ventureradar.com/organisation/Craft%20Docs/3db70f9e-6523-4e69-a46b-83a37ed8b319) — they take investment round only few month ago. 
- [[HyperNotes]] — part of [ZenKit](https://zenkit.com) which owned by [Axonic](https://www.ventureradar.com/organisation/Axonic%20Informationssysteme/f43a0502-a758-4a49-b48c-a00939acdfa2/) — can't find any information about long-term plans or revenue. 
- [[mem.ai]] — founded: 2014 (?), beta, raised $5.6M in **April 2021** [link](https://www.ventureradar.com/organisation/Mem/86447004-e106-41c0-8153-35fd9dbbfe22/)
- [[Notion]] - founded in 2012, release in 2016, venture founded, current evaluation over $2Billion. 
- [[Roam]] - founded in 2017, can't find any information about financial status [link](https://www.ventureradar.com/organisation/Roam%20Research/04d4a9f6-891d-496a-922e-ea74b9967813/)
- [[SimpleNote]] - Free and not core service of [Automattic](https://www.ventureradar.com/organisation/Automattic/0070cace-8bbf-464d-b57a-fafc5f762f30/). They didn't have a public business model for now. 

## CloudKit and iCloud or Dropbox

Some of the standalone apps ([[NotePlan]], [[Apple Notes]], [[Bear]], [[iA Writer]], [[Obsidian#Local]]) uses Apple infrastructure — CloudKit and iCloud. 

Right now, Apple is a well-doing company. A lot of apps in the App Store rely on CloudKit and iCloud. Apple can close it, or Apple can go bankrupt. But I'm not sure that happens in the next few years. 

!!! warning

	We can't predict the future.

**Highlight:** I appreciate how [[NotePlan]] deals with it — it supports CloudKit (as one of the storage options) but stores everything as plain markdown files, taking the best value from both worlds. 

## In English, please!
The most reliable SaaS is [[Notion]] — they have users and make money. I'm pretty sure they remain open in the next few years. 

[[Craft]] and [[Mem]] raised their first money in April 2021. It's a lottery now. I wish them success, but now their future it's not clear. It would be best if you will do regular backups.

[[Clover]] is in beta and YCombinator, so it's an even earlier stage compared to [[Craft]] and [[Mem]]

[[SimpleNote]] and [[HyperNotes]] are part of bigger corporation. SimpleNote is free (that means losing money), and [[HyperNotes]] doesn't look like a core product for ZenKit (probably, I don't know, if you have more details - contact me) — so many of them can be closed at any moment.

[[Roam]] is the only exception — I can't find information for raising money, so I assume they earn enough from subscription and their business model works. Still, that didn't mean that this model will works in the following years — while they still didn't have a mobile client, I'm not sure about their long-term future.

Apps that use CloudKit/iCloud relied on Apple infrastructure, so at least you will not lose your data while Apple exists. 

## Losing access to account

All SaaS companies try to tell you that your data is yours. That's not true.

!!! warning

	Any of the SaaS can remove or block your account without any consequences. That means you will lose access to your life-long notes. 

I'm not saying it will happen, but there is a chance of it. And you are not in control here.

Try to search how often people relied on SaaS and got their accounts removed or blocked. It even happens to me with Twitter — they blocked one of my accounts without the ability to restore it. And I'm an average consumer without any unusual activities. 

## Losing data in outages

SaaS can lose your data in an outage or by hacking. Try to search how often it happens in the past for different products.

It may not happen to your startup, but there is a chance of it. While you didn't have your data on your laptop and in your secured storage — it's a gamble. 

## But I can export or backup my data...

Yes, you can. Please read [[Essential features#Data format and backups]]

## Conclusion

**My recommendation:** use SaaS only if it allows scheduled backups. In all other cases - use standalone apps which rely on iCloud, Dropbox, or CloudKit.
---
title: "DAIR Prepare, Part 4: Training"
date: 2026-11-02 09:00:00 +0100
categories: [Incident Response, DAIR]
tags: [dfir, incident-response, dair, preparation, training, certifications, conferences, bug-bounty]
description: "Before detecting anything, we need to know our job. How to find your way in a vast field, then where to train in Security Operations: learning platforms, certifications, conferences and bug bounty."
---

The first three parts of Prepare covered [the analyst's toolkit](/posts/dair-prepare-the-analyst-toolkit/), [logs and visibility](/posts/dair-prepare-logs-and-visibility/) and [shared infrastructure](/posts/dair-prepare-shared-infrastructure/). Before moving on to the **Detect** step, there's one more prerequisite: knowing our job.

But cybersecurity is a vast field, made of many different jobs, and nobody masters all of them. Two resources help to find your way:

- **[Paul Jerimy's Security Certification Roadmap](https://pauljerimy.com/security-certification-roadmap/)**: nearly 500 certifications mapped by domain (network, identity, architecture, GRC, forensics, penetration testing…) and by level (last updated in 2024). It also gives a good overview of the jobs behind them.
- **[SANS: courses by frameworks and directives](https://www.sans.org/frameworks-and-directives)**: training mapped to skills frameworks, including the US NICE Framework and the **European Cybersecurity Skills Framework (ECSF)** from ENISA, which describes the main cybersecurity roles.

In this blog and this post, I'll focus on my own area of expertise, often grouped under **Security Operations**, which covers both the **defensive** and the **offensive** side.

---

## 1. Train first: the learning platforms

Before talking about pieces of paper and certifications, there's a simpler step: training. Learning platforms let you practise on realistic labs, at your own pace, without the pressure of having to pass an exam.

### To get started: TryHackMe

**[TryHackMe](https://tryhackme.com/)** is often the first step: guided paths, browser-based labs, and content that covers both the offensive and the defensive side. Recently, they've been investing heavily to regain ground on the other platforms. I haven't tested their more advanced content yet, so I can't give an opinion on it, but for getting started it remains an easy entry point.

### Offensive side

Two platforms stand out to learn:

- **[Hack The Box](https://www.hackthebox.com/)**: the **[HTB Academy](https://academy.hackthebox.com/)** for structured modules, then the **Labs** and their machines (*boxes*) to put it into practice on realistic targets.
- **[PortSwigger Web Security Academy](https://portswigger.net/web-security)**: the reference for web application security, built by the makers of Burp Suite. Each topic (SQL injection, XSS, SSRF, access control…) comes with explanations and hands-on labs, and it's entirely free.

### Defensive side

For me, the best resources are:

- **[LetsDefend](https://letsdefend.io/)**: a SOC analyst environment, with alerts to triage in a simulated SIEM, investigations and training paths.
- **[Blue Team Labs Online](https://blueteamlabs.online/)**: investigation challenges from Security Blue Team, on real artefacts: logs, PCAPs, memory, disk images.

---

## 2. Certifications

From my point of view, when you start, you need knowledge on **both** the defensive and the offensive side. Whichever side you end up on, what you've learned from the opposite one will be an integral part of your work: a defender who understands how attackers operate investigates better, and an attacker who understands detection works more effectively.

The paths I'd suggest:

| Side | Path |
|---|---|
| Offensive | [PJPT](https://certifications.tcm-sec.com/pjpt/) (TCM Security) → [HTB CPTS](https://academy.hackthebox.com/preview/certifications/htb-certified-penetration-testing-specialist) → [HTB CWEE](https://academy.hackthebox.com/preview/certifications/htb-certified-web-exploitation-expert) → [CRTO](https://www.zeropointsecurity.co.uk/courses) (Zero-Point Security) |
| Defensive | [HTB CDSA](https://academy.hackthebox.com/preview/certifications/htb-certified-defensive-security-analyst) → [CCDL2](https://cyberdefenders.org/blue-team-training/courses/certified-cyberdefender-level-2/) (CyberDefenders, formerly CCD) |

With that solid foundation, you'll have all the tools to start a good career.

When budget isn't an issue, **[OffSec](https://www.offsec.com/)** and **[SANS](https://www.sans.org/)/[GIAC](https://www.giac.org/)** provide high-quality courses and exams, but they're quite expensive.

I strongly recommend SANS if you have access to a [scholarship](https://www.sans.org/scholarship-academies/) or if your employer can cover the costs: it will open a lot of doors. There's also **[SANS.edu](https://www.sans.edu/)**, the SANS Technology Institute, which awards degrees and certificates built on SANS courses, with GIAC certifications included, often at an advantageous price.

> **Learn to walk before you run.** Cybersecurity is trendy, but a solid foundation in **system and network administration** is essential to progress. You can't defend or attack a network, an Active Directory or a Linux server you don't understand. If you don't have that background, train extensively on the IT fundamentals first.
{: .prompt-warning }

Over time, you'll discover other certifications and other resources. That means you already have a foot in the field. This post is here to guide you and show you where to look: training is a big business, with a lot of players, and it's easy to get lost.

---

## 3. Conferences

Platforms and certifications are done alone, in front of a screen. Conferences are where you meet the community: talks on the latest techniques and investigations, hands-on workshops, CTFs, and above all people. Many opportunities, jobs and collaborations start with a conversation in a hallway.

A selection, from close to home to the other side of the world:

| Country | Conference | In short |
|---|---|---|
| Belgium | **[BruCON](https://www.brucon.org/)** (Ghent) | The Belgian security conference: talks, workshops and trainings |
| France | **[InCyber Forum](https://europe.forum-incyber.com/)** (Lille, formerly FIC) | One of the largest events in Europe, with a strong policy and industry side |
| France | **[leHACK](https://lehack.org/)** (Paris) | A non-profit hacking conference: offensive security, hardware, OSINT |
| Luxembourg | **[Hack.lu](https://www.hack.lu/)** | A long-running technical conference, organised by CIRCL, the team behind MISP |
| Monaco | **[Les Assises](https://www.lesassisesdelacybersecurite.com/)** | A meeting place for security decision-makers and experts, mostly French-speaking |
| Poland | **[x33fcon](https://www.x33fcon.com/)** (Gdynia) | Built around collaboration between red and blue teams: purple teaming |
| United Arab Emirates | **[GISEC Global](https://www.gisec.ae/)** (Dubai) | The large regional event, with over 25,000 expected attendees |
| United States | **[Black Hat](https://www.blackhat.com/)** and **[DEF CON](https://defcon.org/)** (Las Vegas) | The summer week in Las Vegas: research and briefings at Black Hat, the community and its villages at DEF CON |
| United States | **[RSAC Conference](https://www.rsaconference.com/)** (San Francisco) | One of the largest industry conferences, very vendor and leadership oriented |

And the **[SANS Summits](https://www.sans.org/cyber-security-summit/)**, held all over the world on specific topics (DFIR, threat hunting, CTI, cloud…). Many of them can also be followed online, often for free.

The **[BSides](https://bsides.org/)** are community-run conferences, free or cheap, organised in many cities around the world. A good first conference, and often the easiest place to give your first talk.

Many conferences also host a **CTF**, and [CTFtime](https://ctftime.org/) lists the online ones all year round. Playing as a team builds the same reflexes as an incident: splitting the work, sharing findings, keeping notes.

> Many conferences publish their talks online afterwards. Even when you can't attend, the recordings are a free and up-to-date source of training.
{: .prompt-tip }

---

## 4. Bug bounty

When you have enough experience and want to practise web security on real targets, bug bounty is an easy way in. Companies open part of their systems to researchers, with clear rules, and reward the vulnerabilities reported. A few platforms:

- **[Intigriti](https://www.intigriti.com/)**: a Belgian platform, with many European programmes.
- **[YesWeHack](https://www.yeswehack.com/)**: a French platform, also strongly present in Europe.
- **[HackerOne](https://www.hackerone.com/)** and **[Bugcrowd](https://www.bugcrowd.com/)**: the two large US platforms.

> **Check your legal situation first.** Before taking part, make sure you understand the law and the rules of your country, as well as the scope and rules of each programme: testing outside the scope is not covered. In Belgium, for example, a [legal framework](https://www.intigriti.com/blog/news/new-belgian-legal-framework-gives-safe-harbor-to-ethical-hackers-and-bug-bounty-hunters) has protected ethical hackers since February 2023, but only under strict conditions, including reporting to the Centre for Cybersecurity Belgium (CCB).
{: .prompt-warning }

---

Whatever path you choose, training never stops: techniques, tools and attackers keep changing. Start with the fundamentals, practise without pressure, get certified when it makes sense, and go meet the community. And remember that every incident you work on is also a lesson.

---

**Next:** the last part of Prepare, **playbooks and communication**: turning all this preparation into procedures the team can follow under pressure, and the exercises that test them.

### References

- [Paul Jerimy: Security Certification Roadmap](https://pauljerimy.com/security-certification-roadmap/)
- [SANS: courses by frameworks and directives](https://www.sans.org/frameworks-and-directives)
- [TryHackMe](https://tryhackme.com/)
- [Hack The Box](https://www.hackthebox.com/) · [HTB Academy](https://academy.hackthebox.com/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)
- [LetsDefend](https://letsdefend.io/)
- [Blue Team Labs Online](https://blueteamlabs.online/)
- [TCM Security: PJPT](https://certifications.tcm-sec.com/pjpt/)
- [HTB Academy certifications](https://help.hackthebox.com/en/articles/9561479-academy-certifications)
- [Zero-Point Security: CRTO](https://www.zeropointsecurity.co.uk/courses)
- [CyberDefenders: CCDL2](https://cyberdefenders.org/blue-team-training/courses/certified-cyberdefender-level-2/)
- [OffSec](https://www.offsec.com/) · [SANS](https://www.sans.org/) · [GIAC](https://www.giac.org/)
- [BruCON](https://www.brucon.org/) · [InCyber Forum](https://europe.forum-incyber.com/) · [leHACK](https://lehack.org/) · [Hack.lu](https://www.hack.lu/) · [Les Assises](https://www.lesassisesdelacybersecurite.com/) · [x33fcon](https://www.x33fcon.com/)
- [GISEC Global](https://www.gisec.ae/) · [Black Hat](https://www.blackhat.com/) · [DEF CON](https://defcon.org/) · [RSAC Conference](https://www.rsaconference.com/) · [SANS Summits](https://www.sans.org/cyber-security-summit/) · [BSides](https://bsides.org/) · [CTFtime](https://ctftime.org/)
- [Intigriti](https://www.intigriti.com/) · [YesWeHack](https://www.yeswehack.com/) · [HackerOne](https://www.hackerone.com/) · [Bugcrowd](https://www.bugcrowd.com/)
- [Intigriti: new Belgian legal framework for ethical hackers (2023)](https://www.intigriti.com/blog/news/new-belgian-legal-framework-gives-safe-harbor-to-ethical-hackers-and-bug-bounty-hunters)
- [SANS Cyber Academies (scholarships)](https://www.sans.org/scholarship-academies/) · [SANS.edu](https://www.sans.edu/)

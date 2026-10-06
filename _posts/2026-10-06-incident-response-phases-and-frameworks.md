---
title: "Incident Response Frameworks: Four Models, One Path for This Blog"
date: 2026-10-06 09:00:00 +0200
categories: [Incident Response, Fundamentals]
tags: [dfir, incident-response, dair, picerl, nist, iso27035]
description: "A high-level look at the four incident response models worth knowing (NIST SP 800-61r3, ISO/IEC 27035, PICERL and DAIR), and why this blog will follow DAIR, one step at a time."
pin: true
image:
  path: /assets/img/posts/ir-frameworks/dair-model.png
  alt: "The DAIR model: Prepare, Detect, Verify & Triage, the Response Actions Loop, and Debrief"
---

## Welcome to Cyber Horizon

This is the first post on this blog. Here I'll share hands-on write-ups from the field: incident response, malware analysis and threat hunting. Practical, technical, no marketing fluff.

Before getting into tools and artefacts, I want to set the frame. Every incident response team follows a model, explicitly or not. It defines the steps, the vocabulary, and how the team knows what to do next. Here are the four you'll come across, from a responder's point of view, and the one this blog will follow.

---

## 1. NIST SP 800-61r3: incident response as part of risk management

The reference in the US and in many international organisations. The previous version (2012) described a four-phase lifecycle that many teams still use: *Preparation; Detection & Analysis; Containment, Eradication & Recovery; Post-Incident Activity*.

The current revision, published in April 2025, changed approach: it maps incident response onto the six functions of the NIST Cybersecurity Framework 2.0 (*Govern, Identify, Protect, Detect, Respond, Recover*).

![NIST SP 800-61r3 incident response model based on the CSF 2.0 functions](/assets/img/posts/ir-frameworks/nist-800-61r3.svg){: w="900" h="470" }
_Preparation (Govern, Identify, Protect), incident response (Detect, Respond, Recover) and continuous improvement in between. Adapted from NIST SP 800-61r3, Fig. 2._

**In practice:** it ties incident response to the rest of the security programme and tells you what needs to be in place. NIST deliberately left the detailed procedures out, because they change too fast for a static document, so you won't find a case-handling playbook in it.

## 2. ISO/IEC 27035: the international standard

The ISO series dedicated to information security incident management, with parts covering principles and process (2023), planning and preparation (2023), response operations (2020) and coordination between organisations (2024). Its process runs through five phases: *plan and prepare, detect and report, assess and decide, respond, learn lessons*.

![The five phases of the ISO/IEC 27035-1 incident management process](/assets/img/posts/ir-frameworks/iso27035.svg){: w="760" h="620" }
_The ISO/IEC 27035-1:2023 incident management process._

**In practice:** the natural reference for ISO 27001-certified organisations. It describes a generic process that each organisation tailors, so responders usually feel it through their own procedures, escalation rules and reporting, rather than by reading the standard during a case.

## 3. PICERL: the classic responder's model

Six phases dating back to the 1990s, popularised by the SANS guide *Computer Security Incident Handling: Step by Step* (1998). It's still the most familiar vocabulary among responders:

![The six PICERL phases in sequence](/assets/img/posts/ir-frameworks/picerl.svg){: w="1100" h="260" }
_PICERL: six phases, one after the other._

**In practice:** simple, easy to remember, and everyone in the field speaks it. Its limit is that it reads as a straight line, while real incidents never are. You contain what you've found, then a new host or account turns up, and you're back to investigating.

## 4. DAIR: the dynamic approach

The **Dynamic Approach to Incident Response**, introduced by Joshua Wright in his book *Dynamic Incident Response* (September 2026), rethinks PICERL rather than throwing it away: the old phases aren't wrong, they just don't hold up as a straight line. It keeps the same goals but organises them around five waypoints, with the core of the response work happening in a loop, and coordination with decision-makers running through every step:

![The DAIR model](/assets/img/posts/ir-frameworks/dair-model.png){: w="1600" h="774" }
_The DAIR model. Figure from Joshua Wright, *Dynamic Incident Response*, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)._

**In practice:** it matches how incidents actually unfold. Verification and triage get their own step, scoping is no longer buried inside "identification", and going back round the loop when new evidence appears is expected rather than seen as a failure. The loop ends when no new evidence turns up and a named decision-maker signs off on the residual risk. The book is free under a Creative Commons (CC BY 4.0) licence: [dynamicincidentresponse.com](https://dynamicincidentresponse.com).

---

## At a glance

| DAIR | PICERL | ISO/IEC 27035 | NIST SP 800-61r3 |
|---|---|---|---|
| Prepare | Preparation | Plan and prepare | Govern, Identify, Protect |
| Detect | Identification | Detect and report | Detect |
| Verify & Triage | Identification | Assess and decide | Detect, Respond |
| Scope, Contain, Eradicate, Recover (loop) | Containment, Eradication, Recovery | Respond | Respond, Recover |
| Debrief | Lessons Learned | Learn lessons | Identify (improvement) |

Same work, different vocabulary. These models aren't competitors: NIST and ISO frame how an organisation governs incident response, while PICERL and DAIR describe how responders actually work a case. The DAIR book even maps its steps to the CSF 2.0 functions, so a team can work in DAIR and still report against NIST. Whatever model your organisation uses officially, what matters is that everyone on the team speaks the same one during an incident.

---

## The path for this blog: DAIR, one step at a time

This blog will follow **DAIR**. It's the model that best reflects what responders actually do, and its iterative loop is exactly where most of the hands-on work lives.

Each upcoming post will cover one step, from the responder's chair:

1. **Prepare**: the logs, tooling and access you need before the call comes in.
2. **Detect**: making sure the right signal reaches the right person, with enough context.
3. **Verify & Triage**: confirming the alert is real, assessing the initial risk, and deciding with the business whether to continue, stop or defer.
4. **Scope**: hunting indicators across the fleet and building the timeline.
5. **Contain**: stopping the attacker and collecting volatile evidence, without tipping them off.
6. **Eradicate**: finding the root cause, removing persistence and closing the door they came in through.
7. **Recover**: getting back to business without letting them back in.
8. **Debrief**: running a blameless after-action review and turning every blind spot into an improvement.

Each one with concrete artefacts, tools and field experience. Along the way, I'll also publish standalone write-ups on specific cases and techniques.

If you need help with an incident, or want to prepare before one happens, you can reach me through [cyberhorizon.be](https://cyberhorizon.be).

### References

- [Dynamic Incident Response (DAIR)](https://dynamicincidentresponse.com)
- [NIST SP 800-61 Rev. 3](https://csrc.nist.gov/pubs/sp/800/61/r3/final)
- [ISO/IEC 27035 series overview](https://www.iso27001security.com/html/27035.html)

---
layout: default
title: Academic Agency & Data Continuity
description: Best practices for graduate students and postdocs to protect their research. Covers backup strategies, email archiving, and preventing authorship disputes.
keywords: PhD advice, grad student protection, research continuity, authorship MOU, academic agency, postdoc rights
---

# **Academic Agency and Data Continuity**

**Best Practices for Graduate Researchers and Postdocs**

## **Introduction**

Research is a professional endeavor that generates valuable intellectual property. Whether you are a PhD candidate writing code or a Postdoctoral Fellow analyzing patient data, you are creating assets that require management. This guide outlines the core principles of protecting your work, ensuring its reproducibility, and maintaining professional clarity with your collaborators.

## **Principle 1: Digital Sovereignty (Redundancy)**

University infrastructure is temporary. Your access to servers, email, and cloud storage is contingent on your current enrollment status. To ensure the continuity of your research career, you must maintain a parallel infrastructure.

**The Rule of Three:**
Data should exist in three places:

1. **The Lab Environment:** The shared server or Box folder where collaboration happens.
2. **The Local Machine:** A copy on your physical workstation for offline access.
3. **The Personal Archive:** A private, off-site backup (personal hard drive or personal cloud account) that ensures you retain access to your intellectual property if institutional access is interrupted.

**CRITICAL WARNING: Restricted Data vs. Your IP**
You must distinguish between Restricted Source Data and Your Intellectual Property.

* **Do NOT Backup:** Raw human subjects data containing PII (Personally Identifiable Information), HIPAA data, or un-anonymized video/audio files. Moving these to a personal drive is often a violation of your IRB protocol and federal law. Check your IRB approval before moving any raw data off-site.
* **DO Backup:** Your code, your analysis scripts, your de-identified aggregate data, your lab notebooks, your manuscripts, and your literature reviews. These are the products of your labor and are generally safe to archive personally.

**Correspondence Archiving:**
Do not rely solely on your institutional email address (.edu) as your primary record of correspondence. University IT policies often prevent auto-forwarding, and accounts are frequently deactivated upon graduation. You should manually archive your mailbox once per semester to a local format (like .mbox or .pst) to preserve your professional history.

## **Principle 2: The Paper Trail (Communication)**

Ambiguity is the primary cause of authorship disputes. Most conflicts arise not from malice, but from differing recollections of verbal agreements. You must convert conversation into documentation.

**The Recap Email:**
Never rely on a verbal agreement regarding timelines, responsibilities, or authorship. Immediately following any supervisory meeting, send a brief summary email.

> **Subject:** Recap of meeting [Date]
>
> "Dear Professor,
>
> Just to recap our meeting: I will complete the analysis by Friday. We agreed that if this yields results, I will draft the methods section as first author."

*Function:* This creates a contemporaneous record. If the supervisor does not reply, their silence implies consent. If they dispute it, the misalignment is identified immediately rather than years later.

**The "Witness" Network:**

* **For Grad Students (The Committee):** Avoid isolating yourself with a single mentor. Your dissertation committee functions as a Board of Directors. Schedule brief updates with individual committee members once a semester to demonstrate your progress and show them your raw data.
* **For Postdocs (The IDP):** You lack a committee, which makes you vulnerable to isolation. You must formalize your **Individual Development Plan (IDP)**. Most federal grants (NIH/NSF) mandate these. Insist on a biannual IDP meeting and invite a secondary mentor or department chair to sit in on the "Career Goals" portion. This establishes a third-party witness to your productivity and forces the PI to articulate their timeline for your promotion or departure in front of a peer.

## **Principle 3: Attribution Metadata (Timestamping)**

You must be able to prove *what* you created and *when* you created it.

**Preregistration:**
For empirical work, register your hypotheses and analysis plans on public repositories before data collection begins. This establishes your priority on the intellectual concept and protects against "scooping."

**Authorship Memorandums (The CRediT System):**
At the start of any collaborative project, advocate for a simple Authorship Memorandum of Understanding (MOU). This document tentatively lists the author order and the specific roles assigned to each contributor.

To prevent ambiguity, utilize the **CRediT (Contributor Roles Taxonomy)**. Instead of vague promises of "help," assign specific ISO-standard roles to each person. It is much harder for a PI to ghost you if you have a signed document stating you are the sole lead on these specific categories:

* **Conceptualization**
* **Software**
* **Formal Analysis**
* **Data Curation**
* **Writing – Original Draft**

## **Implementation**

These principles require specific tools to implement effectively. Please refer to the specific protocol for your discipline:

* [**Protocol A: Computational Workflow**]({{ site.baseurl }}/protocol_computational/) (Code-heavy).
* [**Protocol B: Manuscript Workflow**]({{ site.baseurl }}/protocol_manuscript/) (Document-heavy).
+++
title = "eCPPTv3 Technical Guide"
date = 2024-11-22
description = "My experience with the eCPPT v3 certification: preparation, exam insights and honest considerations"
+++

<div class="has-toc">
<div class="ox-hugo-toc toc">
    <div class="heading">Table of Contents</div>
    <ul>
        <li><a href="#introduction"><strong>Introduction</strong></a></li>
        <li><a href="#personal-experience"><strong>Personal Experience</strong></a></li>
        <li><a href="#training-and-preparation"><strong>Training and Preparation</strong></a></li>
        <li><a href="#note-taking-strategy"><strong>Note-Taking Strategy</strong></a></li>
        <li><a href="#strengths"><strong>Strengths</strong></a></li>
        <li><a href="#drawbacks"><strong>Drawbacks</strong></a></li>
        <li><a href="#ecppt-v3-vs-v2"><strong>eCPPT v3 vs v2</strong></a></li>
        <li><a href="#useful-resources"><strong>Useful Resources</strong></a></li>
        <li><a href="#conclusion"><strong>Conclusion</strong></a></li>
    </ul>
</div>
</div>

I recently achieved the **eLearnSecurity Certified Professional Penetration Tester v3** certification and wanted to share my experience, offering an honest perspective on the pros and cons of this certification that has undergone significant changes compared to previous versions.
<br><br>

<div style="text-align: center;">
    <img src="/images/ecppt.png" alt="CPTS Certification" style="max-width: 700px;">
</div>

## Introduction {#introduction}

The **eCPPT v3** represents an important step in the certification path for penetration testers, positioning itself as a natural successor to the **eJPT**. However, version 3 has introduced substantial changes that deserve in-depth analysis.

The certification primarily focuses on:
- **Active Directory Enumeration & Attacks**
- **Network Penetration Testing**
- **Post-Exploitation**
- **Lateral Movement**
- **Credential Harvesting**

## Personal Experience {#personal-experience}

The exam has a duration of **24 hours** and I started it around **9:00 AM**, managing to complete it the same day at **11:30 PM** - approximately **14.5 hours** of actual work.

The exam was challenging but manageable. I took strategic breaks throughout the day to maintain focus and avoid burnout. The time investment was reasonable considering the scope of the assessment, though some phases required more patience than others, particularly during enumeration and credential validation.

I'm satisfied to have achieved this milestone in my cybersecurity journey, building upon the foundation established with my **eJPT** certification.

## Training and Preparation {#training-and-preparation}

### Materials Used

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**Official INE Course:**</a> I completed the official course, but I must be honest - **it's not sufficient**. The material is still based on v2 and appears outdated for current exam standards.

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**HackTheBox Academy:**</a> The most valuable resource was definitely the **"Active Directory Enumeration & Attacks"** module. This is fundamental and I recommend it as the absolute priority.

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**HackTheBox Labs:**</a> VIP subscription to practice on more realistic environments, especially **retired boxes** with Active Directory focus.

### Recommended Priority Order

1. <a style="color: #bc7afe; text-decoration: none; cursor: default;">**HackTheBox Academy**</a> - Active Directory Module (highest priority)
2. <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Official INE Course**</a> - Labs and basic theory
3. <a style="color: #bc7afe; text-decoration: none; cursor: default;">**HackTheBox Labs**</a> - Retired boxes for practice

**Note**: If budget is limited, focus everything on HTB Academy. It's the investment with the best ROI for this certification.

## Note-Taking Strategy {#note-taking-strategy}

**Effective note-taking** was crucial for my success. I used **CherryTree** with the following structure:

### Organization Structure

```
General Notes
   └── Subnet in scope
   └── Wordlists (seasons.txt, months.txt, xato, rockyou.txt)

Hosts Table
   └── Node Number | Name | Domain | IP Address

Credentials
   └── Account | Password | Domain User? | Notes

Node x [IP] [Machine_Name]
   ├── Nmap Scan
   ├── Important Notes
   └── Shares
```

### Note-Taking Tips

- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Rigorous organization:**</a> Don't underestimate the importance of keeping everything organized
- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Document everything:**</a> Every credential, every discovery, every useful command
- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Flexible structure:**</a> Adapt the structure to your needs, but keep it consistent

## Strengths {#strengths}

### Personal Growth
The eCPPT helped me **discover my real capabilities**, pushing me beyond my limits and testing dedication and motivation.

### Thorough Preparation
It forced me to explore additional resources like HTB Academy, particularly the **Active Directory** module which proved fundamental.

### Stable Lab Environment
Contrary to some reports of instability, the lab environment was **reliable**. The web-based Kali machine was fluid and responsive.

### Active Directory Focus
The emphasis on AD is current and relevant for the modern job market.

## Drawbacks {#drawbacks}

### Outdated Training Material
The **syllabus is still outdated** and many topics have been removed or modified without adequately updating the study material. This creates a significant gap between what you study and what you encounter in the exam, forcing candidates to rely heavily on external resources.

### Excessive Focus on Bruteforcing
<a style="color: #bc7afe; text-decoration: none; cursor: default;">**Time wasted on bruteforce**</a> - contrary to what INE claims ("if you spend more than 30 minutes bruteforcing you're doing something wrong"), many credentials required longer times. This approach feels more like a patience test than a skills assessment.

### Tool Limitations and Technical Issues
- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Not all tools are available**</a> in the exam machine
- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Evil-WinRM doesn't work**</a> despite multiple fix attempts
- Need to find workarounds for specific tools

The most frustrating aspect was discovering that critical tools don't function as expected in the exam environment. This forces you to adapt on the fly and find alternative methods, which while educational, can be time-consuming during a timed assessment.

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**The most serious problem:**</a> some exam questions **don't make sense**, requiring information about non-existent users in domains/hosts. Since they're not MCQ, you can't even try your luck. This issue alone consumed hours of my exam time as I questioned my methodology and attempted different approaches.

## eCPPT v3 vs v2 {#ecppt-v3-vs-v2}

The **v2 was superior** in many aspects, offering a more comprehensive learning experience. The removed topics include **Buffer/Stack Overflow**, **Pivoting & Double Pivoting**, and **Report Writing** - these were the aspects that excited me most, and their removal was a **major disappointment**.

These topics weren't just theoretical concepts; they represented core skills that any professional penetration tester should master. Buffer overflow exploitation teaches you to understand memory corruption at a fundamental level, while pivoting techniques are essential for complex network assessments. Report writing, perhaps most importantly, bridges the gap between technical findings and business impact.

The v3 has essentially transformed into a **specialized Active Directory certification**, losing the completeness that characterized previous versions. While AD skills are undeniably important in modern environments, the narrow focus limits the certification's value as a comprehensive penetration testing credential.

This shift feels like a step backward in terms of educational value. The original eCPPT was designed to produce well-rounded penetration testers capable of handling diverse scenarios. The current version, while still valuable for AD-focused roles, doesn't provide the same breadth of knowledge.

## Useful Resources {#useful-resources}

### Recommended Materials

1. **HackTheBox Academy - Active Directory** (essential)
2. **HackTheBox Labs** - Retired boxes
3. **IppSec YouTube Channel** - Detailed walkthroughs
4. **eJPT Course** - For penetration testing basics
5. **eCPPTv3 Review by ElnurBDa** - Additional perspectives

### Setup and Tools

- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**CherryTree**</a> for note-taking
- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Wordlists:**</a> seasons.txt, months.txt, xato, rockyou.txt
- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Evil-WinRM alternatives**</a> (prepare backups)

## Conclusion {#conclusion}

After completing the eCPPT v3, I find myself with mixed feelings about recommending this certification. While it certainly provided value in terms of Active Directory knowledge and hands-on experience, the significant issues I encountered cannot be ignored.

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**I currently discourage taking eCPPT v3**</a> until INE resolves the fundamental problems with exam questions, updates the training material to match v3 requirements, and ensures tool stability in the lab environment. The frustration of encountering nonsensical questions that waste valuable exam time is simply unacceptable for a paid certification.

If you're specifically looking to develop Active Directory skills, consider the <a style="color: #bc7afe; text-decoration: none; cursor: default;">**HackTheBox CPTS**</a> as a more modern and complete certification, or the specialized <a style="color: #bc7afe; text-decoration: none; cursor: default;">**HackTheBox CAPE**</a> for focused Active Directory expertise. Both options provide better value and more reliable assessment experiences.

For those determined to pursue eCPPT v3 despite these issues, ensure you have multiple backup plans for tool failures and be prepared for potentially confusing exam questions. Focus heavily on HackTheBox Academy's Active Directory module rather than relying solely on the official INE materials.

The certification landscape is evolving rapidly, and while eCPPT v3 may improve over time, there are currently better options available for developing practical penetration testing skills. <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Choose your certification path wisely**</a> - your time and money are valuable resources that deserve to be invested in quality learning experiences.

---

<br><br>
*by Andrea Gelmi*

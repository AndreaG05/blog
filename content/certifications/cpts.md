+++
title = " CPTS Technical Guide"
date = 2025-06-14
description = "A complete guide to the HTB CPTS certification based on personal experience and practical insights"
+++

<div class="has-toc">
<div class="ox-hugo-toc toc">
    <div class="heading">Table of Contents</div>
    <ul>
        <li><a href="#introduction"><strong>Introduction</strong></a></li>
        <li><a href="#cpts-vs-oscp"><strong>CPTS vs OSCP</strong></a>
            <ul>
                <li><a href="#cost">Cost</a></li>
                <li><a href="#material-quality">Material Quality</a></li>
                <li><a href="#validity-recognition">Validity/Recognition</a></li>
            </ul>
        </li>
        <li><a href="#training-pro-labs"><strong>Training - Pro Labs</strong></a></li>
        <li><a href="#the-exam"><strong>The Exam</strong></a></li>
        <li><a href="#report"><strong>Report</strong></a></li>
        <li><a href="#practical-advice"><strong>Practical Advice</strong></a></li>
    </ul>
</div>
</div>
<br><br>

I recently achieved the HTB Certified Penetration Testing Specialist (CPTS) certification, and I wanted to share my experience and insights with the cybersecurity community. After months of preparation, hands-on practice, and navigating the challenging examination process, I can confidently say this certification represents one of the most practical and valuable credentials available for aspiring penetration testers.
<br><br>

<div style="text-align: center;">
    <img src="blog/images/cpts.png" alt="CPTS Certification" style="max-width: 700px;">
</div>

## Introduction {#introduction}

The HTB Certified Penetration Testing Specialist (HTB CPTS) certification is a highly practical certification that evaluates candidates' skills in penetration testing. It's one of the best regarding the offensive part in the certification market. It covers numerous topics, such as:

- Information gathering & reconnaissance techniques
- Web Application Penetration Testing
- Active Directory Enumeration & Attacks
- Pivoting and Lateral Movement
- Post-Exploitation Enumeration
- Linux & Windows Privilege Escalation
- Vulnerability/Risk communication and reporting



## CPTS vs OSCP {#cpts-vs-oscp}

The dilemma of every penetration tester: CPTS or OSCP, which one to take? This is a topic that every penetration tester faces before taking one of these certifications. In my opinion, the CPTS is the best regarding the knowledge learned, and I'll also explain why:

### Cost {#cost}

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**OSCP:**</a> $1800  
<a style="color: #bc7afe; text-decoration: none; cursor: default;">**CPTS:**</a> $220

The price difference is abysmal and makes the CPTS accessible to many more professionals, especially those who are at the beginning of their career.

### Material Quality {#material-quality}

Regarding material quality, HackTheBox offers a well-structured path, excellent also for newcomers in the field. The modules are organized progressively, starting from theoretical basics to arrive at complex and realistic scenarios.

Offensive Security instead offers a more traditional approach, with the famous motto <a style="color: #bc7afe; text-decoration: none; cursor: default;">"Try Harder"</a>. The OSCP material is consolidated over time but can result less updated compared to modern techniques. The documentation is more spartan and requires greater autonomous research from the candidate.

### Validity/Recognition {#validity-recognition}

Currently the OSCP enjoys greater recognition in the job market, being the first hands-on penetration testing certification. However, the CPTS is rapidly gaining credibility thanks to the quality of the training program and the growing reputation of HackTheBox in the cybersecurity community.



## Training - Pro Labs {#training-pro-labs}

According to my personal experience, to prepare best for the CPTS, besides following all the modules, I also recommend the following Pro Labs provided by HTB:

- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**P.O.O**</a> - Mini Pro Lab
- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**Dante**</a> - Pro Lab
- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**FullHouse**</a> - Pro Lab
- <a style="color: #bc7afe; text-decoration: none; cursor: default;">**RPG**</a> - Mini Pro Lab

If you find particular difficulties in solving them, make sure to review more thoroughly your knowledge on the corresponding modules. Each Pro Lab will allow you to put into practice the techniques learned in a controlled but realistic environment.



## The Exam {#the-exam}

The candidate will perform blackbox web, internal and external penetration testing activities against a real-world Active Directory network hosted in HTB's infrastructure and accessible via VPN (using Pwnbox or their own local VM). 

Upon launching the laboratory environment, you will receive a starting IP address that serves as your initial entry point into the target network. From this single address, you must begin your penetration test by systematically enumerating the environment and expanding your access throughout the network infrastructure.

You have <a style="color: #bc7afe; text-decoration: none; cursor: default;">10 days</a> to complete both the practical testing and written report, with the objective of capturing at least <a style="color: #bc7afe; text-decoration: none; cursor: default;">12 out of 14 flags</a> while producing a professional report that HTB defines as Commercial-grade quality. The report constitutes the majority of your final score. Even if you capture all 14 flags, submitting an unprofessional or poorly structured report will result in exam failure.



## Report {#report}

As mentioned previously, the report is the fundamental part of the exam, and in this section I will give you tips that personally helped me a lot:

During my report writing, I used <a style="color: #bc7afe; text-decoration: none; cursor: default;">**sysreptor**</a>, a completely free platform that will give you enormous help in automating most of the tasks that you would normally have to do manually.

Register here: [https://labs.sysre.pt/login/local/](https://labs.sysre.pt/login/local/)



## Practical Advice {#practical-advice}

In this section I want to give you practical advice to pass the exam and write a good report:

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**Taking notes during the exam:**</a> As you perform scans, find credentials, PoCs, exploits, etc, always keep track of them, so that when you go to write the report you will already have your notes organized.

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**The art of enumeration:**</a> The fundamental part of your success in the exam is precisely enumeration. I say this because personally I lost 2 days because of the latter. Enumerate, enumerate, enumerate, and especially use all the wordlists you know.

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**Report timing:**</a> According to my experience, to write a good report takes at least a couple of days, so if you get the 12 flags and you have few days left, start writing it immediately. If you then have additional time (I don't think so) try to complete the exam by getting the remaining flags.

<a style="color: #bc7afe; text-decoration: none; cursor: default;">**Study the modules well:**</a> Especially the Active Directory part, it's not obvious and if you don't know all the attacks thoroughly you will struggle a lot. The fundamental techniques to master include:

- Kerberoasting and ASREPRoasting
- DCSync and Golden/Silver Ticket attacks
- Windows Privilege Escalation
- Lateral Movement with pass-the-hash, pass-the-ticket
- Bloodhound
- ACL Abuse
---
<br><br>
*by Andrea Gelmi*

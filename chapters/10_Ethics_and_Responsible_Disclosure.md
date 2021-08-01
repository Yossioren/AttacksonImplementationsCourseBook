---
nav_order: 10
---
# Ethics and Responsible Disclosure
1. Table of Contents
{:toc}

## Layout

1.  Computer Laws

2.  Cyber-ethical dilemmas

3.  Responsible disclosure

## Computer Laws

Israel’s computer laws[1] are *case-laws* – meaning there are a few
written laws, and a judge would use those along with precedents and
personal judgment to determine whether a person is guilty. This is
opposed to *continental-law*, in which everything is written and
proceedings are executed literally by the book.

### Definitions

1.  "computer material" - software or computer information

2.  "computer" - A device that works with a software to perform
    arithmetic or logical processing of data and peripherals, with
    exception to auxiliary computer

3.  "auxiliary computer" - A device that is only able to perform
    arithmetic processing

4.  "information" - or computer information, is signs, instructions,
    data or concepts, except for software. the information is expressed
    via computer language and stored in the computer or any other media
    or volume.

5.  "output" - any information that is produced or derived via the
    computer

6.  "computer language" - appropriate expressive form for
    interpretation, delivery or processing by computer

7.  "software" - A group of instructions expressed in the computer
    language that can cause a computer to function or to perform an
    action, and is either embedded or marked with a device or by means
    of electronic, electromagnetic, electro-optics or any other means,
    or either united with the computer in some way or separated from it

The laws state which cyber-activities are considered illegal, as
follows:

1.  Unlawfully disrupting or interfering with a computer system

2.  Unlawfully modifying or deleting any material or files from the
    computer system

3.  Providing false information or false output

4.  Unlawful access, invade or penetrate to a computer system

5.  Unlawful eavesdrop, according to the Wiretap Act 1979 rule

6.  As the above, but in order to commit another offence

7.  Creating, distributing or offering to another person a computer
    virus (a virus can perform variety of malicious actions, such as
    removing/changing files, ransomware, backdoor, etc.)

<figure>
<img src="images/chapter10/computer_in_cyber_crimes.png" id="fig:comp_in_cybercrime" alt="The computer in cybercrime " /><figcaption aria-hidden="true">The computer in cybercrime <span class="citation" data-cites="tabansky2012cybercrime"></span></figcaption>
</figure>

From this we learn that not any crime committed with the aid of a
computer constitutes a cyber-crime; if a computer was used in the
process of the crime, but none of the above computer laws were broken –
for example while profiteering[2] off an online ticket sale – the
action, while illegal, is not a cyber crime.

### Unlawful Disruption or Interfering with a Computer System

##### Definition.

Disrupting the normal operation of a computer, interfering with the use
of a computer or deleting of materials saved on a computer.

Let’s observe some examples:

-   Performing a DDoS attack on a server

-   Infecting a computer with a virus preventing access to information
    saved on it

-   Recruiting a computer into a botnet, thus draining its resources

-   Infecting a computer with a program that sends information from it
    to a remote server

-   Cheating at a single player video game

-   Installing an unlicensed program

All of the above actions are illegal. The first three are violations of
the first section of Israel’s computer laws, while the latter three are
illegal for other reasons, since they do not directly prevent/interfere
with the victim’s system’s functions.

### False Information or Output

##### Definition.

Misinformation; generating, or changing the code of a program such that
it would generate information that is forged or misleading. Let’s
observe some examples:

-   Sending an email on behalf of someone else without their consent

-   Changing the code of a grade-calculating program in order to change
    the output grades

-   Cheating in an online game to gain an unfair advantage

-   Using a *key generator*: a program that forges fake software
    licenses

-   Recruiting a computer into a botnet

-   Accessing an email inbox of another user

All of the above actions are illegal, but only the first four violate
the second section of Israel’s computer laws.

### Unlawful Access

##### Definition.

Virtual trespassing; any action which results in the perpetrator
accessing information to which they do not have access, such as images,
text files, code, etc.

Let’s observe some examples:

-   Viewing personal information of coffee shop patrons by using the
    same Wi-Fi

-   Penetration testing (attempting to find weaknesses) on a company’s
    server without its consent

-   Using some else’s password to access their inbox without their
    consent

-   Using a program to forge credit card numbers

Forging credit card numbers, while illegal, does not fall under this
section of the law; it is constitutes as false information. Note that
penetration testing is a violation of this section of the law even if it
is unsuccessful.

## Cyber Ethics

We first present two case studies, then proceed to discuss them and
cyber ethics in general.

### Case Studies

##### Stresser.

Two people from Israel ran a DDoS service, known as Stresser, which
performed DDoS attacks on websites for money. They made a large profit,
but were eventually caught, and claimed they were ethical, and there are
occasions where they refused to attack Israeli websites. What were their
motives?

##### Eternal Blue.

In 2013, the NSA found a vulnerability in Windows  and secretly built a
tool called Eternal Blue to exploit it. At some point, a group of
hackers known as the Shadow Brokers stole security tools from the NSA
and offered to sell them on the Dark Net. When nobody paid, the Shadow
Brokers leaked the tools. Microsoft released a patch to fix the bug a
short time later; the patch was prepared in advance after Microsoft was
tipped off by the NSA.

In 2017, a piece of malware known as “WannaCry" first appeared; it
utilized Eternal Blue to spread quickly through computers on which the
security patch wasn’t yet installed, and encrypt the victim’s files,
then asking for money to decrypt them[3].

<figure>
<img src="images/EthernalBlue-WannaCry_Timeline.jpg" id="fig:wannacry_timeline" alt="EthernalBlue-WannaCry Timeline" /><figcaption aria-hidden="true">EthernalBlue-WannaCry Timeline</figcaption>
</figure>

WannaCry was finally beaten when a malware researcher found it made
requests to an unused control domain, and purchased the domain.[4] As it
turned out, purchasing the domain triggered the destruction of WannaCry,
whether by mistake or by design (the domain could have been designed as
a kill-switch).

While WannaCry did not make a lot of money, it had a nasty side-effect
on healthcare systems; medical equipment that got infected could not
function normally, with dangerous, possibly lethal, repercussions.

Suppose a man was killed due to a failure induced by WannaCry; let John
be such a casualty. There are many parties in this story, each holding
part of the blame for John’s death:

-   WannaCry’s writers, whose malware caused John’s death

-   Microsoft, whose software was used and trusted by the hospital

-   The hospital, which relied solely on Microsoft’s software without
    providing safety measures of their own

-   The NSA, who knew about the bug well in advance, but did not perform
    responsible disclosure

-   The Shadow Brokers, who leaked the NSA’s tools to the public, which
    lead to the development of WannaCry

### Discussion

##### Ethics.

Ethical behavior is deciding how to act according to one’s moral system.
It is mostly instinctive, or composed of a personally devised code,
rather than conforming to a set of rigid universal rules.

##### The Trolley Problem.

Imagine a trolley approaching a fork in the railway. On the first path
lie five people, and on the second only a single person. The trolley, if
its course remains unchanged, will head for the first path, resulting in
the deaths of the five people there. However, you as a bystander have
the option to pull a lever to change the direction of the trolley to the
second path, resulting in the single death of the man there.

<figure>
<img src="images/The_Trolley_Problem.jpg" id="fig:trolley_problem" alt="The Trolley Problem" /><figcaption aria-hidden="true">The Trolley Problem</figcaption>
</figure>

According to the numbers, you should pull the switch to save the five.
But in that case, by sending the trolley toward the single person on the
other path, you are *directly* responsible for his death! So should you
avoid getting involved, thus allowing the deaths of five people instead?

What if one of the people is a close friend? Would that change your
answer?

There is another version to this problem, in which there is only a
single road with five people on it. You, along with a very large man,
are standing on a bridge above the road, and you have the option of
*pushing* the large man beside you off the bridge to block the
approaching trolley. The stakes are the same, but in the scenario, in
order to save the five you need to actually commit murder!

<figure>
<img src="images/The_Trolley_Problem_Fat_Man.jpg" id="fig:trolley_problem_fat_man" alt="The Trolley Problem (Fat Man)" /><figcaption aria-hidden="true">The Trolley Problem (Fat Man)</figcaption>
</figure>

Our “closeness" to a situation affects on how we judge it by our moral
standards.

##### How to decide.

There are two main theories by which the morality of an action is
judged:

-   Deontological ethics (Kant[5]) – what do my rules/morals say about
    this action? (i.e. judge by motives)

-   Utilitarian ethics (Bentham[6]) – what are the consequences of this
    action? (i.e. judge by consequences)

Consider the cyber setting. If we were to program ethics into an AI
(say, an autonomous car), we would have to use Utilitarian Ethics – a
score system by which the algorithm could judge what would be the least
terrible outcome according to our moral system.

This presents complications; for example, let’s consider a practical
implementation of the Trolley Problem in autonomous cars: Assume a car
is driving on a bridge containing five pedestrians in the middle of the
road. If the car continues on its path, they will all die. However, the
car can choose to veer off the bridge, saving five lives but killing the
driver. By utilitarian considerations, this is the best approach – but
who will purchase a car which is programmed to kill him on certain
circumstances?

<figure>
<img src="images/chapter10/dilemmaA.png" id="fig:a" alt="killing several pedestrians or one passer by" /><figcaption aria-hidden="true">killing several pedestrians or one passer by</figcaption>
</figure>

<figure>
<img src="images/chapter10/dilemmaB.png" id="fig:b" alt="killing one pedestrian or killing its own passenger" /><figcaption aria-hidden="true">killing one pedestrian or killing its own passenger</figcaption>
</figure>

<figure>
<img src="images/chapter10/dilemmaC.png" id="fig:c" alt="killing several pedestrians or killing its own passenger" /><figcaption aria-hidden="true">killing several pedestrians or killing its own passenger</figcaption>
</figure>

##### Cyber crime.

Our brain is “programmed" to feel distressed when confronted with an
unethical scene; i.e. when we see a scene of a person committing an
unethical act, we feel bad in sympathy with the victim. This is why it
is easier to commit a cyber crime – we do not see the victim, and do not
sympathize with them. Upholding cyber ethics would mean artificially
causing users to use their judgment when their brains would not.

## Responsible Disclosure

Disclosure is the act of alerting a product vendor to a vulnerability in
their product so that they could patch it. Disclosure is performed by an
honest party (i.e. not a hacker who wishes to exploit the vulnerability)
with the intention of increasing the security of the product. There is a
question of exactly when and how to perform this disclosure.

An exploit is considered as *zero day* when the vendor is unaware of the
vulnerability it exploits (meaning it is known only to a few, and
unknown to the general public - i.e. it has not been disclosed).

describes a timeline of a vulnerability from the moment it is found to
the moment its patch is deployed.

<figure>
<img src="images/Vulnerability_Timeline.PNG" id="fig:vulnerability_timeline" alt="Timeline of a vulnerability" /><figcaption aria-hidden="true">Timeline of a vulnerability</figcaption>
</figure>

Symantec, the company founding Nortron[7], had a lot of data regarding
vulnerabilities and exploits, and used it to research the matter. shows
their results.

<figure>
<img src="images/Disclosure_Research_Findings.PNG" id="fig:disclosure_research_findings" alt="Symantec’s disclosure research findings" /><figcaption aria-hidden="true">Symantec’s disclosure research findings</figcaption>
</figure>

From Symantec’s results, we conclude the following:

-   Zero days exist

-   Usually zero days are targeted, and not highly used so that they
    would remain secret.

-   Disclosure is terrible for security; after a patch is released,
    attackers use it to find the vulnerabilities and exploit them.
    Attackers go through public responsible disclosure and attack even
    before a patch is released. Between the point where the disclosure
    was made publicly and the patch deployment was completed, the scale
    of attacks rose by 5 orders of magnitude, making public disclosure a
    bad idea.

##### Responsible disclosure.

There is a government operated website called CVE – Common
Vulnerabilities and Exposures. Disclosure could be performed by
uploading a vulnerability to the site such that only the owner of the
software can see it, and publish the details only when a patch is
released (between points *t*<sub>*p*</sub> and *t*<sub>*a*</sub> in
<a href="#fig:vulnerability_timeline" data-reference-type="ref" data-reference="fig:vulnerability_timeline">1.8</a>),
to avoid the window when the vulnerability is public and unpatched
(between *t*<sub>0</sub> and *t*<sub>*p*</sub> in
<a href="#fig:vulnerability_timeline" data-reference-type="ref" data-reference="fig:vulnerability_timeline">1.8</a>).
Microsoft called this practice of disclosing privately Coordinated
Vulnerability Disclosure, and claim it significantly reduces the amount
of exploits on new vulnerabilities.

Google introduced a system where the vulnerability remains private for
90 days, after which it goes public, with or without a patch. The strict
deadline is meant to make sure the vulnerable vendor does not dismiss
fixing the bug due to it being unknown, and thus security is improved.

<figure>
<img src="images/chapter10/macOScve2.png" id="fig:macOSsve" alt="Example to a cve entry of a vulnerability found in macOS" /><figcaption aria-hidden="true">Example to a cve entry of a vulnerability found in macOS</figcaption>
</figure>

Over the years using machine learning with CVEs was used for detecting
and classifing vulnerabilities in code, as well as making automatic
predictions for unseen vulnerabilities.

On the other hand, CVEs can be used to find unpatched exploits – for
example, there was a bug in Linux which hasn’t yet gone public, but
someone needed to commit the changes, which contained the CVE-ID. Thus
hackers could see the fix and exploit the vulnerability before a patch
was posted.


## Analysis of cyber cases in the Israeli judicial system
In this section we will present a review of 4 cyber case studies that are related to Israel’s Computer Laws and went to trial.
The first part will include a summary of a case, the court decisions in regard to the case and a discussion about each case.
The second part will be composed of questions in the form of a test about the case and will also include a True or False 
questions to allow practice and understanding of Israel cyber laws. 
### Avi Mizrahi 2004 - Israeli man charged with hacking Mossad
Avi Mizrahi was interested in working at the Mossad, Israel's main intelligence agency, but did not know how to apply to 
this organization. In 2002, Mossad uploaded a webpage which can only be used to leave contact information for candidates.
Avi Mizrahi suspected that this webpage was fake and he feared that the details of his candidacy would be visible to other parties.
He carried out a number of actions for which he was charged with an offense of attempted penetration of computer material 
contrary to clause 4 of Israel's computer laws[1]. Here are the main points of the indictment:
1. On 22.9.2002, at around 19:25, the defendant attempted to penetrate computer material with a computer that was in an office in Jerusalem.
2. The defendant connected the Webpage of the Mossad.
3. The defendant used cracking and hacking software against the site, which launched dozens of various cracking attempts of many different code defenses of the Webpage's.
4. The defendant also output the results of the "attack" data on the site, which allows you to know what are the security failures in the Webpage's.
5. The defendant asked for assistance over the internet in reading the output of the data that he could not read himself. The defendant carried out the alleged act although he assumed that it was unlawful.
The judge in this trial was Dr. Avi Tenenbaum, who had several academic degrees in law, criminology and computer science. The following are the main points of summary of the judge's decision:
- **The defendant does not understand computer security** and does not pretend to understand.
- The defendant had been interested in joining the institution for a long time prior to this incident. When the Mossad website was uploaded, the defendant entered the Mossad's website with the aim of joining his services and suspected that it was an unsecured site.
- There is no way to communicate with its managers and there is only an application form with no details to contact the Mossad representatives.
- The defendant contacted a site that included software of computer security and hacking. He downloaded the popular software which had the highest number of downloads. It's an anonymous software that the defendant didn't understand much about. To activate it, he only had to type in the destination address.
- The software produced a log that the defendant could not understand. He made an online query asking for help.
- The defendant did not receive any responses to the request and then deleted the software.
- The defendant made **no attempt to conceal anything** and from the very first moment cooperated fully with his interrogators. Also, the actions carried out simply without attempted concealment and disruption.
- The judge's decision was the **acquittal** of the defendant.
The State Attorney's Office has filed an appeal with the District Court. The District Court ruled that the defendant is innocent. 

#### Discussion
- The term illegal penetration in clause 4 [1] is unclear and it would have been advisable to add clarification in the law to this issue. For example, penetration without the permission of the site manager.
- "Don't Mess with the MOSSAD"- The defendant's activity was carried out on the Mossad's website. In our opinion, this claim would not have been filed if this activity had been carried out on the website of another government organization (transportation, agriculture, etc). Also, we think it's a show of strength for this organization that wants to make it clear that it's not being messed with.
- The difference between the penetration of the physical world and the virtual world is inconclusive and clear. For example, an attempted door-breaking at home versus attempted hacking in the virtual world. 
- In our opinion, the defendant was not charged in trial because of the judge's knowledge and understanding of computer science.

### Moshe Halevy (HALEMO) 2009- Israeli man charged with hacking to Collecting fines site

Moshe Halevy (HALEMO) is a famous blogger in the field of technology in Israel.
In 2005, he published an unsympathetic article about the first spammer, Ofer Sdot, who went to prison for three years.
After his release from prison, Ofer asked HALEMO to delete the article on the grounds that it was offensive to his new career as an investment entrepreneur.
HALEMO did not respond to this request and then a confrontation began between them. Ofer sent spam messages to HALEMO and HALEMO contacted the police who decided not to act on the matter and expected that the issue would be dealt privately between them.
Ofer sends pedophile material by email to HALEMO.HALEMO went to the police but again the police decided not to intervene.
HALEMO responds with phone calls as a harassment operation against Ofer during the day and night.
HALEMO also ordered pizzas to Ofer's house free of charge. He also went to the debt collection website and searched for details about Ofer's debts. HALEMO exploited a weakness that exists on the site in order to obtain details of Ofer's debts.
HALEMO paid 2 NIS to receive a document for **HALEMO's address** showing Ofer's debt of 7 million NIS.
On this site there was a weakness **without** HALEMO 's knowledge in the way that partial payment leads to the **cancellation of all debt**. During a routine audit of this organization, the gap in the debt reset of NIS 7 million was revealed and a police investigation was opened. The Police are investigating Ofer but found no evidence of a crime. Ofer claims to police that HALEMO may have done this.
Police indict HALEMO for committing sophisticated computer fraud contrary to clause 3 and 5 of the Israel’s computer laws[1].
The judge in this trial was Dr. Avi Tenenbaum.
The following are the main points from the summary of the judge's decision:

- This is not a 'sophisticated computer scam' but a simple operation that anyone with a minimal understanding of computers can take.
- The defendant did not attempt anywhere to conceal his actions and/or evade responsibility.
- The facts show that there is no 'sophistication' here on the part of the defendant, but a serious failure that the defendant is not at all a party to.
- If there was room for blame for something, it would be towards the state and its authorities that enabled these actions. The site was not built for partial payments. **Partial payment of the debt leads to the cancellation of all debt**.
- The defendant **was unaware of the site's failures** and so the incident unfolded in a direction that could not be expected.
- The defendant refused to accept representation of a public defender although the defendant is not a lawyer and has no formal legal education.

#### Discussion
- The term illegal penetration in clause 5 [1] did not exist because there were no **reasonable security mechanisms** on this site.
- Is entering another person's information into the site an illegal act for which to be punished? **In the virtual world, there is no clear boundary between penetration and non-penetration**. 
- The organization collecting the fines did not reasonably protect the privacy of the information. Performing a simple action of changing ID resulted in maliciously obtaining private information by exploiting the weaknesses of the security mechanisms. Implementation of security tools will be able to enable protection through the law against dealing with illegal **penetration**, etc. 
- What is the **limit on which police should handle harassment** incidents that take place in the virtual world such spam, deletion of content, private information, etc?

### Doron Ben Shoshan (2014)- Perform malicious actions after dismissal

Doron served as a computer network administrator for a company that provides computer services and had an administrator password.
Doron got into a feud with his workplace and then quit the company. Doron’s workplace **hasn't revoked** his corporate network password.
As part of the discourse on his severance pay, there was a **dispute** between him and the **company representative**.
Doron then connected from VPN in his private computer to the corporate network using his password and performed a number of malicious actions such as deletion of data, deletion of settings, turning off FW security mechanisms of three of the company’s customers and data change. The actions described above caused the computer networks of the three customers to shut down for about six hours.
The company complained to the police and there was a trial where Ben got charged by clauses 4 and 2.2 of Israel's computer laws[1].
Doron admitted his actions but claimed that this is an offense of malicious damage to property and not a violation of the charged clauses 4 and 2.2.
Also, the interpretation of those rules and the purpose of the legislation is to prohibit computer penetration or tampering with computer material only through designated software - such as "virus" or hacking software.
The Shalom's Court in Jerusalem convicted him on these counts. Doron filed an appeal to the District Court for his conviction.
The District court decided to overturn the conviction so as not to cause disproportionate harm to the appellant and at the prospects of employment in the future, he was sentenced to 340 hours of public service. Also, for a one year probation **without a conviction**.

#### Discussion
- There is a **public interest in reducing the phenomenon** of computer delinquency and in particular computer penetration because of the relative ease involved in the penetration of computer material by such and other technological means and misuse of modern technology. 
- Not deleting a fired **employee's password** is not a reason for employee abuse. In our opinion, It's necessary to examine the addition of a clause in the law that will not allow an employee who has been convicted in such criminal offenses to continue working in that technological field.
- The employee did a very serious thing as he not only harmed his company but also damaged corporate networks of customers. In our opinion, It's necessary to examine the addition of a clause in the law which refers to the worsening of the punishment if the defendant has committed offenses in other organizations beyond his organization.

### Nir Ezra (2015) - Stealing money from Israeli users’ bank accounts

Nir Ezra contacted hackers', requesting password information of other users' bank accounts and debit cards.
In this section, we will review his actions on obtaining password information of Israeli users to local bank accounts.
As a result, Ezra received from an unknown person the details of four or five bank accounts.
On July 15, 2010, Ezra used the bank account details of Lydia Rahman and transferred an amount of 3,000 NIS without consent to Igor Nemtsov's account in exchange for converting virtual jitons.
For this action, he was charged with an offense of penetration of computer material clause 5 of Israel's computer laws[1], theft and obtaining anything fraudulently in aggravated circumstances.
In order to convict an offense under clause 5 of the Computers Law, it is necessary to prove that the defendant committed an offense of illegal penetration for computer material. The defendant believes that connecting over the Internet using a password is at most penetration into the **"output" of a computer** that is not defined as computer material.
The court convicted the defendant of this clause 5 of the Computers Law. 
The defendant appealed this decision to the District Court. The District Court overturns Ezra's conviction for penetration into computer material. The District Court ruled that there should be a hacker or at the very least the right knowledge and tools to overcome a **technological obstacle** (encryption, firewall, etc) to be convicted of an offense of penetration into computer material.
The State Attorney's Office filed an appeal to the Supreme Court.
The Supreme Court reinterpreted the term “lawlessly” to “without consent”.
The Supreme Court decided that no action was required to circumvent a technological obstacle as a condition of conviction for an offense and sentenced him to **four months of service** and compensation.
### Conclusion
In conclusion, we can see in each case that there are gray areas where it’s not quite clear where immorality ends and criminal behavior starts. We examined these cases only in association with Computer Laws offenses. In some cases the offenses are also related to other issues such as privacy laws, fraud and theft. We didn’t refer to those issues in this section.
The Computer Laws are dated (1995) and the advancement of technology is a very good reason for updating those laws, especially since nowadays it’s relatively easy to penetrate computer material by such and other technological means and misuse of modern technology. 
### Test


1. To which organization is Mr. Avi Mizrahi accused of hacking?
    1. Bank Hapoalim
    2. Soroka Medical Center
    3. IDF- Israel Defense Forces
    4. Mossad - Israel's main intelligence agency
2. What was the District Court's decision regarding Avi Mizrahi's case?
    1. He was found guilty
    2. He was found not guilty
    3. Avi Mizrahi's case did not get to court at all
    4. Avi appealed the court's decision and the case is still pending
3. What was the act of Avi Mizrahi in which he was charged?
    1. Creating or distributing a computer virus
    2. Cracking and Hacking software against the site
    3. Forging credit card passwords
    4. Send spam email
4. What is the maximum penalty in Clause 4 (of Israel's computer laws) for which Mr. Avi Mizrahi was charged?
    1. Year
    2. 2 Years
    3. 3 Years
    4. 5 Years
5. Why did Mr. Mizrahi hack the website?
    1. He wanted to impress his friends
    2. He wanted to see if he can do it
    3. He thought it's a malicious site
    4. He wanted to change data
6. Who was Moshe Helevy?
    1. The CEO of a known tech company
    2. A famous blogger
    3. An entrepreneur
    4. A government employee
7. What was the police’ response to HALEMO when he first contacted them Ofer’s spam messages and pedophile material sent to him?
    1. They immediately opened a case against Ofer
    2. They ignored HALEMO completely
    3. They wanted nothing to do with the matter and asked them to solve it in private.
    4. They arrested Ofer
8. What led to the cancellation of Ofer’s 7 million NIS debt?
    1. The 2 NIS HALEMO paid in order to receive the information
    2. Ofer’s own hacking to the site and deleting his debt
    3. A malfunction of the site leading to the cancellation of the debt
    4. Both a+c are correct
9. What was HALEMO convicted for?
    1. Illegal penetration to a website
    2. Obtaining private information illegally
    3. Harassment 
    4. He was not convicted at all
10. What was the Judge’s main claim?
    1. That no one should try to obtain someone else’s private information
    2. That there should be reasonable security mechanisms for such financial sites.
    3. That there is no justification for sending someone so many pizzas
    4. None of the above
11. What was Doron’s position at the company?
    1. He was a regional director
    2. He was the CTO
    3. He was the CFO
    4. He was a computer network administrator
12. Why did Doron quit the company he worked at?
    1. He got another job
    2. He wanted to rest
    3. He got into a feud with his bosses
    4. He didn’t like the company’s name
13. To whom Doron caused damage in his actions?
    1. Only the company he worked for
    2. Himself
    3. The company he worked for and three of its customers
    4. b+c are correct
14. Why did Doron appeal?
    1. He did not agree with the clauses of the law he was charged for
    2. He felt he was mistreated in trial
    3. He did not like the judge who convicted him
    4. None of the above
15. What did the District Court do?
    1. Accept the appeal
    2. Did not accept the appeal
    3. Charged Doron with an additional offense
    4. b+c are correct
16. How did Nir get the private information of Israeli users?
    1. He hacked them by himself
    2. He contacted hackers in order to obtain the information for him
    3. He didn’t eventually
    4. He downloaded a public document
17. What was the purpose of Nir’s actions?
    1. Stealing money
    2. Demonstrating his abilities to a friend
    3. Testing himself
    4. He had no specific purpose, just having fun
18. How many times did this case get appealed?
    1. It didn’t
    2. Once
    3. Twice
    4. There is no mentioning of any appeal in this specific case
19. How many years was Nir sentenced to?
    1. He was sentenced to only 4 months
    2. 4 years probation
    3. 4 months of service and compensation
    4. 2 years and compensation
20. Did Nir’s case cause a change in the law?
    1. Not at all
    2. Yes, it got amended
    3. Yes, the entire clause was changed
    4. It wasn’t Nir’s case that caused the changes.

##### Answers

1-iv, 2-ii, 3-ii, 4-iii, 5-iii, 6-ii, 7-iii, 8-iv, 9-iv, 10-ii, 11-iv, 12-iii, 13-iv, 14-i, 15-i, 16-ii, 17-i, 18-iii, 19-iii, 20-ii


#### True/False Questions

Choose the actions that are considered a cyber offense:
1. False statement about age at the entrance to an online age restricted website
2. Entrance to an email account that has been left open
3. Penetration testing to Soroka Medical Center website with approval 
4. Entrance to someone’s Twitter account and posting messages on their behalf 
5. Snooping on your partner's Twitter account
6. Developing a software to forge credit card numbers
7. Snooping on your child's Twitter account
8. Using the workplace computer equipment for personal purposes contrary to the employer's consent
9. Posting on someone else's Facebook account without their knowledge
10. Looking over someone's shoulder while he or she are at the ATM 
11. Turning off IoT air conditioner without the owner's consent
12. Using a friend's username and password in order to surf in a pre-paid website
13. Opening an attachment that was sent to my child with permission
14. Turning on a friend's computer with permission
15. Brute force
##### Answers

1-True, 2-True, 3- False, 4-True, 5-True, 6-False, 7-True, 8-True, 9- True, 10- True, 11- True, 12- True, 13- False, 14- False, 15- True 

[1] Published in *Sefer Hachukkim* 5755 No. 1534, 25 July 1995 p. 366
(P.L. 5754 No. 2278 p. 478).

[2] The activity of taking unfair advantage of a situation to make a
large profit, often by selling goods that are difficult to get at a very
high price (Cambridge Business English Dictionary).

[3] This is known as ransomware. Recall that this falls under the first
section of the computer laws.

[4] Malware researchers often try to purchase control domains in order
to gain information on the behavior of the malware.

[5] Immanuel Kant was a German philosopher during the Enlightenment era.
His contributions have had a profound impact on almost every
philosophical movement that followed him.

[6] Jeremy Bentham was an English philosopherduring the Enlightenment
era and a social reformer regarded as the founder of modern
utilitarianism.

[7] Norton is an anti-virus.

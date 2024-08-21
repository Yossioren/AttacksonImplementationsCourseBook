# Attacks on Implementations of Secure Systems

This is the handbook for the course "Attacks on Secure Implementations", taught in 2020 at Ben-Gurion University by Dr. Yossi Oren.

You can download the PDF of the entire handbook [here](https://github.com/Yossioren/AttacksonImplementationsCourseBook/raw/master/UniversityCourseBookAOI.pdf), or view it online [here](https://orenlab.sise.bgu.ac.il/AttacksonImplementationsCourseBook/). 

The source code for the handbook, experimental labs and other fun material can be found in the GitHub repository:

[https://github.com/Yossioren/AttacksonImplementationsCourseBook]

Online course page: [https://moodle2.bgu.ac.il/moodle/enrol/index.php?id=30088]

More information: [https://iss.oy.ne.ro/Attacks]

# Course materials

### Lecture 1 - Introduction
[Textbook Link](https://orenlab.sise.bgu.ac.il/AttacksonImplementationsCourseBook/01_introduction)

- [TEMPEST](https://www.youtube.com/watch?v=m7FYn4XMONE&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=64) and secure communications, an attack on teletypewriter repeater machine. Part 1 (15 minutes);
- [TEMPEST](https://www.youtube.com/watch?v=lQzzB87ADYA&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=70) and secure communications, an attack on teletypewriter repeater machine. Part 2 (18 minutes); 
- [Examples of implementation attacks on other machines](https://www.youtube.com/watch?v=HVFg5JGpU0k&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=71) (11 minutes);
- [Implementation attacks on secure devices](https://www.youtube.com/watch?v=x0C-5wAg38s&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=69)  (9 minutes);
- [Between theory and implementation](https://www.youtube.com/watch?v=BMpsojq_Z7M&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=68): System security, cryptographically secure algorithms and protocols, secure architectures  (19 minutes);
- [Breaking an implementation](https://www.youtube.com/watch?v=ZcSvl1MO9MA&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=67): The difference between theory and implementation (11 minutes);
- [Constructing and using a threat model](https://www.youtube.com/watch?v=JT9VGrV2wIQ&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=66): Review of the victim assets and the attacker capabilities (19 minutes);
- [Case studies](https://www.youtube.com/watch?v=xDp1Tz4TXHE&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=65): Review examples of attacks  (23 minutes);

Basic reading is the first chapter of Coursebook; for further reading, see the paper about the [TEMPEST](https://cryptome.org/nsa-tempest.pdf); here's Thomas Popp's paper [An Introduction to Implementation Attacks and Countermeasures](https://ieeexplore.ieee.org/document/5185386); there's also an [Overview about Attacks on Smart Cards](https://linkinghub.elsevier.com/retrieve/pii/S1363412703001079);

### Lecture 2 - Temporal Side Channels I
[Textbook Link](https://orenlab.sise.bgu.ac.il/AttacksonImplementationsCourseBook/02_Temporal_SC_1)

- [Countermeasures and their drawbacks](https://www.youtube.com/watch?v=s_ZSHFCO0Fc&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=64) (14 minutes);
- [A history of temporal Side Channel](https://www.youtube.com/watch?v=ohJRhhPX5t8&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=63) (10 minutes);
- [The definition of Temporal Side Channels](https://www.youtube.com/watch?v=wqBZ6cy-Z8g&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=62) (6 minutes);
- [A timing attack on passwords](https://www.youtube.com/watch?v=S_TmpLgNASw&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=61) part 1 (15 minutes);
- [A timing attack on passwords](https://www.youtube.com/watch?v=rBCy7t72qos&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=60) part 2 (23 minutes);
- [Countermeasures to timing attack on passwords](https://www.youtube.com/watch?v=JQ_P37_4VQ8&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=59): Examples of password checkers. (16 minutes);
- [The Algebra behind RSA](https://www.youtube.com/watch?v=_r_LBRVDROg&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=58) (16 minutes);
- [Make RSA more efficient via LR and CRT](https://www.youtube.com/watch?v=xSpX2HpEA-k&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=57) (18 minutes);

Basic reading is the second chapter of Coursebook; for additional background reading on timing attacks, see [A Practical Implementation of the Timing Attack](https://link.springer.com/chapter/10.1007%2F10721064_15); To read more about Montgomery's Modular Multiplications, see [Modular Multiplication Without Trial Division](https://www.ams.org/journals/mcom/1985-44-170/S0025-5718-1985-0777282-X/home.html); there's also an [Overview about Attacks on Smart Cards](https://linkinghub.elsevier.com/retrieve/pii/S1363412703001079); To delve more the math behind RSA, you can read [Kaliski's "The Mathematics of the RSA Public-Key Cryptosystem"](https://www.ams.org/publicoutreach/msamhome/06-Kaliski.pdf);

### Lecture 3 - Temporal Side Channels II
[Textbook Link](https://orenlab.sise.bgu.ac.il/AttacksonImplementationsCourseBook/03_Temporal_SC_2)

- [Make RSA more efficient via Montgomery reduction](https://www.youtube.com/watch?v=C2686MV9vew&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=56) (18 minutes);
- [An example of a practical timing attack on RSA using Montgomery Reduction](https://www.youtube.com/watch?v=-cxhBdt-MHc&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=55) - A brief overview of a practical timing attack (9 minutes);
- [The "Vaizata" method - an introduction](https://www.youtube.com/watch?v=LxLzLLBZfeU&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=54) - An introduction to the Vaizata method, with 5 basic steps: implementation assumption, guessing part of the key, formulating a hypothesis, measurements classification, and drawing out statistical meaning (16 minutes);
- [The "Vaizata" Method in practice - PART 1](https://www.youtube.com/watch?v=WFWi-pTZkiM&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=53) - A partial example of using the Vaizata method (12 minutes);
- [The "Vaizata" Method in practice - PART 2](https://www.youtube.com/watch?v=iUHFYZADD48&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=52) - The second part of the practical example to the Vaizata method, following each one of the 5 steps (18 minutes)
- [The "Vaizata" Method - wrap up](https://www.youtube.com/watch?v=4qL6JrwMDgE&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=51) - The final video regarding the Vaizata method, with a statistical analysis demo using Matlab (23 minutes);
- [Countermeasures to RSA timing attacks](https://www.youtube.com/watch?v=Ppv_HMWkWdI&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=50) - How to mitigate and prevent timing attacks (Hiding, Masking, Blinding, Square and Always Multiply) (17 minutes)
- [Bonus: timing attack paper - BlackHat2013](https://www.youtube.com/watch?v=m7-wk4a1YVY&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=49) - A [link](https://youtu.be/KcOQfYlyIqw) to the 2013 BlackHat session on timing attacks featured by Paul Stone, where he introduces a number new techniques that use JavaScript-based timing attacks to extract sensitive data from browsers (6 minutes for the lecture video, 51 minutes for the YouTube video).

Basic reading is the 3rd chapter of our Coursebook. It starts with a recap and then introduces efficient implementations of modular exponentiations as described in Chapter 14 of [The Handbook of Applied Cryptography](https://doi.org/10.1201/9781439821916); To read about a cheaper way for modular multiplication, you can learn about the [Chinese Remainder Theorem](https://books.google.co.il/books?id=RQLtCgAAQBAJ&lpg=PR5&ots=l13HVwsuKW&dq=Chinese%20remainder%20theorem%3A%20applications%20in%20computing%2C%20coding%2C%20cryptography&lr&hl=iw&pg=PR5#v=onepage&q=Chinese%20remainder%20theorem:%20applications%20in%20computing,%20coding,%20cryptography&f=false); You can also read the 1998 paper ["A Practical Implementation of the Timing Attack"](https://link.springer.com/chapter/10.1007%2F10721064_15) that proposes improvements to Kocher's idea that when the running time of a cryptographic algorithm is non-constant, timing measurements can leak information about the secret key; Then it discusses the Vaizata method, and it's recommended you brush up on [T-Tests](https://en.wikipedia.org/wiki/Student%27s_t-test), developed by Guinness head brewer, [William Sealey Gosset](https://en.wikipedia.org/wiki/William_Sealy_Gosset);

### Lecture 4 - Power-EM Side Channels I
[Textbook Link](https://orenlab.sise.bgu.ac.il/AttacksonImplementationsCourseBook/04_Low_Data_Complexity_Power_EM_1)

- [Basic electric circuit and Ohm's Law](https://www.youtube.com/watch?v=KNHn61t1Bmg&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=48) - A brief overview/refresh for Ohm's Law (20 minutes);
- [Open and Short Circuits](https://www.youtube.com/watch?v=8cvmVmwj0QY&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=47) - An overview on short circuits and open circuits (14 minutes);
- [Introduction to transistors(and other electronic components)](https://www.youtube.com/watch?v=6W9VeMXTERI&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=46) (15 minutes);
- [Computational circuit based on FET - CMOS](https://www.youtube.com/watch?v=7YJUMdPCXFA&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=44) - Demonstrating combinational circuits and logic gates (17 minutes);
- [Sequential circuits based on FET](https://www.youtube.com/watch?v=CNa20b0UpBk&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=45)(10 minutes);
- [Power consumption: Representation and computation](https://www.youtube.com/watch?v=P2HB80Af7v4&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=43) - How attackers can exploit device clock frequency, circuit activity, and power consumption to gain knowledge about the device for their own benefit (9 minutes);
- [Types of noise & power consumption vs EM](https://www.youtube.com/watch?v=1MwLpdDfo1E&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=42) - Introducing the 3 different types of Noise, and a short explanation on drawing measurements via Electro Magnetism (11 minutes);
- [Attacker setup explanation & demonstration](https://www.youtube.com/watch?v=y0WVhA4yp0k&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=41) - Exploring a Power-EM attacker setup  (10 minutes);

Basic reading is chapter 4 of the Coursebook, that starts with an introduction to electric circuits and the involved components, [Ohm's Law](https://en.wikipedia.org/wiki/Ohm%27s_law), [logic gates](https://en.wikipedia.org/wiki/Logic_gate) and calculating the power consumption on a CMOS device using the [Hamming Distance Model](https://en.wikipedia.org/wiki/Hamming_distance);


### Lecture 5 - Power-EM Side Channels II
[Textbook Link](https://orenlab.sise.bgu.ac.il/AttacksonImplementationsCourseBook/05_Low_Data_Complexity_Power_EM_2)

- [The New York Times 1998 - Paul Kocher](https://www.youtube.com/watch?v=rC6mYV5f1cw&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=40) - Revisiting an attack from the 1995 on Smart Cards (10 minutes);
- [Simple Power Analysis Main idea](https://www.youtube.com/watch?v=PDWMQ-3It0g&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=37) (17 minutes);
- [MC, ASIC & FPGA](https://www.youtube.com/watch?v=lE3S2Nm3L2o&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=39) (10 minutes);
- [Basic MC - Virgulator](https://www.youtube.com/watch?v=L13p5dFl2P0&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=36) (17 minutes) - Introducing the [Virgulator](http://tice.sea.eseo.fr/riscv/) - a Javascript-implemented micro controller simulator;
- [Simple power analysis of RSA](https://www.youtube.com/watch?v=dTCsycglAxg&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=38) (13 minutes);
- [The history of AES](https://www.youtube.com/watch?v=emBHqbA27u4&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=35) (17 minutes);
- [AES - Main theme](https://www.youtube.com/watch?v=OTvMCIzht8U&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=34) - Exploring the AES/Rijndael encryption standard, it's strengths and steps. (23 minutes);

The basic reading is Chapter 5 of the Coursebook up to around 5.12 "AES Internals"; It starts by Kocher's 1995 smart card power analysis attack that made it to the front page of The New York Times. It then further explores Power Analysis side-channel Attacks, simple power analysis, low and high data complexity attacks (sub-classes of power analysis attacks) and the types of devices commonly targeted by such attacks ([microcontrollers](https://en.wikipedia.org/wiki/Microcontroller) and [ASIC](https://en.wikipedia.org/wiki/Application-specific_integrated_circuit)), [AES](https://en.wikipedia.org/wiki/Advanced_Encryption_Standard_process) power analysis attack.


### Lecture 6 - Power-EM Side Channels III

- [Simple power analysis on AES - Plan A](https://www.youtube.com/watch?v=x8WMxbpjdLQ&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=33) - Delving into 1 of 2 ways to performing a power analysis of AES. First, by capturing a power trace, then recovering the state bytes from that trace, and then using the state bytes to recover the key. (20 minutes);
- [Simple power analysis on AES - Plan B](https://www.youtube.com/watch?v=jvyTLZlNsHc&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=32) - Delving into the 2nd of 2 ways of performing a power analysis of AES. First, by capturing a power trace, then recovering the Hamming Weight from that trace, and then using the Hamming Weights to recover the key. (23 minutes);

The basic reading is Chapter 5 of the coursebook, from 5.10 The Advanced Encryption Standard, that explores the steps of AES and their leaky nature that can be used for a power analysis attack to recover the key.

### Guest Lecture [Part 1] - Stjepan Picek - CSI NN: Reverse Engineering of Neural Network Architectures Through Electromagnetic Side Channel
- [CSI NN(Reverse NN via EM) - part 1](https://www.youtube.com/watch?v=9gQlJZKCTrg&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=31) - An intro about how timing attacks can be used for reverse engineering machine learning modules to obtain sensitive information about the involved datasets (20 minutes);
- [CSI NN(Reverse NN via EM) - part 2](https://www.youtube.com/watch?v=Mn6J7LqWdWo&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=29) - Exploring which information is required to execute such attacks, and which operations in the model are targeted (22 minutes);
- [CSI NN(Reverse NN via EM) - part 3](https://www.youtube.com/watch?v=Vr7KXwLXUbA&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=30) - Delving into the reverse engineering process on a Neural Network (9 minutes);
- [CSI NN(Reverse NN via EM) - part 4](https://www.youtube.com/watch?v=zf9bZDUKq90&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=28) - Examining results of attacks (16 minutes);


### Guest Lecture [Part 2] - Stjepan Picek - Machine Learning and Implementation Attacks
- [SCA via Deep Learning - part 1](https://www.youtube.com/watch?v=XyXqInBYae4&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=27) - Discussing different types of profiled attacks and Neural Network architecture (19 minutes);
- [SCA via Deep Learning - part 2](https://www.youtube.com/watch?v=hWFG1TnAqWM&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=26) (16 minutes);


### Lecture 7 - High Data Complexity Attacks Power-EM I
[Textbook Link](https://orenlab.sise.bgu.ac.il/AttacksonImplementationsCourseBook/07_High_Data_Complexity_Power_EM_1)

- [Recap - Attacks on RSA](https://www.youtube.com/watch?v=kp4gv4icZ_c&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=23) - A recap of RSA and AES attacks (15 minutes);
- [Recap - Attacks on AES](https://www.youtube.com/watch?v=iWwzi1rqzYg&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=25) - A recap of RSA and AES attacks (13 minutes);
- [High data complexity Attacks](https://www.youtube.com/watch?v=RqC5hJnRo8k&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=24) - Discussing the main idea of high data complexity attacks (DPA/CPA) (15 minutes);
- [DPA With Vaizata](https://www.youtube.com/watch?v=sFQJfKHsWxY&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=22) - Revisiting the Vaizata method and how to use it with DPA (13 minutes);
- [DPA With Vaizata On AES](https://www.youtube.com/watch?v=XLnRHlx7vlk&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=18) (18 minutes);
- [DPA With Vaizata On AES - Result Analysis](https://www.youtube.com/watch?v=8A4VLm0Dfh0&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=20) - Vaizata with DPA demo - Examining the results (12 minutes);
- [DPA With Vaizata On AES - Matlab(part 1)](https://www.youtube.com/watch?v=cVl9su9Q6Lg&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=21) - Demonstrating Vaizata with DPA on Matlab (16 minutes);
- [DPA With Vaizata On AES - Matlab(part 2)](https://www.youtube.com/watch?v=TXESGYUDAWA&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=19) (19 minutes);

Basic reading is Chapters 7 and 8 of the Coursebook; Whereas chapter 5 mainly focused on low data complexity attacks (with few traces), chapter 7 focuses on high data complexity attacks, aka DPA and CPA (many, many traces). It revisits the Vaizata method and how it can be used for high data complexity attacks, similarly to timing attacks (this time the assumption is that the power consumption is depended on the key). At 7.2 we demonstrate an attack on AES using example data from the [Power Analysis Attacks book](https://link.springer.com/book/10.1007/978-0-387-38162-6) and visualize the process.

### Lecture 8 - Micro-Architectural Side Channels
[Textbook Link](https://orenlab.sise.bgu.ac.il/AttacksonImplementationsCourseBook/06_Cache_Attacks_Guest_Lecture)

- [Defining Micro-Architectural Attacks](https://www.youtube.com/watch?v=dFnHC6OH2H4&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=13) - Discussing Micro-Architecture attacks between processes (19 minutes);
- [The Cache - Hierarchy and Structure](https://www.youtube.com/watch?v=NJEgH9jgifA&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=12) - Discussing the need for caches, their structure, mapping policy and hierarchy (20 minutes);
- [Prime + Probe Cache Attack](https://www.youtube.com/watch?v=t4jxgga4XIQ&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=17) - An explanation of the Prime + Probe cache attack (9 minutes);
- [From Prime + Probe To Spectre](https://www.youtube.com/watch?v=cQ2-toh-kr0&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=15) - Demonstrating Spectre vulnerability using the Virgulator emulator (11 minutes);
- [Virgulator Redux - Execution Order](https://www.youtube.com/watch?v=XcJBSGFCoIw&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=14) - Discussing and demonstrating Virgulator Redux (15 minutes);
- [Spectre - Toy Example](https://www.youtube.com/watch?v=h-CEHjEkIm8&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=16) - Discussing the Spectre vulnerability (9 minutes);

Basic reading is chapter 6 of the coursebook that deals CPU Caches and Cache attack techniques; For further reading on cache attacks, see Colin Percival's [Cache Missing For Fun And Profit](http://css.csail.mit.edu/6.858/2014/readings/ht-cache.pdf); The chapter also introduces 2 main cache attack techniques: [Flush+Reload](https://www.usenix.org/conference/usenixsecurity14/technical-sessions/presentation/yarom) and [Prime+Probe](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7163050); For further reading about the hash function can be reverse engineered, see [Reverse engineering intel last-level cache complex addressing using performance counters. ](https://link.springer.com/chapter/10.1007%2F978-3-319-26362-5_3); Finally, there is a step-by-step Flush+Reload cache attack (as presented in Gruss, Spreitzer and Mangard's ["Automating attacks on inclusive last-level caches"](https://www.usenix.org/conference/usenixsecurity15/technical-sessions/presentation/gruss) and on Yarom and Faulkner's ["A high resolution, low noise, L3 cache side-channel attack"](https://www.usenix.org/conference/usenixsecurity14/technical-sessions/presentation/yarom) demonstration to retrieve the user's keystroke timestamps in a gedit program. The Github repository can be found [here](https://github.com/clementine-m/cache_template_attacks).

### Lecture 9 - Fault Attacks I
[Textbook Link](https://orenlab.sise.bgu.ac.il/AttacksonImplementationsCourseBook/09_Fault_Attacks)

- [Definition of Fault Attacks](https://www.youtube.com/watch?v=PSRZaFiDwy8&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=11) - Defining Fault Attacks, which are active attacks for extracting information from devices by breaking them (12 minutes);
- [Fault Attack Taxonomy](https://www.youtube.com/watch?v=9e0fCJMJpQY&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=9) - Further discussion of Fault Attacks, fault methods, and targets(25 minutes);
- [FA Example - Unlooper (1997)](https://www.youtube.com/watch?v=urrVGoVhC0s&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=10) - Discussing unloopers which were smartcards intended to cause the card to skip one or more instructions by applying a "glitch" in some form to the power or clock signal(8 minutes);

This lecture is based on chapter 9 of the coursebook "Fault Attacks", which is an active attack that allows the attacker to extract information from a device by breaking it. It goes on to discuss different kinds of fault methods (power supply attacks, timing attacks, temperature attacks, and more), further giving examples of classic fault attacks targeting the control flow: [Canon camera blinking](https://chdk.fandom.com/wiki/Obtaining_a_firmware_dump#Q._How_can_I_get_a_firmware_dump.3F), and [Unloopers](https://www.oocities.org/wild_lightning21/hardware/unlooper.htm). We then examine a fault attack on RSA-CRT as presented by Boneh and Lipton in [On the importance of eliminating errors in cryptographic computations](https://doi.org/10.1007/s001450010016); 

### Lecture 10 - Fault Attacks II
- [Introduction to the Biham-Shamir Fault Attack](https://www.youtube.com/watch?v=Kmx6huPoDJA&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=8) - Recap of Fault Attacks and introduction of Biham-Shamir Fault Attack (20 minutes);
- [Biham-Shamir Fault Attack Explained](https://www.youtube.com/watch?v=hFDZK5nVYGo&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=7) - Explanation of Biham-Shamir Fault Attack (20 minutes);
- [Introduction to The Boneh, DeMillo, Lipton Fault attack - RSA-CRT](https://www.youtube.com/watch?v=kkqEYy-fS0A&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=1) - Fault Attack on RSA-CRT, Chinese Remainder Theorem (20 minutes);
- [The Theory of The Boneh, DeMillo, Lipton Fault attack](https://www.youtube.com/watch?v=9i02fjm8EPI&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=3) - The Boneh, DeMillo, Lipton Facult Attack on RSA-CRT,  (11 minutes);
- [The Boneh, DeMillo, Lipton Fault attack in practice](https://www.youtube.com/watch?v=XLqseoch_wM&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=2) - Explanation of The Boneh, DeMillo, Lipton Facult Attack in Practice (15 minutes);
- [The Theory of Rowhammer](https://www.youtube.com/watch?v=yMdnAXTp_Q0&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=4) - Introduction of Rowhammer, DRAM, DRAM internals and Rowhammer Basics (17 minutes);
- [Rowhammer in Practice](https://www.youtube.com/watch?v=Smm9I-fyoWA&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=5) - Further discussion on the basics of Rowhammer, and explaining Rowhammer Exploit Code (14 minutes);
- [DVFS - Dynamic Voltage and Frequency Scaling](https://www.youtube.com/watch?v=VsWBeWmzs9s&list=UUKK5uxRGT-0Jtq1bGAg7XkQ&index=6) - Introduction of DVFSand explaining DVFS Fault Attacks (12 minutes);

This lecture is based on chapter 9 of the coursebook "Fault Attacks". Papers covered include Kim et al.'s ["Flipping bits in memory without accessing them: An experimental study of DRAM disturbance errors"](https://doi.org/10.1109/ISCA.2014.6853210), Razavi et al.'s ["Flip Feng Shui: Hammering a Needle in the Software Stack"](https://www.usenix.org/conference/usenixsecurity16/technical-sessions/presentation/razavi), Tang et al.'s ["CLKSCREW: Exposing the Perils of Security-Oblivious Energy Management"](https://www.usenix.org/conference/usenixsecurity17/technical-sessions/presentation/tang), Schmidt and Hutter's ["Optical and EM Fault-Attacks on CRT-based RSA: Concrete Results"](https://graz.pure.elsevier.com/en/publications/optical-and-em-fault-attacks-on-crt-based-rsa-concrete-results), Boneh DeMillo and Lipton's ["On the Importance of Eliminating Errors in Cryptographic Computations"](https://doi.org/10.1007/s001450010016), Murdock et al.'s ["Plundervolt: Software-based Fault Injection Attacks against Intel SGX"](https://www.plundervolt.com), and Biham and Shamir's ["Differential fault analysis of secret key cryptosystems"](https://doi.org/10.1007/BFb0052259).



## How To Compile The Handbook
### Windows
#### Toolchain Installation
1. Install MikTex from: https://miktex.org/download (with default settings). NOTE that although Tex Live is supposedly a decent alternative to MikTex on windows - attempts to use it for compiling the book failed miserably.
2. Install Perl from: http://strawberryperl.com/
3. [Optional but Recommended] Install VSCode and the **LaTeX Workshop** extension to be able to compile from VSCode.
4. [Optional but Recommended] Install the **LaTex language support** VSCode extension to ease editing in VSCode.
#### Full book Compilation
- From VSCode: open UniversityCourseBookAOI.tex, click on the "TEX" icon in the left sidebar, run the "Build LaTeX project" command.
- Without VSCode: run `latexmk` from the root directory of the book repository

Other operating systems: just run `latexmk`


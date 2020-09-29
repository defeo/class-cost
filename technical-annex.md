
# TECHNICAL ANNEX

## 1	S&T EXCELLENCE

### 1.1	Soundness of the Challenge 

Elliptic curves have been central to the development of number theory throughout the 20th century,
and of public-key cryptography in the 21st century.
Their interest and utility is beyond question.
Contemporary **Elliptic Curve Cryptography (ECC)**,
which is now ubiquitous in digital security (from the internet to smart cards),
represents a brilliant example
of effective exchange and collaboration
between researchers from pure mathematics (especially number theory and algebraic geometry),
computer science, and engineering.
Now, the new emergence of **isogeny-based cryptography**
requires us to strengthen, broaden, and re-focus this computational and mathematical exchange
for a renewed purpose:
this is the goal of the Action.


**Isogenies**
are algebraic mappings---essentially, nontrivial alebraic relationships---between elliptic curves.
Isogenies play the elliptic-curve role that matrices play in linear algebra:
they are fundamental to the study of elliptic curves.
Until recently, 
isogenies have played a minor and somewhat hidden role in ECC:
for example, they are crucial in the generation of secure ECC parameters
(in the SEA algorithm),
and they have also been used to map hard cryptographic problems between curves.
Indeed,
it has been possible for researchers to learn and work in ECC without knowing about isogenies.

In the past decade, however, 
a new generation of public-key **isogeny-based cryptosystems** has appeared,
rapidly gaining attention for their apparent resistance to 
adversaries equipped with quantum computers---a quality that classical ECC spectacularly lacks.
Here, isogenies emerge from the background to become the central objects.
Indeed, in isogeny-based cryptosystems,

- their *security* depends on the difficulty of reconstructing an unknown isogeny with classical and/or quantum computers;
- their *utility* depends on highly efficient algorithms and software for computing isogenies; and
- their proper *design and analysis* requires a deep understanding of the mathematical and algorithmic nature of isogenies.

Isogeny-based cryptography is the newest of the main paradigms in **post-quantum cryptography**,
but it has already found some success.
One early cryptosystem, SIKE, has progressed to the third round of the NIST post-quantum cryptography 
as an alternate candidate.

After this early success,
the challenge now facing us is to renew, strengthen, and enlarge
the collaboration between mathematicians, computer scientists,
and engineers that was fundamental to the success of ECC,
in order to better understand and establish the theory and practice of isogeny-based cryptography.

#### 1.1.1	DESCRIPTION OF THE STATE-OF-THE-ART

The beginning of isogeny-based cryptography (as we recognise it today)
goes back to 2006,
with the early public-key cryptosystems sketched by Stolbunov
and the isogeny-based hash function of Charles, Goren, and Lauter.
The first competitive cryptosystem was Jao and De Feo's SIDH (2009) 
post-quantum key exchange algorithm,
which became the basis of the SIKE key encapsulation mechanism (KEM)
submitted to the NIST post-quantum standardization process.
Early research on isogeny-based cryptosystems was mostly focused
on SIDH, its cryptanalysis, and its efficient implementation.

In recent years, however, Stolbunov's ideas have been revisited,
producing an explosion of new cryptosystems based on the nexus
of isogenies and class field theory.
The most notable such cryptosystem is CSIDH,
which promises to be the first post-quantum solution
for non-interactive key exchange.

However, the mathematical foundations of Stolbunov's cryptosystems and CSIDH
lend themselves to more detailed constructions.
In particular, 
we now have new and efficient isogeny-based digital signature schemes,
such as CSI-FiSh and SQISign,
as well as advanced cryptosystems
including threshold signatures and Verifiable Delay Functions.

SOA of cryptanalysis:

- Basic classical collision- and golden-collision-finding algorithms
- Quantum algorithms:
    - quantum isogeny evaluation
    - uncertain status of Kuperberg's algorithm etc
    - ...

SOA of supporting algorithms:
- Large class group computations

#### 1.1.2	DESCRIPTION OF THE CHALLENGE (MAIN AIM)

Main challenges:

- To grow and focus ECC-style collaboration
- To involve more number theorists
- To include engineers and computer scientists
- To include quantum algorithm specialists
- Protocol specialists

What we need to build together, and knowledge we need to share effectively:

- Improved algorithms for isogenies
- Construction of databases and basic formulae
- Large-scale computations for secure parameter generation and cryptanalysis
- Common understanding of quantum security


### 1.2	Progress beyond the state-of-the-art 

This action can be reasonably expected to make significant progress beyond the state-of-the-art in three main topics: constructing new protocols, cryptanalysis, and implementation.

We see above that isogenies have proven already to be flexible in their breadth of cryptographic applications: (non-interative) key exchange, signatures, VDFS, and more. 
However, many of the classical cryptographic protocols from later generations, for example using pairings, do not yet have efficient post-quantum analogues. We will have a focussed working group on number-theoretic foundations in order to explore further the potential for new post-quantum as well as classical applications of isogenies; such a study may also lead to improved algorithms for the current popular isogeny-based constructions.

With cryptanalysis it is especially important that the best classical and quantum algorithms to attack isogeny-based cryptosystems are well understood and pushed to their limits, as well as searching for new approaches. By the end of the action, we will have a unified stance on the classical and quantum security of SIKE and CSIDH, as well as more advanced protocols, and have a better understanding of the security of isogeny-based cryptography more generally. This will give much-needed confidence in the schemes before they are implemented on a wide-scale.

Secure and efficient implementation is a very active topic in isogeny-based cryptography. 
Through this action, by the careful creation of databases and coordination of work it will be possible to present secure and optimized implementations for not only the main protocols but also for new constructions. 

#### 1.2.1	APPROACH TO THE CHALLENGE AND PROGRESS BEYOND THE STATE-OF-THE-ART

Our approach to the challenge from the perspective of the network has two main foci: introducing young researchers to the main open problems while equipping them with the tools they will need, and bringing together researchers from different fields to learn from each others' different perspectives. 

Concretely, for the first aim we plan to hold a week-long school near the beginning of the action, 
and to create a book with chapters contributed by the lecturers of this school. The book will be maintained on an open source online platform with possibility for the future addition (or removal) of chapters until the end of the action, 
due to the fact that the topic is still changing rapidly, and will be formally published during the last year of the action.

For the second aim, 
we will bring together reseachers from different fields by means of both dedicate working groups and workshops. 
-For cryptanalysis, we will hold a dedicated workshop, with follow-up workshops focussed on aspects of (classical or quantum) cryptnalysis that prove to be of interest to the partners in the action. 
-For the development of new protocols, we have a dedicated working group on number-theoretic foundations.
-For implementation, we have dedicated working group, and we will also hold implementation focussed workshops throughout the action.
This will include a workshop dedicated to the creation of a database for isogeny formulas.

Finally, we will support Short-Term Scientific Missions, especially to foster research connections formed at the aforementioned workshops, throughout the entire action period.
These missions will be vital for the continuation of the research inspired by our workshops, and especially prioritise mobility for young researchers and participants who do not have access to alternate travel funding.

#### 1.2.2	Objectives

Although isogeny-based cryptography is still very much an emerging field, the time pressure of achieving post-quantum cryptographic standards
and the memory benefits of using isogeny-based cryptosystems are facilitating the possibility of relatively early wide-scale adoption of
isogeny-based cryptosystems. Our objectives, listed below, aim to mitigate the risk of early adoption where possible as well as develop a 
unified global outlook in the field. In particular, no one country involved in the Action (or indeed globally) has a critical mass of
isogeny-based cryptography researchers; a research network will facilitate regular discourse and collaboration between both the European and
international community. 

##### 1.2.2.1 Research Coordination Objectives

1. Lead a global discussion to develop a common understanding of both classical and quantum algorithms applied in cryptanalysis to isogeny-based cryptosystems. 

2. Develop the field of isogeny-based cryptography both by improving the understanding of the existing protocols and by developing new protocols.

3. Facilitate access to foundational knowledge in isogeny-based cryptography, both for early career researchers and newcomers to the field. This will include mathematical background, algorithms, and protocol design, and will be achieved for example through open-source articles, books, and databases. 

4. Provide input to international standardization bodies such as NIST and ETSI. For example, writing 'Requests for Comment' (RFCs), technical reports, and filing comments for the NIST post-quantum competition. 

5. Disseminate the work achieved through COST collaboartions by presenting at high-profile international cryptography conferences.

##### 1.2.2.2 Capacity-building Objectives

1. Grow the field of isogeny-based cryptography by fostering existing research conections. Most of the innovative papers in the field have resulted from multinational collaborations facilitated by ad hoc workshops or visits; a research network will allow for much more regular collaboration and consequently a rapid increase in high-quality research output.

2. The Action is by nature interdisciplinary. We will bring together researchers from cryptography, number theory, and quantum computing, all of whom have different perspectives on the major open problems in isogeny-based cryptography.

3. We will give collaboration opportunities and increased visibility to Early Career Investigators who would otherwise be isolated or limited to very few local collaborators by connecting them with the whole European isogeny-based cryptography community.

4. We will promote diversity in the community, for example by ensuring a diverse consortium and by collaboration with the Women in Numbers Europe community.

## 2	NETWORKING EXCELLENCE

TODO: ??

### 2.1	Added value of networking in S&T Excellence
#### 2.1.1	ADDED VALUE In relation to existing efforts at European and/or international level

Related networks:

- PQcrypto (https://pqcrypto.eu.org/)
- AlgANT (http://algant.eu/)
- Cryptography for Secure Digital Interaction (https://www.cost.eu/actions/IC1306/)
- CRYPTACUS (https://www.cost.eu/actions/IC1403/, https://www.cryptacus.eu/en/)
- WIN
- CIMPA?

### 2.2	ADDED VALUE OF NETWORKING IN IMPACT
#### 2.2.1	SECURING THE CRITICAL MASS AND EXPERTISE 
#### 2.2.2	INVOLVEMENT OF STAKEHOLDERS
#### 2.2.3	MUTUAL BENEFITS OF THE INVOLVEMENT OF SECONDARY PROPOSERS FROM NEAR NEIGHBOUR OR INTERNATIONAL PARTNER COUNTRIES OR INTERNATIONAL ORGANISATIONS

## 3	IMPACT

The aim of the Action is to expand the impact of isogenies on future
communication technologies. By creating the conditions to adopt,
safely and cost-effectively, isogeny-based protocols in future
communication protocols, the Action will positively impact the
competitiveness of SMEs and large companies in Europe and beyond.

The action will seek to maximise impact by disseminating results in
written form (books, academic papers, whitepapers, blog posts), and by
training a new generation of young researchers and engineers in the
fundamental tools of isogeny-based cryptography.


### 3.1	IMPACT TO SCIENCE, SOCIETY AND COMPETITIVENESS, AND POTENTIAL FOR INNOVATION/BREAK-THROUGHS

#### 3.1.1	SCIENTIFIC, TECHNOLOGICAL, AND/OR SOCIOECONOMIC IMPACTS (INCLUDING POTENTIAL INNOVATIONS AND/OR BREAKTHROUGHS)

NIST's eventual standardization of SIKE, possibly at some point within
the time frame of the Action, or shortly thereafter, is the first
clear impact factor tied to the Action. Through its published
analyses, the Action will aim at influencing NIST's decision
process. Two outcomes are possible: either the analyses shed doubt on
the security of SIKE, an unfortunate outcome, but a valuable
contribution to NIST and to society; or they confirm the strength of
SIKE, and possibly improve its performance, paving the way for
widespread adoption as well as growth in the sector of
post-quantum cryptography.

While the eventual standardization of SIKE will be an undeniable
booster for the popularity of isogeny-based cryptogrpahy, the Action
goals reach beyond NIST's competition and post-quantum
cryptography alone. 

Within the scope of post-quantum cryptography, the Action will 
explore many significant innovations, such as, for
example, efficient isogeny-based signature schemes, new advanced
primitives not currently known to be constructible from isogenies,
better provable security for already known primitives, and more
in-depth analyses of available attacks. Although on a longer
time-scale than SIKE, these innovations will directly benefit
stakeholders operating in the post-quantum space such as SMEs and
large companies offering encrypted products with long-term security.

Beyond post-quantum cryptography, the recently discovered "time delay
protocols" based on isogenies offer another opportunity for high
impact, providing cost-effective solutions to difficult problems in
distributed computing such as generation of fair randomness or
electronic voting. The primary beneficiaries of these technologies are
stakeholders working with blockchains, and more generally financial
services. The Action will advance the state-of-the-art of time delay
protocols, providing more powerful constructions, more efficient
protocols, and more secure instantiations.

Finally, in terms of scientific impact, the goal of the action is to
establish a common language and to reach a critical mass capable of
accelerating progress in isogeny-based cryptography. The various
actions described in the implementation section (workshops, schools,
books) will contribute to form a new generation of experts with a deep
understanding of isogeny-based cryptography, whose impact in the
broader field of cryptography ---both theoretical and applied--- will be felt
well after the Action is over.

### 3.2	MEASURES TO MAXIMISE IMPACT

#### 3.2.1	KNOWLEDGE CREATION, TRANSFER OF KNOWLEDGE AND CAREER DEVELOPMENT

Owing to its interdisciplinary nature, and to the wide range of skills
involved, the Action will alternate large meetings aimed at all
partners and smaller focused meetings gathering participants from one
or two Working Groups.

Concretely, the Action will be structured around yearly meetings, in
rotating locations, aimed at all participants and open to outside
researchers. The meeting will have both an educational component, in
the form of lectures, and a research one, in the form of contributed
talks, posters, and work sessions. To encourage outside participation,
the Action will seek to co-locate the meetings with related
conferences, e.g., Eurocrypt or ANTS. Lecturers will be encouraged to
write lecture notes, and the notes will be collected on the website of
the Action [Luca: or shall we try to publish proceedings?] 
[Chloe: nice idea, but do we want to promise that now already?]. Whenever
technically possible, measures will be taken to also encourage remote
participation; at a minimum, lectures will be recorded and made
available online shortly after the workshop.

Between yearly meetings, the action will organize smaller workshops or
schools focused on narrower topics, typically involving one or two
Working Groups. The workshops will primarily be targeted at Action
members, but will be open to anyone, within the capacity of the event.
Whenever feasible, these workshops will be organized in participating
Inclusiveness Target Countries, to facilitate participation of their
researchers. The format of the workshop will be decided by
the organizers, and will have to be validated by the Management
Committee.

Both for meetings and workshops, the
Action will strive to involve young researchers in their
organization, in particular from Inclusiveness Target Countries, to
encourage responsibility taking and network building.

A limited amount of Short-Term Scientific Missions and Conference
Grants will be reserved to encourage PhD students to visit other
institutions and develop scientific collaborations.


#### 3.2.2	PLAN FOR DISSEMINATION AND/OR EXPLOITATION AND DIALOGUE WITH THE GENERAL PUBLIC OR POLICY

Throughout the duration of the Action, the official website will serve as a one stop shop for all sorts of resources related to the Action. In particular, it will contain:

- News feeds, agenda, links to mailing lists and social media accounts providing informations on the Action's activities.

- A regularly updated blog (1 post per month on average at least) discussing scientific topics related to the action using an informal style.

- A database of all scientific publications in the field of isogeny based cryptography, both by Action members and non-members, searchable and downloadable in machine readable formats.

- Lecture material from the Action's meetings and workshops.

- Information on the management of the Action.

The website will be maintained for at least 4 years after the end of the action. We aim for it to become a standard source of information for the field, and be kept up to date in the long term.

In the last year of the Action, selected lectures from the schools, plus invited essays if necessary,
will be invited to become chapters of a book edited under the
supervision of the Action and published with an academic publisher.

The Action will disseminate its scientic discoveries through the usual academic channels. Gold open access will be the preferred publication model; fortunately, this is often the standard model in the appropriate communities. Should the action publish datasets (e.g., tables of polynomials, formulas, ...), these will be published according to open data practices. The action will generally not seek to establish patents, as these are typically considered a hindrance to the deployment of cryptosystems. Exceptions may be made when a member seeks to establish a "defensive patent"; in this case the member will be required to explicitly release the patent to the public domain royalty-free.

The Action will target strategic venues for its communications: major conferences and journals in cryptography and number theory, targeted workshops on post-quantum cryptography, and standardization body meetings. In particular, the Action will target the workshops regularly organized by NIST as part of the post-quantum competition, by submitting whitepapers and contributed talks.

Software produced by the Action will mostly consist of research software for demonstrative purposes, or contributions to open source computer algebra systems (e.g., PARI/GP, Sagemath, Oscar, ...). In both cases, the code will be published under standard open source licenses, such as the GPL. Occasionally, some of these software may be integrated in the products of the industrial partners of the Action. As a general rule, the open source license will still apply to the software; most companies in cryptography regularly work with open source software. If the open source license does cause a problem with an industrial partner however, the authors of the code may decide to grant an additional closed source license to the industrial partner.

Besides advancing the state-of-the-art, the action also aims at making isogeny-based cryptography accessible to as wide an audience as possible. The blog will be the primary communication medium targeted at the general public, and shall thus be rich in expository informal articles and links to further reading. A series of short introductory videos targeting Masters and PhD students will be recorded to complement the lectures given at schools.


## 4	IMPLEMENTATION
### 4.1	COHERENCE AND EFFECTIVENESS OF THE WORK PLAN
#### 4.1.1	DESCRIPTION OF WORKING GROUPS, TASKS AND ACTIVITIES

Due to its multidisciplinary nature, the Action brings together several communities with different expertise and vocabularies. The work plan will be structured around 4 Working Groups (WG), roughly corresponding to each of the communities. We describe the WG below.

**WG1 - Number theoretic foundations** This WG will be concerned with the mathematical foundations of isogeny-based cryptography, rooted in number theory and algebraic geometry. It will study the objects upon which cryptographic protocols are built, their generalisations and their algorithmic properties. In particular, it will research efficient algorithms for working with isogenies of elliptic curves and higher dimensional abelian varieties, the structure of isogeny graphs, and the algorithmic relationships with their endomorphism rings. Its outputs will inform the other working groups on the best algorithmic ways to reach their goals, and on the potential risks to security. From the other WG, it will draw inspiration for useful properties to look for in the algebraic objects.

**WG2 - Cryptanalysis** This WG will focus on algorithms to break the concrete schemes that have been proposed. It shares with WG1 an interest for algorithms to navigate isogeny graphs, however it approaches them from a cryptographic perspective, focusing on the security definitions and the minor details that make each system unique. Unlike other WGs, it will have a strong focus on quantum algorithms. Security reductions will also be an object of study of this WG, in collaboration with WG3. Its outputs will be used to set parameters for different security levels, in coordination with WG4.

**WG3 - Primitives, Protocols and Assumptions** This WG will research new primitives and protocols that can be built from isogenies. It will monitor the emergence of new primitives that have a potential to be built from isogenies, and inform other WGs in the hope of coming with a working proposal. It will construct new protocols (mostly advanced ones that go beyond encryption and signatures) using the available primitives, and seek to make them as efficient as possible in collaboration with WG4. Inspired by protocols in other subfields (e.g., lattice based cryptography), it will propose new isogeny-based assumptions upon which new protocols can be constructed, and assess their security in collaboration with WG1 and WG2.

**WG4 - Hardware & Software implementations** This WG will produce high efficiency implementations of isogeny algorithms and protocols, both in hardware and in software. It will discuss with WG2 to determine the most efficient parameters for a given security level. It will interact with WG1 to seek new theoretically efficient algorithms for isogeny computations, that translate into fast software and hardware.

[We need to say something about transversality, risk management, and how we make the WG talk to each other]

#### 4.1.2	DESCRIPTION OF DELIVERABLES AND TIMEFRAME

TODO: later

- book
- EFD extension
- classpol/modpol database
- security whitepaper on SIKE or CSIDH?

#### 4.1.3	Risk analysis and Contingency Plans
#### 4.1.4	GANTT Diagram

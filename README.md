## Theat modeling questions
* What are we working on?
* What can go wrong?
* What are we going to do about it?
* Did we do a good enough job?

## Threat modeling manifesto
* Values: Dont check boxes, fix issues. Cooperate and work rather than talk
* Principles: Frequent analysis, org scope.
  * Good patterns
    * systematic aproach
    * Informed creativity
    * varied viewpoint
    * useful toolkit
    * Theory into practice
  * Bad patterns
    * MC threat modeling
    * overcomplicating the problem

## Threat modeling videoes
* What are we working on? What could go wrong? What can we do about it? Did we do a good job?
* Flow diagrams help understanding what you have
* Fixing the treat should go in to your workflow just like any other programming.

## Podcast (Cheaters)

* Cheat-developers sell cheats for 40€+ subscription services
* a lot of infighting. Devs will sell each other out.
* Game devs act as double agents and buy cheats to fix it.
* Semi Illegal, mainly due to copyright. Illegal in some asian countries
* Stream proof (not visible while streaming)
* Some pros cheat

# Make-Belief Boogie man.

## SynergyFlow Analytics (SF Analytics)
* Bussines idea:
 * To help businesses of all sizes achieve peak operational performance by providing intuitive, data-driven insights and seamlessly integrated workflow solutions.

## 1) What are we working on?

### assets:
 * Skilled workforce (not a priority)
 * Intelectual propperty (High Priority)
  * Software (High)
  * Reserch for improving software (High)
 * Technological infrastructure (High Priority)
  * Cloud technology (High)
  * Data analysis tools (Medium)
 * Client relationships (High priority)
  * Relationships with clients and bussines partners
 * Financial recourses (Medium priority)
  * Funding and investment (Low)
  * Revenue streams (Medium) (can be compensated if temporarily down)
 * Brand reputation (High Priority)
  * Customer satisfaction

### Security already in place

* 2FA
* Change passwords every 2 months (16 char, symbols, big and small letters, numbers)
* Anti phishing training
* compartmentalized acces
* Limited acces to client data, mainly test using dummy data
* NDA (Strict)

<img width="731" height="432" alt="image" src="https://github.com/user-attachments/assets/cfdfeb72-3dda-4947-9950-e11ee918e27f" />

### Customer is king

#### What do we need to do for our customers?
* Update tool for newer versions
* Tech support (on site)
* Training to use systems

#### Interactions and customer view
* sales
* Tech support (using partners if far away)
* Training
* When interacting with our tools

## What can go wrong?

### STRIDE (https://www.youtube.com/watch?v=iGkX06sVFFM&list=PLCVhBqLDKoOOZqKt74QI4pbDUnXSQo0nf&index=9)
* Spoofing
 * Server recieves no cloud data unless it is from a trusted device connected to internal network and proven using MFA
 * Client server should only take information from a single source, our server, but if you can spoof or intercept this you could push a "baad" update
* Tampering
 * High risk if attacker gains acces. A baad update couid expose a lot of data.
* Repuditation
 * Everything we send and recieve should be logged (excluding sensitive data)
* Information disclosure
 * We cannot give client info as we don't have it
 * Bigest risk is client list leaking
* Denial of Service
 * Not a big issue as we operate localy for the client
 * Mainly prevents updates and new features from being pushed
* Elevation of Priviliges
 * Sholud be segmented well enough
 * If succsesfull on multiple segment simultainuously potentially disaterous.
 * Biggest risk is source code leaking making future attempts easier.

### Priority risks

* Spoofing to tamper with client servers (High) (Valuable due to amount of information)
* Acces to source code (medium) (Low emediate value not counting comptetetors) (High long term value for gaining furhter acces)
* Compromised updates (High) (Valuable due to amount of information)

### Are we targeted by anyone? Common attacks
We are unlikely to be targetted for political reasons and haven't made any enemies.

#### Common attacks
* Phishing
* Spoofing communications

### Bussines continuity
* Service being down has no emmediate downsides
* Important to not get compromised as that would ruin our bussines due to lack of trust

## What are we going to do about it?
* Enshure up to date encryption on updates sent to clients
* Clients will require a key from us for a package to be trusted, changes once a month, Unoque to each client. Only stored on our server and client server, requres manual updating once a year trough NinjaOne (Remote acces program with a lot of sequrity)
* Better compartmentalisation, only acces to the code you will be working on.
* More training for customers on cyber security.

## Did we do good enough?
* Hired penetration test firm to attempt to hack in to our systems
* Staffed security team constantly working on imporving security
* continious training of staff and clients.
* Next threat model to be made in 3 months

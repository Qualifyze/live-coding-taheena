<br />
<br />

<p align="center">
  <img src=".images/video-call.png" alt="qualifyze live coding challenge" width="80" height="80">
</p>


<h1 align="center">
  <b>
    Qualifyze Live Coding Challenge
  </b>
  <br />
  <h4 align="center"><small>Auditor Assignment System</small></h4>
</h1>

<br />

### Context

We are developing a system to manage and schedule audits for various suppliers, ensuring efficient use of our auditors and adherence to different client subscription levels. This solution aims to address typical scenarios where companies require timely and fair distribution of audit resources.

### Project Overview

The system will handle the scheduling of audits for a supplier company, "Supplier 4 Live," with the following requirements and constraints:

#### 1. **Auditor Availability**

- An auditor can audit only one site per day.
- We aim to distribute the audits proportionally among auditors to ensure fairness.

#### 2. **Subscription Levels**

Clients pay for different subscription levels, each with distinct commitments for audit report delivery:
    - **Essentials:** Report available no earlier than 4 weeks after the request, with a maximum wait time of 4 months.
    - **Advanced:** Report available no earlier than 3 weeks after the request, with a maximum wait time of 2 months.
    - **Premium:** Report published as soon as it is ready, with a maximum wait time of 4 weeks.

#### 3. **Performance Considerations**

Ensure the system can handle concurrent audit requests efficiently. The audit assignment logic should balance the load among auditors while adhering to subscription-level constraints.

### Challenge Description

You have been provided with the problem statement a few days in advance to familiarize yourself with the requirements and constraints. During the live coding session, which will last 90 minutes, your task is to design and implement a part of this system, focusing on:

#### **System Design:**

Design an architecture that supports the requirements above, using principles of hexagonal architecture and Domain-Driven Design (DDD). Ensure the system can manage auditor availability, client subscriptions, and audit scheduling.

#### **Implementation:**

Implement a feature to assign auditors to sites, ensuring that:

  - Each auditor audits only one site per day.
  - Audits are distributed proportionally among auditors.
  - Adherence to subscription-level constraints for report delivery.

#### **Additional Complexity:**

Implement a basic event management system to handle notifications for audit assignments and report deliveries. Consider concurrency issues that might arise from multiple audit requests and provide solutions to handle them efficiently.

### Example Scenario

- **Client:** "Farma World Champion SLU"
- **Supplier:** "Supplier 4 Live"
- **Subscription Levels:** Essentials, Advanced, Premium

The system should schedule audits as per the subscription level constraints and assign auditors proportionally while ensuring that no auditor is double-booked on any given day.

### Key Points to Address

- **Architecture Design:** Explain how you would organize the system using hexagonal architecture and DDD. Identify key aggregates, entities, and value objects.
- **Event Management:** Describe how you would implement event handling for notifications.
- **Concurrency and Performance:** Discuss how you would manage concurrency in audit assignments. Outline strategies to optimize system performance.

### Structure of the live coding and tips to be prepared

* You will be given with the problem statement a few days ahead of the live coding meeting. Read the problem statmente carefully specially to address possible questions related to the problem itself. We will answer all questions as long as they're not related to how to implement the solution to the problem.
* If you want to implement a complete / partial solution before the live coding call and want to come with something already built, it's fine for us. We will do the call around that and inspect the code you provide.
* You will be doing the live coding call along with one or two potential team mates in a pair-programming or mob-programming fashion (depending whether if we are one or two people along with you). You will be the main driver and we will support you in whatever we can. This means that _**we will be doing our best to make you feel the most comfortable we can**_, providing help, advice or whatever you need. Our goal is to evaluate your fit into the team so we will do our best in helping you shine your best version simulating a common team situation with potential team mates.
* We value simple solutions with simple code above all. Try to avoid rabbit holes as much as you can and if you feel that you are falling into one it's perfectly fine to stop going that way and try to go simpler. We really value this kind of demanding attitude. Having said that we know that this kind of interviews can be stressing, so if you we feel that you can go using another simpler way we will try to advice you.
* Some implementation details
  * The code will be in Typescript. If you're not familiar with it, we suggest you to take a quick look of the basic things. We do not demand Gurú-level skills, but the basic level to get going. We can cover gaps if you need help.
  * The framework will be **[NestJs](https://docs.nestjs.com/)** as provided in this repository. Same thing here, if you're not familiar with it we suggest you to take a quick look of the basic things (the **Overview** topics in the NestJs documentation). And we can cover gaps if you need help here.
  * The tools that we use to collaborate in the team are:
    * To host calls: **[Google Meet](https://meet.google.com/)**
    * To sketch diagrams: **[Miro](https://miro.com/)**
    * To do pair programming: **[Code With Me](https://www.jetbrains.com/code-with-me/)** from IntelliJ.
  * If you do not have any of those or you're not familiar with them, no worries. We will adapt to what you feel most comfortable with.
* Some other tips. For obvious reasons, they're not mandatory just a few suggestions from ours to have your mind and body as fresh as possible (all of the suggestions are proven to improve the freshness of body and mind).
  * Sleep well the day before. This will help you take better decisions.
  * If you are used to do sports / workout, we suggest you to do your workout before or the day before. This is proven to lower stress levels and improve focus.
  * Eat well before or the day before, as healthy as you can with no alcohol and no soft drinks, and with no ultra-processed food or the least possible. This is proven to enhance concentration, energy levels, mood, and sleep quality, thereby boosting mental performance.

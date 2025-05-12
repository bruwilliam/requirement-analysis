# Requirement Analysis in Software Development.

## Description
This repository will contain information related to gathering, analysis and elicitation of user requirements for software development projects.

## What is Requirement Analysis?
Requirements Analysis is the process of identifying, documenting, and validating the needs and constraints of stakeholders (users, clients, or business teams) to define what a software system must do. It ensures that developers build the right product by clarifying functionality, performance, security, and usability expectations.

### What is it's role in the software development life cycle?
Requirements analysis is a critical phase in the SDLC, typically occurring after feasibility studies and before system design. Its key roles include:

1. Bridges Business Needs & Technical Solutions<br>
Translates stakeholder expectations into clear, actionable software specifications.

2. Defines Scope & Objectives<br>
Identifies what the system should do (functional requirements). Specifies constraints like performance, security, and compliance (non-functional requirements).

3. Reduces Development Risks<br>
Uncovers ambiguities, conflicts, or missing requirements early. Prevents feature creep (uncontrolled addition of features) by setting priorities.

4. Forms the Basis for Design & Testing<br>
Developers use requirements to architect the system. QA teams rely on them to create test cases (e.g., acceptance criteria).

5. Supports Project Planning<br>
Helps estimate time, cost, and resources needed. Enables better sprint planning in Agile methodologies.

## Why is Requirement Analysis Important?
### 1. Ensures Alignment with Business & User Needs
- Why it matters: Misunderstood or vague requirements lead to software that doesn’t solve the intended problem.

- Impact:

  - Prevents wasted effort by clarifying what the system must do (e.g., "Users need a one-click checkout" vs. assumed features).

  - Bridges gaps between stakeholders (clients, users, developers) through documentation like SRS (Software Requirements Specification).

- Example: A banking app without proper requirement analysis might miss critical fraud detection features, leading to security risks.
### 2. Reduces Cost & Rework
- Why it matters: Fixing errors in later phases (e.g., development or testing) is 5–100x more expensive than fixing them during requirements analysis (IBM Systems Sciences Institute).

- Impact:

  - Identifies conflicts, ambiguities, or missing requirements early (e.g., "Does ‘fast’ mean 1-second or 5-second response time?").

  - Avoids scope creep (uncontrolled feature additions) by prioritizing needs (e.g., MoSCoW method: Must-have vs. Nice-to-have).

- Example: A poorly analyzed e-commerce requirement might lead to rebuilding the payment gateway mid-project, increasing costs.


### 3. Forms the Foundation for Design & Testing
- Why it matters: Developers and testers rely on requirements to build and validate the system.

- Impact:

  - Guides system architecture (e.g., microservices vs. monolith based on scalability needs).

  - Enables accurate test cases (e.g., "Verify login works with 10,000 concurrent users" for non-functional requirements).

- Example: A social media app’s requirement for "real-time notifications" dictates the choice of WebSockets over HTTP polling.

## Key Activities in Requirement Analysis.
- Requirement Gathering
  - What: Collecting high-level needs from stakeholders (clients, users, regulators).
  - How: Interviews, surveys, market research.
  - Goal: Identify what the system should achieve (e.g., "Users need secure login").
- Requirement Elicitation
  - What: Extracting detailed, actionable requirements through collaboration.
  - How: Workshops, brainstorming, prototyping.
  - Goal: Uncover hidden needs (e.g., "Login must support 2FA").
- Requirement Documentation
  - What: Structuring requirements into clear, standardized formats.
  - How: SRS (Software Requirements Specification), user stories, use cases.
  - Goal: Create a single source of truth for developers/testers.
- Requirement Analysis and Modeling
  - What: Refining requirements for feasibility and consistency.
  - How: Diagrams (UML, BPMN), prioritization (MoSCoW).
  - Goal: Resolve conflicts and define how the system will work.
- Requirement Validation.
  - What: Ensuring requirements align with stakeholder expectations.
  - How: Reviews, walkthroughs, acceptance criteria checks.
  - Goal: Confirm the right system is being built before coding begins.
 
  ## Types of Requirements.
  ### Functional Requirements.
  Functional requirements define the specific actions, behaviors, and capabilities a software system must perform to meet user and business needs. They describe what the system should do and are typically expressed as inputs, operations, and expected outputs.<br>
**Key Characteristics**
  - Action-Oriented – Specify tasks the system must execute (e.g., "User can reset password").
  - Testable – Must have clear pass/fail criteria (e.g., "System sends confirmation email after signup").
  - User-Focused – Often phrased as features (e.g., "Search bar filters products by price range").
    
  For example, for the airbnb system;
  - The guests/visitors should be able to search for available hotels.
  - Hotel management should get a notification when a hotel room is available.
  ### Non functional Requirements.
  Non-functional requirements (NFRs) define the quality attributes, constraints, and performance standards of a software system. They describe how the system should behave rather than what it should do (unlike functional requirements). NFRs ensure the system is reliable, scalable, secure, and user-friendly.

**Key Characteristics**
  - System-Wide Impact – Affect the entire system, not just individual features.
  - Measurable – Often quantified (e.g., "Response time < 2 seconds").
  - Critical for UX & Stability – Poor NFRs lead to slow, insecure, or hard-to-maintain software.

For example, for the airbnb system;
The booking server should request for recent data through reddis.

## Use Case Diagrams.
Use case diagrams are a type of UML (Unified Modeling Language) diagram that visually represents the interactions between users (actors) and a system to achieve specific goals. They help capture functional requirements in a simple, high-level way.<br>

Key Components
- Actors
  - Roles interacting with the system (e.g., User, Admin, Payment Gateway).
  - Represented as stick figures.
- Use Cases
  - Actions/functionalities the system provides (e.g., Login, Process Order, Generate Report).
  - Drawn as ovals.
- Relationships
  - Associations (lines between actors and use cases).
  - Includes/Extends (for reusable or conditional behaviors).<br>

Benefits
- Simplifies complex systems.
- Identifies missing requirements.
- Guides development and testing.

![Use case diagram for the airbnb_clone project] (Images/alx-booking-uc.png)

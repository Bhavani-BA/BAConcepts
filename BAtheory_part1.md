# 
## Day 4 — Business Analyst Interview Preparation
## syllabus
### OOA, OOD and Enterprise Analysis
- Object-oriented approach
- Classes, objects, attributes and methods
- Encapsulation, abstraction, inheritance and polymorphism
- Object-Oriented Analysis (OOA)
- Object-Oriented Design (OOD)
- Enterprise analysis
- Business needs and objectives
- Current-state and future-state analysis
- Feasibility analysis
- Solution options analysis
- Requirement analysis and prioritisation
- MVC architecture
- PLODATT framework — expansion to be verified from your training material
- Gap analysis and impact analysis

  
  ## Object-Oriented Approach
  
 # What is it?
   The object-oriented approach is a way of developing a system by organising it around objects that represent real-world things.

## An object has:
- Data (attributes): Information about it.
- Behaviour (methods): Actions it can perform.
- Hospital appointment example


- # BA role OOA
- ## What does a BA do here?
- 
   As a Business Analyst, you help identify:
1. What users and business stakeholders need.
2. Which important objects the system must represent.
3. What information each object needs.
4. What actions users need to perform.
5. What business rules the system must follow

# 2. OOA — Object-Oriented Analysis

## What is OOA?
     OOA stands for Object-Oriented Analysis.

  It focuses on understanding the business problem and identifying the objects, their responsibilities and their relationships.

 In simple words:

OOA asks: What does the business need?

 Example
A hospital currently accepts appointments through phone calls. Patients complain that they cannot easily find available doctors or appointment slots.

As a BA, you speak with patients, receptionists, doctors and hospital management.

# You identify:
- Patient
- Doctor
- Appointment
- Payment
- Notification
- 
# You also identify business rules:

- A patient must be registered before booking.
- A doctor must have an available slot.
- A slot cannot be booked by two patients at the same time.
- A successful booking must generate confirmation.
These findings contribute to the analysis of the required system.

# Typical OOA activities
1. Understand the business problem.
2. Gather and analyse requirements.
3. Identify objects and their responsibilities.
4. Identify relationships between objects.
5. Identify business rules and system interactions.
6. Model requirements using appropriate diagrams, such as use case and class diagrams.
Important: OOA is not the same as coding. It is primarily about analysing the problem and the requirements.


## What is OOD
. OOD — Object-Oriented Design

 It focuses on how the system should be structured to satisfy the requirements identified during analysis.

 In simple words:

OOD asks: How should the system be designed?

# Example
  During OOA, you identify that patients must book and cancel appointments.

  During OOD, the technical team may design:
- The classes and their attributes.
- The methods that each class needs.
- How classes communicate.
- How the system checks slot availability.
- How the booking service communicates with the payment gateway.
- How the system handles errors and failed payments.
- 
- # 4. Object-Oriented Concepts
- 
- ##  Class
- A class is a blueprint for creating objects.

 Example:
Patient is a class that defines the information and actions associated with patients.

## Object
An object is a specific instance of a class.

 Example:
A registered patient with Patient ID P101 is an object of the Patient class.

# Remember:
- Class = blueprint.
- Object = actual instance

- # Encapsulation
- 
     Encapsulation combines data and the methods that operate on it, while controlling access to internal information.

## Hospital example:
    A payment system should protect sensitive payment information and allow access only through authorised operations.

# As a BA,
you might document security requirements such as:

- Only authorised users can view payment details.
- Sensitive information must be protected.
- Access to patient records must follow the hospital’s security policies.
Encapsulation is a software design concept; it is not simply displaying a password as asterisks.

## Abstraction

   Abstraction exposes the functionality a user needs while hiding unnecessary implementation details.

# Example:
A patient clicks Pay Now. The patient does not need to understand all the internal communication between the hospital system, payment service and bank.

  The BA should specify what the user must see and what the system must do, including successful and failed payment scenarios.
  
## Inheritance

   Inheritance allows one class to reuse or extend the characteristics of another class.

# Example:
Suppose a hospital system has a general Appointment class. InPersonAppointment and TeleconsultationAppointment could extend it.

     The general appointment information might include appointment ID, date and status, while each specialised appointment could have additional details.

   This is a possible design choice, not a requirement for every hospital system.
   
## Polymorphism

Polymorphism allows the same operation or interface to behave differently depending on the object or implementation.

# Example: 
A system may support a common processPayment() operation, while different payment providers implement the operation differently.


## Enterprise analysis
Helps an organisation understand its business needs, objectives, problems and opportunities before selecting a solution.

# for example
In a pharmaceutical vaccination project, the business objective may be to reduce employee absenteeism. I would understand the existing absenteeism process, analyse the baseline data, identify the desired future state and define KPIs to measure success.

Based on the analysis, the business can evaluate suitable solutions and estimate their costs, benefits and feasibility.

# Feasibility analysis

   Helps determine whether a proposed solution is practical.

          I would consider technical, economic, operational and schedule feasibility. For example, before implementing an online hospital appointment system, I would help assess whether the existing system supports integration, whether the cost is justified, whether staff can adopt the process and whether the project can meet its deadline.

          I would document the findings and risks so that stakeholders can make an informed decision.

# 7. Solution Options Analysis

# What does it mean?
  Solution options analysis means identifying and comparing different ways to solve a business problem.

   A BA should not immediately assume that developing new software is the only solution.
   
# How should a BA compare the options?

Consider:
1. Business benefits.
2. Implementation cost.
3. Technical feasibility.
4. Delivery time.
5. User experience.
6. Security and compliance.
7. Integration with existing systems.
8. Maintenance and support.
The BA documents the comparison and helps stakeholders understand the trade-offs.

# Interview point:
   The best solution is not always the most technically advanced one. It is the option that best meets the business objectives within the    relevant constraints.

#  Requirement Analysis and Prioritisation

 This is one of the most important Day 4 topics.
 
# Requirement analysis

Requirement analysis means examining requirements to ensure they are clear, complete, consistent, feasible and testable.

# Characteristics of a good requirement
  A good requirement should be:
  
- # Clear:
- Easy to understand.
- # Complete:
- Contains the information needed to understand it.
- # Consistent:
-  Does not conflict with other requirements.
  # Feasible: 
  Can realistically be implemented.
- # Testable:
-  Can be verified through testing.
- # Traceable:
-  Can be linked to its source and related work.
- 
# Requirement prioritisation
# using MOSCOW 

 [ ] Requirement analysis involves reviewing requirements to ensure they are clear, complete, consistent, feasible and testable.

- [ ] Requirement prioritisation determines which requirements should be implemented first based on business value, risk, dependencies, cost and stakeholder needs.
- [ ] 
- [ ] For example, in a hospital appointment system, preventing double-booking is essential, whereas customising the screen theme may be a lower-priority enhancement. I can use the MoSCoW technique to classify requirements as Must have, Should have, Could have and Won't have this time.
- [ ] 
- [ ] If stakeholders disagree, I facilitate discussion, assess the business impact and document the agreed decision.

 # MVC Architecture
 # What is MVC?
    MVC stands for Model–View–Controller.

     It is a software architectural pattern that separates an application's data,
     user interface and request-handling logic.
The application displays the result, such as booking confirmation or a message that the selected slot is no longer available.

This is a simplified explanation. The actual responsibilities can vary depending on the system design.

# Why is MVC useful?

- Separates responsibilities.
- Makes the system easier to maintain.
- Helps organise the application structure.
- Allows interface changes without necessarily changing the underlying business rules.
- Supports more organised development and testing.

# What is the BA's role in MVC?

 A BA is not necessarily responsible for implementing MVC.

The BA should understand the architecture well enough to communicate requirements and collaborate with the technical team.

For example,
the BA documents:
- What the patient should see on the booking screen.
- What validation is required.
- What business rules determine slot availability.
- What confirmation or error messages should appear.     

# 0. Gap Analysis

# What is gap analysis?
Gap analysis compares the current state (AS-IS) with the desired future state (TO-BE) to identify what is missing or needs to change.
Example: Hospital appointment system

Current state — AS-IS
- Patients book appointments by telephone.
- Receptionists manually check doctor availability.
- Patients may wait on hold.
- Appointment reminders are sent manually.
- 
Future state — TO-BE
- Patients can book appointments online.
- Available slots are displayed automatically.
- The system prevents double-booking.
- Appointment reminders are sent automatically.

# Steps in gap analysis
1. Understand the current process.
2. Define the desired future process.
3. Compare the two.
4. Identify gaps and their causes.
5. Recommend possible changes.
6. Prioritise the changes.
7. Document and validate the findings with stakeholders.
Remember: Gap analysis identifies what is missing. It does not automatically determine the final solution.

# Impact Analysis

 # What is impact analysis?
   Impact analysis determines how a proposed change may affect existing requirements, 
   systems, processes, users, costs, risks and timelines.

Example

   The hospital has an appointment booking system. The business requests a new feature: patients should be able to cancel appointments online.

   As a BA, you must investigate the impact before the change is approved.

   Impact analysis helps identify the effects of a proposed change on existing requirements, systems, processes, stakeholders, cost and timeline.

For example, if a hospital wants to introduce online appointment cancellation, I would assess the impact on appointment availability, payment refunds, notifications, reporting and testing.

I would document the affected requirements, dependencies, risks and estimated effort, then discuss the findings with the relevant stakeholders before the change is approved.

#  Strategy Analysis
Strategy analysis helps an organisation understand its current business situation and determine what changes are needed to achieve future business objectives.

Example: A hospital wants to reduce patient waiting time by introducing online appointment booking.

As a BA, you:
- Understand the business objectives.
- Analyse the current situation.
- Identify business needs.
- Define the future state.
- Identify risks and possible solutions.
- 
#  Root Cause Analysis
Root Cause Analysis (RCA) identifies the actual reason behind a problem instead of just treating its symptoms.

Example:

Problem: Patients are frequently missing appointments.

Possible reasons:
- Patients forget appointment dates.
- No SMS reminders are sent.
- Patients cannot easily reschedule.
- Appointment confirmation is unclear.
The BA investigates the underlying cause before recommending a solution.

# Fishbone Diagram

Fishbone is also called the Ishikawa diagram or Cause-and-Effect diagram.

It helps identify and organise possible causes of a problem.

# Common categories:
- People
- Process
- Technology
- Environment
- Methods
- Materials
- 
Example: If hospital appointment delays are the problem, the BA can investigate whether the causes relate to staff shortages, manual processes, system failures or poor scheduling

# What is Zachman Framework?

The Zachman Framework is an enterprise architecture framework that organises information about an organisation from different perspectives.

It helps understand how business processes, data, people, locations, timing and business objectives are connected.

The Zachman Framework is an enterprise architecture framework that organises business and technology information using six questions: 

# What, How, Where, Who, When and Why.

For example, in a hospital management system, What represents patient data, How represents appointment booking processes, Who represents patients and doctors, and Why represents the business objective of reducing waiting time.

It helps understand the organisation from different perspectives.

#   Decision Analysis

# What is Decision Analysis?

  Decision Analysis is the process of evaluating different alternatives and 
  selecting the most suitable option based on business needs, cost, risks and benefits.

  BA responsibilities
1. Identify available options.
2. Understand stakeholder expectations.
3. Compare cost and benefits.
4. Assess feasibility and risks.
5. Identify dependencies.
6. Document the comparison.
7. Present findings to decision-makers.

# . Business Requirements Management

# What is Business Requirements Management?
   It involves managing business requirements throughout their lifecycle, 
   from identification and documentation through approval, changes and traceability.

   In BABOK, the closely related knowledge area is called Requirements Life Cycle Management.

# Important documents and tools
- BRD / requirement documentation.
- RTM (Requirements Traceability Matrix).
- Change Request Log.
- Jira.
- Confluence.
- Requirement Sign-off document.

- Business Requirements Management involves managing requirements throughout their lifecycle, including documentation, validation, approval, traceability and change management.

For example, 
If a hospital initially requests online appointment booking and later adds online cancellation, I would document the change, assess its impact, update the requirements and RTM, obtain stakeholder approval and communicate the changes to the development and testing teams.  

# Requirement Validation

# What is Requirement Validation?
    Requirement validation ensures that the documented requirements correctly
    represent the business needs and will help achieve the expected business objectives.

In simple words:

Are we building the right solution for the business?
Example
Business objective: Reduce patient waiting time.

Requirement: Patients should be able to view available doctor slots and book appointments online.

As a BA, you validate:
- Does this requirement address the business problem?
- Does it meet patient and hospital expectations?
- Is it aligned with the business objective?
- Have the relevant stakeholders agreed?
- Are there missing business rules?

# Requirement Validation ensures that documented requirements meet business needs and support the expected business objectives.

For example,
If a hospital wants to reduce patient waiting time, I would review the online booking requirements with patients' representatives, receptionists and hospital management to confirm that the proposed functionality addresses their needs.

I would resolve gaps, confirm stakeholder agreement and obtain approval before moving forward.

   



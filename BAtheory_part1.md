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

  # Question
  ## Object-Oriented Approach
  
 # What is it?
   The object-oriented approach is a way of developing a system by organising it around objects that represent real-world things.

## An object has:
- Data (attributes): Information about it.
- Behaviour (methods): Actions it can perform.
- Hospital appointment example

- # Question
- ## BA role OOA
- ### What does a BA do here?
As a Business Analyst, you help identify:
1. What users and business stakeholders need.
2. Which important objects the system must represent.
3. What information each object needs.
4. What actions users need to perform.
5. What business rules the system must follow

# Question
## 2. OOA — Object-Oriented Analysis
### What is OOA?
     OOA stands for Object-Oriented Analysis.

  It focuses on understanding the business problem and identifying the objects, their responsibilities and their relationships.

# In simple words:

OOA asks: What does the business need?

# Example
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
Typical OOA activities
1. Understand the business problem.
2. Gather and analyse requirements.
3. Identify objects and their responsibilities.
4. Identify relationships between objects.
5. Identify business rules and system interactions.
6. Model requirements using appropriate diagrams, such as use case and class diagrams.
Important: OOA is not the same as coding. It is primarily about analysing the problem and the requirements.

# Question
## What is OOD
. OOD — Object-Oriented Design

# What is OOD?
 OOD stands for Object-Oriented Design.

 It focuses on how the system should be structured to satisfy the requirements identified during analysis.

# In simple words:

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
- ##  Class
- A class is a blueprint for creating objects.

## Example: Patient is a class that defines the information and actions associated with patients.

### Object
An object is a specific instance of a class.

# Example: A registered patient with Patient ID P101 is an object of the Patient class.

# Remember:
- Class = blueprint.
- Object = actual instance

- # Encapsulation
- 
     Encapsulation combines data and the methods that operate on it, while controlling access to internal information.

## Hospital example:
    A payment system should protect sensitive payment information and allow access only through authorised operations.

# As a BA, you might document security requirements such as:

- Only authorised users can view payment details.
- Sensitive information must be protected.
- Access to patient records must follow the hospital’s security policies.
Encapsulation is a software design concept; it is not simply displaying a password as asterisks.

## Abstraction

   Abstraction exposes the functionality a user needs while hiding unnecessary implementation details.

# Example: A patient clicks Pay Now. The patient does not need to understand all the internal communication between the hospital system, payment service and bank.

  The BA should specify what the user must see and what the system must do, including successful and failed payment scenarios.
  
## Inheritance

   Inheritance allows one class to reuse or extend the characteristics of another class.

# Example: Suppose a hospital system has a general Appointment class. InPersonAppointment and TeleconsultationAppointment could extend it.

     The general appointment information might include appointment ID, date and status, while each specialised appointment could have additional details.

   This is a possible design choice, not a requirement for every hospital system.
   
## Polymorphism

Polymorphism allows the same operation or interface to behave differently depending on the object or implementation.

# Example: A system may support a common processPayment() operation, while different payment providers implement the operation differently.




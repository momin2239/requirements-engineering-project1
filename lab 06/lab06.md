
# Week 6 – UML Class Diagrams

## Part A – Reviewing Previous Models

This lab uses the College Equipment Booking System. The Class Diagram shows the main concepts in the system and how they are related.

### Task A1

1. FR01 shows that Booking is an important concept because students can make more than one booking.
2. FR03 identifies two Booking attributes: start date and end date.
3. FR04 and FR05 show relationships involving Staff Member. Staff review booking requests and manage equipment availability.

## Part B – Identifying Domain Concepts

### Task B1 – Candidate Concepts

| Candidate | Type | Supporting Requirement |
|---|---|---|
| Student | Class | FR01 |
| Booking | Class | FR01, FR02, FR03 |
| Start date | Attribute | FR03 |
| Equipment | Class | FR02, FR05 |
| Review | Action | FR04 |
| Staff Member | Class | FR04, FR05 |

### Task B2 – Main Classes

- **Student:** A student can make equipment bookings.
- **Booking:** A booking records the details of an equipment request.
- **Equipment:** This represents the equipment that students can book.
- **Staff Member:** Staff members review bookings and manage equipment availability.

### Task B3 – Unconfirmed Information

A student's email address could be useful for the system, but it is not mentioned in the requirements. The relevant college stakeholder should confirm whether this information is needed.

## Part D – Attributes and Associations

### Task D1 – Booking Attributes

The Booking class includes:
- startDate
- endDate
- status (candidate – confirmation required)

### Task D2 – Associations

| Class 1 | Relationship | Class 2 | Requirement |
|---|---|---|---|
| Student | makes | Booking | FR01 |
| Booking | identifies | Equipment | FR02 |
| Staff Member | reviews | Booking | FR04 |
| Staff Member | manages availability of | Equipment | FR05 |

## Part E – Multiplicity

### Task E1

Each Booking identifies exactly one Equipment item. Therefore, the multiplicity at the Equipment end is **1**.

### Task E2 – Open Multiplicity Questions

| Association | What needs clarification? |
|---|---|
| Student – Booking | Does every booking belong to exactly one student? Can a student have zero bookings? |
| Booking – Equipment | How many bookings can refer to the same equipment item over time? |
| Staff Member – Booking | Can one or several staff members review a booking? |
| Staff Member – Equipment | Can several staff members manage the same equipment? |

### Task E3 – Open Questions

1. Can more than one staff member review the same booking?
2. Can the same equipment item be booked by different students at different times?
3. Does each booking belong to exactly one student?

## Part F – Reviewing the Class Diagram

### Task F1 – Requirements-to-Model Check

| Requirement | Representation | Result |
|---|---|---|
| FR01 | Student – Booking relationship | Yes |
| FR02 | Booking – Equipment relationship and multiplicity 1 | Yes |
| FR03 | startDate and endDate attributes | Yes |
| FR04 | Staff Member – Booking relationship | Yes |
| FR05 | Staff Member – Equipment relationship | Yes |
| FR06 | Booking status / approval decision | Needs clarification |

### Task F2 – Comparing Previous Models

The Class Diagram is consistent with the earlier Use Case and Activity Diagrams. It includes the main concepts involved in creating and reviewing an equipment booking. Some details, especially the multiplicities and booking approval status, still need clarification.

## Part G – Campus Workshop Registration

### Task G1 – Main Classes

- Student
- Workshop
- Registration

### Task G2 – Attributes

| Class | Attributes |
|---|---|
| Student | studentID, name |
| Workshop | workshopCode, title |
| Registration | registrationDate, status |

### Task G3 – Associations

- Student has Registration.
- Registration is for Workshop.

### Task G4 – Multiplicities

- One Student can have zero or many Registrations (0..*).
- Each Registration belongs to exactly one Student (1).
- One Workshop can have zero or many Registrations (0..*).
- Each Registration is for exactly one Workshop (1).

### Task G5 – Interpretation

1. One Student can have zero or many Registration records.
2. Each Registration belongs to exactly one Student.
3. One Workshop can have zero or many Registration records.
4. Each Registration is for exactly one Workshop.

## Part H – Individual Project

**Project: College Student Support Appointment System**

### Task H1 – Candidate Domain Concepts

1. Student – the person requesting support.
2. Support Appointment – the appointment requested by a student.
3. Support Staff Member – the person providing support.
4. Support Service – the type of support being requested.

These are initial candidate concepts and should be checked against the project's existing requirements.

### Task H2 – Possible Associations

- Student requests Support Appointment.
- Support Staff Member handles Support Appointment.
- Support Appointment relates to Support Service.

### Task H3 – Multiplicity

The exact multiplicities should be checked against the documented project requirements before being confirmed.

### Task H4 – Open Question

Can a student have more than one support appointment, and can the student request appointments with different support staff members?


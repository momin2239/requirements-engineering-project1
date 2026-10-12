# 1. Information from Week 2

In Week 2, we learned that using spreadsheets and emails to manage equipment can cause problems. Sometimes, two people may book the same item because the information is not updated properly. It can also be difficult to know if a camera or projector is available. Technicians spend a lot of time checking bookings manually.

# 2. Candidate Requirements

* **E:** Assumption
* **F:** Stakeholder need or concern

# 3. Requirements Surgery

### Requirement 1: The system shall be user-friendly.

**A. Problem / observation:**
The term "user-friendly" is not clear because different people may understand it differently.

**B. Stakeholder need / concern:**
Students and staff need a system that is easy to understand and use.

**C. Candidate requirement:**
The system shall allow users to make a booking without unnecessary steps.

**D. Solution idea:**
Use a simple layout with clear instructions and an easy booking process.

**Question:** How easy should the system be to use, and how many steps should a booking take?

**Missing information:** We need to know who will use the system and how many steps should be allowed when making a booking.

### Requirement 2: The system shall notify users about bookings.

**Problem:**
The requirement does not explain how users will receive notifications or when they will be sent.

**Question:** Should notifications be sent by email or displayed inside the system?

**Missing information:** We need to confirm the notification method and when users should receive reminders.

### Requirement 3: The system shall allow staff to create, edit and delete bookings and send reminders.

**Problem:**
This requirement includes several actions in one sentence, which makes it harder to understand and test.

**Question:** Which staff members are allowed to delete bookings made by other users?

**Missing information:** We need to know the permissions for each staff role and when reminders should be sent.

> * please note that I used AI to design this way of written in the following question based on mu answers
> * thank you for understanding*

# 4. Functional Requirements

| ID    | Requirement                                                                            | Source               | How could we check it?                                                                                  |
| ----- | -------------------------------------------------------------------------------------- | -------------------- | ------------------------------------------------------------------------------------------------------- |
| FR-01 | The system shall allow users to check which equipment is available on a selected date. | Worked example       | Log in, select a date, and check whether the available equipment is displayed correctly.                |
| FR-02 | The system shall allow technicians to approve or reject booking requests.              | Technician need      | Create a booking request and check whether a technician can approve or reject it and change its status. |
| FR-03 | The system shall save the expected return date and time for each booking.              | Equipment management | Make a booking and check that the correct return date and time are saved.                               |

# 5. Quality Requirements

| ID     | Quality requirement                                                                          | Why does it matter?                                            | How could we check it?                                                                               |
| ------ | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| NFR-01 | The system shall require users to log in with their college account before making a booking. | This helps prevent unauthorised people from booking equipment. | Try to make a booking without logging in and check whether the system asks the user to log in first. |

# 6. Applying the Requirements Process to the Project

**Candidate requirement:** The system shall allow students to borrow laptops for up to three days.

**Step 1 – Source:**
This requirement comes from student feedback and the IT helpdesk staff.

**Step 2 – Examination:**
This is a functional requirement because it describes what the system should allow students to do. However, it does not explain whether students can extend their booking.

**Step 3 – Verification:**
Create a test student account and try to book a laptop for three days. Then try to book it for four days to check whether the system prevents bookings that exceed the limit.

**Step 4 – Unknown information:**
We still need to know what happens if a student returns a laptop late. We should ask the IT supervisor about the rules for late returns.

# 7. Reflection

**1. What makes a requirement difficult to understand?**

A requirement can be difficult to understand when it uses unclear words such as "fast" or "easy" without explaining what they mean. It can also be confusing when several different actions are included in one sentence.

**2. What information do you still need for your project?**

We need to find out how many items a student can borrow at one time and what happens if equipment is returned late.

**3. Who could provide that information?**

The head IT technician or the library staff could provide this information because they deal with equipment bookings and returns regularly.




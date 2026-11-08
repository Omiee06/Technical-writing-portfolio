# TaskFlow — Product Inputs and Follow-up SME Q&A

> **Note:** TaskFlow is a fictional portfolio project. The SME/Engineering answers below are simulated inputs.

---

## 1. Product Inputs

### Product Name

TaskFlow

### Product Description

A web-based task management application that allows users to organize and track work.

### Target Users

- Individual users managing personal tasks
- Small teams managing project work
- Team members who need to track task progress

### Core Features

1. Create tasks with a title, description, due date, and priority.
2. Edit, complete, and delete tasks.
3. Track tasks using these statuses:
   - To Do
   - In Progress
   - Completed
4. View tasks on a dashboard, filter by status, and see upcoming due dates.
5. Search for tasks by title.

### Initial Documentation Inputs

- **Audience initially stated:** "SME (Small and Medium-sized Enterprises) and Administration".
- **Goal:** Help users understand the workflow and features of the TaskFlow application.
- **Tasks to cover:** Create, edit, assign, track, and manage tasks.
- **Exclusions:** Software development information and advanced troubleshooting.
- **Proposed sections:**
  - Introduction
  - Getting Started
  - Workflows
  - Advanced features
  - Payment Info (if required)
  - Cancellation and Refund (if required)
  - Help and Support
  - FAQs

### Clarifications Identified During Review

- The clarified primary audience was individual users and small-team members.
- Task assignment was not included in the supplied product brief, so it was not treated as a confirmed feature.
- The product brief did not support payment, cancellation, and refund information.
- Basic user-facing troubleshooting could be included; advanced/internal troubleshooting remained out of scope.

---

## 2. Follow-up SME Questions and Answers

### A. Task Creation

**Q1. What validation rules apply to the task title, description, and due date?**

**Answer:**
- A task title is required.
- The title can contain a maximum of 100 characters.
- The due date cannot be earlier than the current date.
- Correct the information and save again if validation fails.

**Q2. What can cause a newly created task not to appear in the task list or dashboard?**

**Answer:**

The task list does not automatically refresh after task creation. Refresh the page to display the newly created task.

**Q3. What error messages can users receive while creating a task?**

**Answer:**

No specific error message text was provided in the source.

**Q4. Are there any restrictions on the information users can enter?**

**Answer:**

The confirmed restrictions are that the title is required, the title has a 100-character maximum, and the due date cannot be earlier than the current date. No other field restrictions were provided.

---

### B. Task Editing

**Q1. What can cause changes to a task to fail to save?**

**Answer:**

The user must select Save after making changes. If Save is not selected, the changes are not saved.

**Q2. What can cause an updated task to remain unchanged or not appear updated?**

**Answer:**

The source identifies selecting Save as the required action. It does not provide a separate explanation for other display or refresh issues after editing.

**Q3. Which task fields can users edit after creation?**

**Answer:**

The source does not specify the complete list of editable fields.

**Q4. Are there user or permission restrictions for editing a task?**

**Answer:**

Any user who can view a task can edit it.

**Q5. What error messages can users receive while editing a task?**

**Answer:**

No specific error message text was provided in the source.

---

### C. Task Status

**Q1. Can users change a task between To Do, In Progress, and Completed?**

**Answer:**

Yes. Users can move a task among To Do, In Progress, and Completed, including moving it back to an earlier status.

**Q2. What can cause a task's status change not to be saved?**

**Answer:**

The user must select Save after changing the status.

**Q3. What restrictions apply to changing a task's status?**

**Answer:**

No additional restrictions were provided. The source states that users can move between all three statuses.

**Q4. What error messages can users receive when changing status?**

**Answer:**

No specific error message text was provided in the source.

---

### D. Task Deletion

**Q1. What can cause task deletion to fail or appear incomplete?**

**Answer:**

The source does not identify a deletion failure condition. A deleted task may remain visible until the page is refreshed.

**Q2. What can cause a deleted task to remain visible?**

**Answer:**

The task list may not refresh automatically after deletion. Refresh the page to remove the deleted task from the displayed list.

**Q3. Is deletion permanent, or can deleted tasks be restored?**

**Answer:**

Deleted tasks cannot be restored.

**Q4. Are there restrictions on who can delete a task?**

**Answer:**

No deletion-permission details were provided in the source.

**Q5. What error messages can users receive while deleting a task?**

**Answer:**

No specific error-message text was provided in the source.

---

### E. Dashboard and Filtering

**Q1. What can cause a selected filter not to be applied?**

**Answer:**

The source says users must select a status and apply the filter. It does not provide further causes for filter failure.

**Q2. What can cause the task list not to update after a filter is selected?**

**Answer:**

The source does not provide a separate explanation beyond the instruction to select a status and apply the filter.

**Q3. Can users filter tasks by due date or priority as well as status?**

**Answer:**

No. Filtering by status is supported. Due-date and priority filters are not supported.

**Q4. What error messages can users receive while filtering tasks?**

**Answer:**

No specific error message text was provided in the source.

---

### F. Task Search

**Q1. What can cause search to return no results when a matching task exists?**

**Answer:**

Search is case-sensitive. A capitalization mismatch can prevent the task from appearing in the results. Use the correct capitalization.

Q2. Does search require the complete task title, or does it support partial text?

Answer:

Search supports both partial and complete task titles.

Q3. What error messages can users receive while searching?

Answer:

No specific error message text was provided in the source.

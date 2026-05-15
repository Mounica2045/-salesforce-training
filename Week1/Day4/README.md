# Day 4 - Flow Builder

## 1. What is Flow Builder?

Flow Builder is a Salesforce automation tool used to automate business processes without writing code. It helps organizations create workflows, guide users through screens, update records automatically, send notifications, and perform complex operations using a visual interface.

Flow Builder allows businesses to:
- Reduce manual work
- Improve productivity
- Maintain data accuracy
- Automate repetitive tasks
- Create guided user experiences

It is one of the most powerful no-code/low-code automation tools in Salesforce.

---

# 2. Types of Flows

## A. Screen Flow

Screen Flow is an interactive flow that displays screens to users and collects input from them.

### Features:
- User interaction required
- Used for forms, surveys, and guided processes
- Can include buttons, dropdowns, and text fields

### Example:
Employee Leave Request Form

### Process:
1. Employee opens form
2. Enters leave details
3. Manager receives approval request
4. Status gets updated automatically

---

## B. Record Triggered Flow

Record Triggered Flow runs automatically when a record is created, updated, or deleted.

### Features:
- Fully automated
- No user interaction required
- Runs in background

### Example:
When a new customer is added:
- Welcome email is sent automatically
- Follow-up task is created for sales team

### Trigger Types:
- Before Save Flow
- After Save Flow

---

# 3. Automation Ideas (5 Examples)

## 1. Student Attendance Alert
If attendance falls below 75%, automatically send warning email to student and parent.

## 2. Online Shopping Order Update
When order status changes, automatically notify customer through email/SMS.

## 3. Employee Leave Approval
Automatically send leave request to manager and update HR records after approval.

## 4. Customer Support Ticket Flow
Assign tickets automatically to support agents based on issue category.

## 5. Library Due Date Reminder
Send automatic reminders before book return due date.

---

# 4. Flow Diagram

## Example: Employee Leave Approval Flow

```text
Employee Submits Leave Form
            ↓
Manager Receives Approval Request
            ↓
Manager Approves/Rejects
            ↓
HR Record Updated Automatically
            ↓
Employee Gets Notification
You can also create diagrams using:

* draw.io
* Canva
* PowerPoint
* Lucidchart

---

# 5. Manual vs Automated Process

| Manual Process           | Automated Process  |
| ------------------------ | ------------------ |
| Time-consuming           | Fast execution     |
| Human errors possible    | Higher accuracy    |
| Requires repeated effort | Runs automatically |
| Delayed responses        | Instant actions    |
| Difficult to track       | Easy monitoring    |

---

# 6. Reflection

Automation is important in enterprise systems because organizations handle huge amounts of data and repetitive tasks daily. Manual work slows productivity and increases mistakes.

Using automation:

* Saves time
* Reduces operational cost
* Improves consistency
* Enhances customer experience
* Allows employees to focus on important tasks

Automation also helps businesses scale efficiently while maintaining accuracy and reliability.

---

# Reflective Questions

## 1. Why do companies automate workflows?

Companies automate workflows to save time, reduce manual effort, improve accuracy, and increase productivity.

---

## 2. What problems happen with manual processes?

Manual processes can cause:

* Human errors
* Delays
* Data inconsistency
* Increased workload
* Difficulty in tracking progress

---

## 3. Difference between Screen Flow and Record Triggered Flow?

| Screen Flow               | Record Triggered Flow       |
| ------------------------- | --------------------------- |
| Requires user interaction | Runs automatically          |
| Has screens/forms         | No screens                  |
| Used for guided input     | Used for backend automation |
| Triggered manually        | Triggered by record changes |

---

## 4. Why is no-code automation powerful?

No-code automation allows non-programmers to build workflows easily using drag-and-drop tools. It saves development time and increases accessibility.

---

## 5. When should automation be avoided?

Automation should be avoided when:

* Human judgment is necessary
* Processes change frequently
* Tasks are too complex or unpredictable
* Automation cost is higher than benefit

---

## 6. How does automation improve consistency and productivity?

Automation performs tasks the same way every time, reducing mistakes and increasing speed. Employees can focus on strategic work instead of repetitive tasks.


## Example Flow Diagram Ideas

![Image](https://images.openai.com/static-rsc-4/xNRq0_Jm8WHnXhqSMnA2Wbtx_Mt-vQWU-OspifUpL6QIqOQpttYd83iCwKBt1-4W0SKW2o8u1ptk_AI1aqa2-dK9D3rbx0yWGRwL2S_-G6lcKojBYvv26Hm5nFQwPUvfXtnZTArCVrATeKei7QJQ0qga0sWHe5NKNAjgAOXtmvkWjs4B3DMQP7lD3Be1XHm_?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/J956Qeinrb1l92VL2bEHZ9X2AIlW74j3IyhYItOFPj1btwt2hzvalEK0bcsP7WZ9kCu1vyUv1kueJ7JjUaWSEYijDbzdC774k31kqErSdheYq3LFxYH-nQ1OxanoIARmHDmoWzWsJd38yQKthHxPvmGwAIaPb1hNGar3AAHgiHvM4qn-q9lqxvop93y_3oxH?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/2MqXW3AklmSzXXXnkfbMJc-eitdoiOEuxjWaXNNgYJ2R0kewGk-gvHTfcEFbGb93wEpYnD4cruFpiRV6IsRUyhcnyDicYdni9MT8YF1h71dKY_KkPjsBg1Bys8-Wtl34A5aonfcr14zyDlTaYPwO3WrzYrgMLxmFd6nwE_aIWMTqUsNhOUoCLDHKGZsiMEQK?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/LuX5EXSDaMnC8x8kd0AlLHutAd5NigJ_XimBQIuQlcfXYuT2NQKXMkSsKxQa0Iee40I-QC4yvPgbq-XDbdDh8lBq8xTdp_4lnkPrgH2ZJLLMnFaQzwYkSOdbYu5dtTtlKyw4yvNp8YnO2gjnoPQYwFzptQ9-bul2I42NjSe83z8h2e_GP4U3Tt2Pj6mvaJnx?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/7NH6bWUXF_b4DCsHfAp9WbSquVwpzPrFFVQGnm_F03Zh-0Y95lbAPHagm3lw0tPnVJUfBp9EP-xUfxQGOEoMcsbUeodqRiSCpK4vaqfUvcxqw7I091wf8ohSRESeDOd4qntP4QBGe482Zx4YcpfFX6ejNhnLEvYdFWTvPtbEGgiOVvi2EI2mZajuTl5M8gwd?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/mJDFeClYSO0kAGYD6Ha1_V-wN19NzDyoZjEgohuCjtEV5s-A_EreIMdG_2E6yWEx55X7hGCsgYdwJr9l-I1WoSaFrGcMX7Z14RAKkXgveDqqqC1uXuD3VsSQ12igYsHYImNXCl7fG1st-ccB7AADbegx6J6f_naPWBQrrQ7Fb5a_vFX6cxpAy1BWTXhjH2Lv?purpose=fullsize)

# trailhead Diagrams
<img width="1910" height="900" alt="Screenshot 2026-05-12 211845" src="https://github.com/user-attachments/assets/08c033bc-ce24-4e98-aedf-da9938b12304" />
<img width="463" height="615" alt="Screenshot 2026-05-15 221543" src="https://github.com/user-attachments/assets/260bec13-b944-48a5-bf02-bcea60c39a72" />
<img width="1907" height="919" alt="Screenshot 2026-05-12 212917" src="https://github.com/user-attachments/assets/ec971d20-b3ad-40e6-8a77-14ae806c7be1" />
<img width="1905" height="913" alt="Screenshot 2026-05-15 224140" src="https://github.com/user-attachments/assets/e45e2fbd-4ba8-404b-8293-ca1bd16854d2" />







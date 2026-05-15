# `/day5-apex-introduction/`

## `README.md`

````markdown
# Day 5 - Apex Introduction

# 1. What is Apex?

Apex is Salesforce’s programming language used to build custom business logic and advanced automation on the Salesforce platform.

It is similar to Java and runs on Salesforce servers. Apex allows developers to:
- Create custom workflows
- Perform complex calculations
- Integrate external systems
- Write triggers and classes
- Automate advanced business processes

Apex is mainly used when Salesforce Flows or configuration tools are not enough for business requirements.

---

# 2. Difference Between Flow vs Apex

| Flow | Apex |
|------|------|
| No-code/low-code tool | Programming language |
| Easy to create using drag-and-drop | Requires coding knowledge |
| Best for simple automation | Best for complex logic |
| Faster development | More flexible and powerful |
| Less maintenance | Requires testing and debugging |
| Used by admins | Used by developers |

---

# Difference Between Configuration vs Coding

| Configuration | Coding |
|---------------|--------|
| Uses built-in tools | Uses custom programming |
| Faster implementation | More development time |
| Easy to maintain | Requires technical expertise |
| Limited flexibility | Highly flexible |
| Suitable for common requirements | Suitable for complex requirements |

---

# 3. Real Examples Where Apex Is Needed

## 1. Complex Fee Calculation System
A college wants automatic scholarship calculations based on attendance, marks, category, and extracurricular activities. This requires advanced logic using Apex.

---

## 2. External Payment Gateway Integration
When students pay fees online, Salesforce must connect with external payment systems like Razorpay or PayPal using APIs. Apex handles these integrations.

---

## 3. Automatic Timetable Conflict Detection
If two classes are scheduled at the same time for the same faculty or classroom, Apex can detect and prevent scheduling conflicts.

---

# 4. Integrated System Design
# College Management System

## A. CRM (Customer Relationship Management)

The CRM manages:
- Student information
- Faculty records
- Admissions
- Attendance
- Fees
- Examinations
- Placement activities

Salesforce CRM helps track and manage all college operations efficiently.

---

# B. Objects

## Standard Objects
- Account → Departments
- Contact → Students & Faculty

## Custom Objects
- Student
- Course
- Attendance
- Fees
- Examination
- Library
- Placement

---

# C. Relationships

| Object 1 | Relationship | Object 2 |
|----------|--------------|-----------|
| Student | Enrolled In | Course |
| Student | Pays | Fees |
| Faculty | Teaches | Course |
| Student | Appears For | Examination |

Relationship types:
- Lookup Relationship
- Master-Detail Relationship

---

# D. Validation Rules

Validation rules ensure correct data entry.

## Examples:
1. Student phone number must contain 10 digits.
2. Attendance percentage cannot exceed 100.
3. Fee amount cannot be negative.
4. Email format must be valid.

---

# E. Flow Automation

## Examples:
- Send admission confirmation email automatically
- Notify students about fee due dates
- Generate attendance warnings
- Create placement interview reminders

---

# F. Apex Usage

## Apex can be used for:
- Scholarship calculation
- Timetable conflict checking
- Payment gateway integration
- Bulk student processing
- Advanced report generation

---

# 5. Pseudocode Examples

## Example 1: Attendance Warning System

```text
IF attendance < 75%
THEN
   Send warning email to student
ENDIF
````

---

## Example 2: Scholarship Eligibility

```text
IF marks > 90 AND attendance > 85
THEN
   Scholarship = Approved
ELSE
   Scholarship = Rejected
ENDIF
```

---

## Example 3: Timetable Conflict Detection

```text
FOR each classroom booking
   CHECK existing schedules
   IF same time exists
      Show conflict message
   ENDIF
ENDFOR
```

---

# 6. Reflection

Enterprise systems eventually require programming because businesses grow more complex over time. No-code tools are excellent for standard automation, but advanced requirements need custom logic.

Programming helps organizations:

* Handle complex workflows
* Integrate external systems
* Improve scalability
* Customize business rules
* Increase system flexibility

A balance between configuration and coding is important for building efficient enterprise applications.

---

# Reflective Questions

## 1. Why is Apex needed if Salesforce already has Flows?

Flows are powerful for standard automation, but Apex is needed for complex calculations, integrations, bulk processing, and advanced business logic.

---

## 2. When should developers prefer no-code solutions?

Developers should prefer no-code solutions when:

* Requirements are simple
* Faster deployment is needed
* Maintenance should be easy
* Business users need control

---

## 3. What problems require custom programming?

Custom programming is required for:

* Complex business rules
* API integrations
* Real-time processing
* Advanced calculations
* Performance optimization

---

## 4. Why is business logic important in enterprise systems?

Business logic ensures systems follow organizational rules and processes correctly. It maintains consistency, accuracy, and operational efficiency.

---

## 5. Why should developers avoid unnecessary coding?

Unnecessary coding increases:

* Complexity
* Maintenance cost
* Bugs and errors
* Development time

Using configuration first makes systems easier to manage.

---

## 6. How does programming increase flexibility?

Programming allows developers to:

* Create custom features
* Integrate multiple systems
* Build advanced workflows
* Handle unique business requirements

This gives organizations more control and scalability.

---

````

## Suggested Folder Structure

```text
/day5-apex-introduction/
│
├── README.md
├── diagrams/
│   └── college-management-system.png
└── pseudocode/
    └── examples.txt
````

## Example System Design Diagram Ideas
## Example System Design Diagram Ideas for College Management System

### 1. Overall College Management System Architecture

Shows how all modules connect together.

Components:

* Students
* Faculty
* Admin
* CRM
* Database
* Payment Gateway
* Notification System

![Image](https://images.openai.com/static-rsc-4/_TFC7OlwFX1Vr96MMVhwCMLZaawqMSFsyxULGOGhGZbDsTAlfedEdIRkdjiSin7Sd9JtmlbCgs9i6FRaSTqcacDnL6gKF09fLOjhRAtBjAvLzMGlzWynkNhxB3an9XWBDkya4tj_hO4rN9uxy88b37S4peKDwdwPb2AeF0d0_oQL5SPUeCGwqnbryJWeSyPs?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/SL2oYyF1QsIB8Cy20Y4Xdeu_dtg4PfDGRMFbNAopT4dg1bT7v-7H768ylWgJLSHiHjGbCboXbLuwW2seC3yKzHfzG7YzMfBpKQqTDUptZxpTclwNwGUfsoeUqQg1lrlC1WkmGQki9o5Mrp1GhhFi2M5gkxmGbzLJvmrQzrnRKZvo_MNZ03TDhb4DgQSqgNsv?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/f92Cc93ba_nh0P0L_n1zvQx0mnUzU47ARXTj0IXZvPfZjULayIOC0PjHP40OcroaW8e9TXnNq11_Stg-rw8DbpVfcPAWP8fu2XgO5lOaNzP3xgFDgave5wSqHZxw2vLF6iSlAYUNGY4Q_U6B5HBWW05ht4PdlRm3mxAEjFcFiaFBCnHXtFHS7TnLCVWpyIyb?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/0UV6S-C1rRDBA4xD5YDKZu4sQC4WobgHnJn-gVL-uYyrvuzoMNNqIlQnqteYAwbx9ZlVPC26uEr6xhPlxy4vILPgCmwlVL_ciY3BEs_AN_954UPnPmIRHkGCBI9csic4eFrzifkB1gi5bVSZaxvHtsX4LjQf5krvlj6lh7Yb3aHnirYL179K2YwTMi9BVGBa?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/nlzIXG3o0i-UDPD6AYsbhkE6PHJSD4tHuOVCkCuBcpSDawB8EwHyICvptnDXqrKWtXMNYdFkANowSmPnSTFX2TPZ3ljJdvewJW4UG47J10nXNRt5JJeEXgHuQU2u9gEnU0XouYpQV5xjlJAhahMLcFozIePpvdok-u9OZ_5mWc3VcRt-7mNdy8gIZAtRgD3V?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/4_O7wwV1QWX2u4KF6S-KAR0K7xkXxUNA21RoTcxwkq9rwcAZrp0j0obdK3q6U5FTIb0xnTbtIZq_NO2OVTqIEGqvH0NXSzBaSoRHIJmnCCwdWOljoBsPeJLUUSfFfaVM4CsZTlnChxsEGdOLP671sHduMl6QvhPEgEVgh081bWF_qpH_q3HKYLdI-VzSY9NX?purpose=fullsize)

---

## 2. CRM Object Relationship Diagram

Shows relationships between Salesforce objects.

Objects:

* Student
* Course
* Faculty
* Attendance
* Fees
* Examination

Relationship Types:

* Lookup
* Master-Detail

![Image](https://images.openai.com/static-rsc-4/lx2XeBf2qNKDWtKuOc4lc0hXthWsocNPKE23QW88OVyYiWKfvmD7maTQo4_VGxoTOVR-C7CKx5263YvvllDVspjgtZmSxB0Xvjxezyt8vDqOkNp8zhe-hpFcuoO7JT7YYxoboCEw4YXc5v28NfUSDMWmmDLjmbGwkc-ccNONHYdIh7XcbB8N2psG3Ws2dS5v?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/1HehzDTRxzzR1wdokdyZ7DrwyFsPVIbzwYvoPfTRiFEjyPX4qQrmbkfX_giXvVPWpuX3SuuitGpeeOaxHACRJrTSpZ-fncfAmbtF8h9-1WDqekohHVEOsxtQNnCkfzc1wS-il4Stq_XZxiaLV3NH99pRmU2N-e7pqDyKthIFKuq_e0ytACo8YYK1t-X6Qnhf?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/ItuKwYLYxa7gWYU5jf2rme_4PMwDm5UtDQLpvaG8dqVFELlM-xUW6Dib-CLM9RNp5L7sm57CWXICGG35qpPbG5-ZaTTkiNfYHT4ZNNQfa-wYcHkNG8ONbdr4tk07HrLe5LgNuqREatHToY6WyK4_V5jg6eGo5h_oPdDccWVvFToYRgk03rzuvWjrJ9Uq6xUZ?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/SaQe4ToaB2ZruVixQBONP4GyNPbRCwCvS0-jGllV-BelFZJNUqrVc2CDUoFDMC_h8Vy68WbY7SDf6jpELzFTwBo8ClVO9Hq7mjxRJu1c8GDHb5h6rh9JQcj5Wmgnma4vMt_kKiMjkZglbXrYl46wPTSm5oFVDe847tmnd4bN3hv-z4DPQqO8JYvle9mljido?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/yHVtI0pzBqB7-i7LVxjG4j1e1ysQJ7v1ybIyT8JVw9MLiSs953otaGCkWI2conpAuwK_9zFSD42toa0GASEBQcklsimObvYfru-zIyMJutl8eDLTAFNvPDsJO86AZKrKlNtCkjOE0aEth_uvLmbg9n-7637zFkAI2dioC_NGX-bDNnaqOOSev7tZPaJenipy?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/bfMkK_iVp0Py0kKFcKpq9IDJQsWMqE5MN4THVyEaWZwxw5JGjkbxN9hzNQ3pTBkXGJmZC18G1ZcW0gCCf6MDVBtt0br_HBR74d-BVJjQC5mO0OcyEDYbAI1s_nMnijfL4w_KFmK5cvmrxER56EO6xHmiZHefaK6CtX57EW0PpSMrrBSxNWwPFdzes4rDiCze?purpose=fullsize)

---

## 3. Flow Automation Diagram

Shows automation process using Salesforce Flow.

Example Flow:
Student Registration → Email Confirmation → Fee Record Creation → Notification

![Image](https://images.openai.com/static-rsc-4/LuX5EXSDaMnC8x8kd0AlLHutAd5NigJ_XimBQIuQlcfXYuT2NQKXMkSsKxQa0Iee40I-QC4yvPgbq-XDbdDh8lBq8xTdp_4lnkPrgH2ZJLLMnFaQzwYkSOdbYu5dtTtlKyw4yvNp8YnO2gjnoPQYwFzptQ9-bul2I42NjSe83z8h2e_GP4U3Tt2Pj6mvaJnx?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/JKvLlhbUMhhAHmoeMR4bC3P8jhRUukWPgEBx9F4t30lB2Om32Bn3AFucTGM5WZgbvXXXza59lBXeHnk4eB0c8nntbrTxkscx3Z1eVjw-z4HFedksn4gefZRrpY19vwd5SuqrXS2n4aHFpIM5VeSPiW_sRHQ0W1Ow4YP9zIOsJ93TDhEwGzSyRtNEecp-Dkhu?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/wImR-6tngeNtcEesBGp2P93eNMjKLdJAEPB8Sk9Djs2Z7qMx7uXOaGqHbuAaMGX_6Ld8V46Or5h02PnZsbx29fzlDrQY25mxm_vMqoPaJqof6uLJE-XT5wahvcCVaWrQhMqWjnqpbk14nE5dVUnpVemoKmka-rAJmP1NOtKCoz29FFuVjUl_4by19gqmGNNa?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/Som2_Yh5JrPL9etx2WFUYZvvirkC8sp036NbP17aZw3ODS5x7UMJ-sbb5NBjc5NS5BS-1O9m0MedTIUbdReJ40mG-qj9vBMiyPVQggAZ2tWccR7HsVeFHnAWOFvYgMLLX3ijaLMbnhIWHA3TGbGuijuwcLXpzk152mBH3JIepe0JDyXfl-yOVYXp200DIaqE?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/R32-vkw1VdKy188qZzuxJitys96DwKVhBjZDobqaCy4GdRmE8fOj1YLhy3JdfZmm0d7irj5Ex27lRTpSq4XqkKZZKBj_B6CnG4QEo6LYcDrvwjDeir6-vj53XEkFfT0LP4wjPFF3t4TcZs7ck7i9GaL9FN7E00VqjjT88lfHS2E3CbEsj2bWr-MuFqKOTWpA?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/o23tRnXe58asSIvDiNfPYjSLcM9jTXUguYVC7-OgmFZr8tQ31F79wN2yl87nGNC-all41hvOkj9zsABWLCK2k1AkNwvck0i7MqrU5YUvDPieQrhKlTBCZc_ShKfKnyKngl5CJGh7XrZ6r6iFiV4R_aEjChICeR_i2MXljyXD0h_bsr1M045M14LN1mZdgX2y?purpose=fullsize)

---

## 4. Apex Integration Diagram

Shows where Apex is used for advanced processing.

Examples:

* Scholarship Calculation
* Payment Gateway Integration
* Timetable Conflict Detection
* Bulk Student Processing

![Image](https://images.openai.com/static-rsc-4/tePhgZvj_eN09-I0c6eKZQGU2s914INSHvpcyQmnIhSkthWwa8tuw_XWWWFn7RzezqrsJuKSbONLiME3QAbVQ88CRuCXRA-aKemGIU4vkBvI232QzytUOZotyUua4NHV5maRiTwnSHq_ZQnPmT8Z9dgr0XBgyy92RRWdLLbrNSH4Xlq17RLGgbbDoxbLUFn3?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/kkGjSo0HVrp4ock2nLpLMefOipZuZIJbOJlnPRqKJ0j7SaAl1vrht68YG0YPsafww2S4p8aQ2AqbiVZg0RGS_43mYNR9EbudkCVxaiu5-BApTm8VxQ4luqkdp2YtySg8EfrPs8HWFi6dT3gyW66A5X681zw3ok8GqYeIPci-qE025wU1iJ0UaeFCo4B7D1Um?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/3BATlW-8YR8EMb5Q7f9OtNlr5k6yiyE4eDk00hUgCRsb8qz_w6gG8ExX60W0MQgqnoxqRNvFVPz85P36Vha-cuYwGFBASbEwjzP8CPGESLTo-2BCYBr4d3u1r3cmXINTwPAY62B3sRX2tgDFU-by5m7Tpu54xrWOawDOQ-0nYIk-fESnxOEijSddLMK4P7at?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/w26mH2mKA9utNsdzEKjv0bGaTauKZ8GpjER5wRNZ8jQn-KuGy29-DYbHg8_sHfqAMgygWcExzty6h4huwOn8RBq-uXzTOnQ4BnbOrki7g-6QKMCIrsWOcxlPgoFX4OICNcnT6rJcE0YhJaLJd9EAdPoI_g2kUWd5Hv2b9JWo9QudST6QKvi_CKkjfAZO41ut?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/rMcloZ0_oUdgef8Are1VPsz553P52yLSMfTn7Jr4gp94_mv27mM4m-sqpLmDa92p_Cy46ZH07fvq6IjCkllJ1J13WFDqlgwJxEWMA81q9zK6u_hVVHiSsWVkKhlp6HBmTMfnfeA0pNVXsvpBdxp50ctCV__jgyIkgGnBhj9sbw18IcudyNB36XJEthJfGvfJ?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/o3efQeBZpsRhYJhct1oa3qsBIAqY6cKE4XFXQ2wO2ggoKg0ymVA0XjhPUFiBKmlB4PtIBA88ErRiWteHlZbiAbVXWiHBJkrIBivcJD28TY-BEHHLsnb78IZULRXhWeKiFKT1lvgIcVtusYvK774mjWcFi9wbeyIbAtA3eeCEFu0sq9JwgGtLJBRKYxKqz4es?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/fwTcK3HOcsnsF0gY2KNm4k_uKl2Ko8PAFg_w2e9uXU9N3iOIGtE6BHIOixLNGBy0brcXCitV9ZuB-BQWCpDUFcePLK74nQ3Sx1RaQGqDRVTSCJ5oNurTcUbr2TOwaeb3BOZEs7B5GSA3xMti0d6GfqTAlMKO89Zx3Rj6QPO6Jm8LdvKUIfVRjEI4DvRsI_YI?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/paq-7r-_M8QJjBRR3rVIHBxnI11PxwM691OeravAJM1eyAZs8g5r4Ct9kxn2IolhduoXWXf5MuUuXAcTctC4TJoCzR2ZOOeFprwu_2tavvDxNwW86VsMMHQVUrOp_JPVpFdMra7QkiEwJOtzFmh5ERtYKtiJPrVyEJONDLErsZfuVND1R7IiiugM6spyiMgl?purpose=fullsize)

---

## 5. Validation & Approval Process Diagram

Shows how validation rules and approvals work.

Example:
Student Applies for Leave → Validation Check → Faculty Approval → Status Update

![Image](https://images.openai.com/static-rsc-4/QuCXrDguhowOjNnE808CYhol5eOCW665RFe6BWWPXJsfOKemR5jLcICC4j0B7oQd_iRSBMbYdbn4J_FtE4DC3Bqhc8SJznfFdJalMaYUxQBeltOrNQ0onKTIskwcBFfFAYy3fgjXcfJ25Go1_TpawjHhRwK8oOFhkEqmW35uJHgeBRiDKiZl2z4Gzb53FHxO?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/32uUHh_k3NAFmqc9cBtNhuEqrIbO9ls88HwT9JOeYgbppCSamAKWpzKfhkHYUwInVcnzLK9yLBuJBHRGyBwdGngHpY77qv0f34sHh-zQnViadzN_I6B0-WDxkb0fyofFtnRdgM8y-cw2TvsHY5x-OswKFxzimn-gIzowKzp-aMbwtKRCRj9--8rYnyAWa2_D?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/e25217TnUFXko4dQogUi8yC0kp02Op5HXVMrbBtkHTm5jg7Hkw9z4m5JioJ_tbj3r5Uanv3JdLV1TRhezUvG13JRxpCAaXHuB7Q4kzWyRC4ILBBm6wEwbH_ravf6P2mp3iFvbhz-uaVzfeHuXLeuegWZoRt2jGAMz-4uXKV6DWL2xL2FVa2gCCYIp8XK2XfX?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/O9KSyZbzKVH0yeb7u94M7cXhnGC2Tzy0pH1GrJgSFQPODcc05YgQJVTsO9hHYNAytVYa4uGcM7UjLE7dbnfUoWcs5aq3EossefStmjKycfNw_IxuZYr2RMMChs8g1AiYQsaRIVDKtWvASoJ3u5T2fQac-ZKyleccv6efDj6iZUrgU6jOFvB09QmOi4uuedSS?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/llfneTHlCF0ZkBDJ4YmLzbvzmXRV_27fwtw2zKRC9a1cTlaH6gdLWtrOADyxBpIGwwijKQ4cQi_6And-mq_uoxCSpZLNMZ2be85p6x54QZEylIg_zRnMfP8k8tfKO-vHOJhcwmDzn5fVPxlyP0ILEmy734HfheGFqciPSTeTEI7ytBQTBAKCKBIuysu1_rhV?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/nxsAqHr0t6SZo8_YYqCeHqaTL6pE9tOUS10J97owOJCp0j5BD5EcNEuGND3nLWCOpBj_ei33G4kOxq67mc_rcCfnKHrTmyCNxv-7CmW5hcz7qBnS8BjXLJygC67FV_GiP5IP0lgz_ecz02z6DxxObAXXspzuOqTfQ4cUREoLu8fzpLb-bBLXm_J4-rpK1WrQ?purpose=fullsize)

#trailhead examples

<img width="1231" height="913" alt="Screenshot 2026-05-15 233201" src="https://github.com/user-attachments/assets/2154cf55-3da7-4f18-8a5c-625a6220c448" />
<img width="1074" height="578" alt="Screenshot 2026-05-15 233151" src="https://github.com/user-attachments/assets/84fd546b-aa5f-4a35-9524-24aa0cc3f2b6" />
<img width="1005" height="371" alt="Screenshot 2026-05-15 233131" src="https://github.com/user-attachments/assets/cd11076b-ac07-4848-8a08-1967d69f6787" />
<img width="1904" height="904" alt="Screenshot 2026-05-15 231238" src="https://github.com/user-attachments/assets/0ea9e824-501f-484b-b64e-8c27f6e31dab" />

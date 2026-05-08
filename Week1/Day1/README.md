#1
What is CRM?

The provided video describes CRM as an essential business investment whose profitability and Return on Investment (ROI) can and should be rigidly measured

Why companies use Salesforce

Companies use Salesforce—specifically the Customer 360 platform—to unite their teams and data onto a single, connected platform

Real business problems solved using Salesforce Salesforce solves the overarching problem of disconnected systems and team silos that naturally lead to poor customer experiences and stalled business growth
. It addresses specific, tangible pain points across different business departments:
Marketing Disconnects: Marketing teams often struggle to measure their pipeline or smoothly hand off leads to sales
. Salesforce solves this by using AI to deliver personalized customer journeys, track campaign ROI, and automatically route the right leads to the correct salespeople. This drives a 28% improvement in marketing ROI
.
Sales Inefficiencies: Sales reps frequently lose track of deals in personal inboxes and manual spreadsheets
. Salesforce solves this by automating monotonous data entry, generating automatic renewal opportunities, and using AI to help reps focus only on the leads most likely to close. This results in a 29% increase in sales revenue
.
Blind Customer Support: Service agents often lack context about a customer's journey because they operate on completely separate systems from marketing and sales
. Salesforce provides a single, unified view of the customer's history from every touchpoint. It also introduces omnichannel routing and self-service bots to resolve issues faster, which drops support costs by 27%
.
Outdated Leadership Reporting: Business leaders frequently have to make major decisions based on manually updated, perpetually out-of-date spreadsheets
. Salesforce solves this by providing leadership with business insights 29% faster, relying on real-time data rather than incomplete, outdated reports
.

#2
Salesforce Interface Basics:-
Home Dashboard: The main dashboard gives you a "bird's-eye view" of vital information, allowing you to quickly monitor closed deals, pipeline progress, relationships to grow, and daily tasks
. If the default view isn't enough, you can create fully customizable dashboards with personalized charts to track exactly what you want to see
.
Global Actions (+ Sign): Found in the top right corner, this + button acts as a universal shortcut to quickly create new leads, contacts, tasks, events, and emails from anywhere within the system
.
Files Section: This area functions similarly to Google Drive, providing a centralized space where you and your team can upload and instantly access necessary documents
.
Leads, Contacts, and Accounts
Leads: A lead represents the very beginning of a potential deal, often starting as a simple conversation with someone who seems interested
. When creating a new lead, you log standard information such as their name, title, company, email, and phone number
.
Accounts: Accounts represent the actual companies or businesses that you are working with
.
Contacts: Contacts represent the specific individuals who work at those companies
.
The Relationship: You do not necessarily have to create Accounts and Contacts manually. When a lead is successful and you convert it, Salesforce automatically creates a new Account for the company and a new Contact for the individual

Basic Workflow Understanding 1. Initiating and Tracking a Lead: The CRM lifecycle starts by creating a lead
. As you interact with the prospect, you manually advance the lead's status through a designated lifecycle, moving it from stages like "open - not contacted" to "working - contacted"
.
2. Converting the Lead: Once the prospect is fully engaged and ready to move forward, you update their status to "converted"
. Upon clicking convert, Salesforce automates the heavy lifting by instantly transforming that single lead into an entire business relationship, creating an Account, a Contact, and an Opportunity all at once
.
3. Managing the Opportunity: The newly created Opportunity represents the actual deal or sale you are trying to make
. Just like leads, opportunities have their own lifecycle stages. You will guide the opportunity through stages such as "qualification" and "needs analysis," continually advancing it until the deal is successfully "closed"
.
4. Utilizing Tasks: To manage your daily operations throughout this lifecycle, you can create Tasks
. Tasks can be assigned specific due dates, linked to specific accounts or companies, and delegated to different team members
. These tasks will populate in a calendar view and notify you on your home dashboard so you never miss a step in the workflow

#3

What are Objects? In Salesforce, objects are digital representations of real-world things
. Because you cannot physically insert actual people or organizations into the CRM, you use objects to represent them digitally
. Objects are also commonly referred to as different "record types"
. Key examples of standard objects include Leads (unqualified opportunities), Contacts (people), Accounts (organizations), and Opportunities (qualified deals)
. Products are also objects used to represent the specific goods and services your business offers
.
What are Records? Records are the individual digital forms or entries that exist within an object to represent a specific, singular entity
. For example, if a user searches for a specific person's name in the system, Salesforce will pull up the relevant individual records associated with that search
. Because Salesforce functions as a relational database, each record should be assigned an owner (a specific user) to ensure accountability and guarantee that nothing falls through the cracks
.
Understanding Salesforce Data Structure Salesforce is built on a relational database structure, meaning distinct objects and records are interconnected
. A core example of how this data structure flows is the standard lead conversion process:
Data often initially enters the system into the Leads module, which acts as a "dumping ground" for unqualified opportunities
. Leads function as an "orphan module" that sits independently from the rest of the system to ensure your other data stays clean
.
Once a lead becomes qualified, you perform a conversion, which takes the lead record's data and uses it to automatically create three distinct but related records: an Account, a Contact, and an Opportunity
.
This relational structure allows you to group data logically, such as growing a list of multiple specific contacts (people) directly underneath a single target account (organization)
.
How Salesforce Applications are Built Building and customizing Salesforce applications involves modifying backend configurations to support your organization's specific processes
. This should be guided by "Task Technology Fit theory," meaning you should only build customizations and layouts if they actively support your business processes and customer journey
. Applications are customized and automated using backend tools:
Object Manager: This configuration tool allows you to modify how specific objects function
. You can create custom page layouts, manage custom fields and relationships, and add specific buttons, links, or actions to build personalized views
.
Automations (Flows): Salesforce allows you to build automated workflows using the Flow Builder so you can accomplish more tasks with less manual effort
. These automations are built using a "When, If, Then" logic framework
:
When (Event): The trigger that kicks off the automation, such as a new record being created or updated
.
If (Condition): The entry conditions used to narrow the scope, ensuring the automation only runs in specific scenarios (e.g., only if a lead was generated from a "book consultation" form)
.
Then (Action): The resulting step the system takes, such as automatically updating a related record or sending an email alert

<img width="1903" height="901" alt="Screenshot 2026-05-07 234040" src="https://github.com/user-attachments/assets/9b3ea173-6d12-42a6-aa91-e8df1a003641" />

<img width="1903" height="911" alt="Screenshot 2026-05-07 233830" src="https://github.com/user-attachments/assets/1062d88f-d967-4547-a6fe-1638fda243fa" />

<img width="1903" height="911" alt="Screenshot 2026-05-07 233830" src="https://github.com/user-attachments/assets/e390313e-4c12-49f8-9147-c8af5743f169" />

<img width="1904" height="914" alt="Screenshot 2026-05-07 222142" src="https://github.com/user-attachments/assets/deb1e030-1b4f-48be-8b14-f47596df6273" />

<img width="1904" height="914" alt="Screenshot 2026-05-07 222142" src="https://github.com/user-attachments/assets/00e41999-1ce6-4090-89b2-fa3c1e615f6d" />

1. What problem does Salesforce solve?
Salesforce solves the problem of managing customer relationships, sales, support, and business operations in one centralized cloud platform. It helps companies track customers, automate tasks, improve communication, and increase productivity.


2. What is CRM?
CRM stands for Customer Relationship Management. It is a system used to store and manage customer information, interactions, sales, support, and business activities to improve customer relationships and business growth.


3. What is an Object in Salesforce? Give one example.
An Object in Salesforce is a database table used to store data. Each object contains records and fields.
Example: Account Object – used to store information about companies or customers.


4. Difference between Salesforce Admin and Salesforce developer 

Salesforce Admin

Manages and configures Salesforce platform

Handles users, security, reports, dashboards, and workflows

Uses mostly no-code or low-code tools

Maintains day-to-day system operations


Salesforce Developer

Develops custom applications and features in Salesforce

Writes code using Apex, Visualforce, and Lightning Web Components (LWC)

Creates integrations and advanced automation

Extends the functionality of the Salesforce platform

5. Suggest one real-world application that can be built using Salesforce.
A Hospital Management System can be built using Salesforce to manage patient records, appointments, doctor schedules, billing, and customer support efficiently.





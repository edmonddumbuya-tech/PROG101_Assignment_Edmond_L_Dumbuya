WasteTrack SL
A Community Waste Collection Scheduling and Missed-Pickup Reporting System (Logical Design)
Course	PROG101: Principles of Programming Logic and Design
Assignment	Assignment 1: Designing Logical Solutions for Sierra Leone Community Challenges
University	Limkokwing University of Creative Technology, Sierra Leone
Student: Edmond L. Dumbuya 
Student ID: 905006577
Examiner: Elijah Fullah
Semester: 1
Note: This is a design project. No source code is included, as the assignment brief requires a logical design only (algorithm, pseudocode, flowcharts and modular design).
1. Project Overview
In many Sierra Leonean communities, household waste is collected irregularly. Residents do not know when collection will happen, crews have no shared schedule, and there is no simple way to report a missed pickup. Waste then piles up, blocks drains and affects public health.
WasteTrack SL is a logical system design that:
registers households into collection zones,
stores a weekly collection day for each zone,
sends SMS reminders the day before collection,
lets residents report a missed pickup,
escalates repeatedly missed zones to a supervisor,
produces a weekly performance report.
The system is designed to work through SMS/USSD, so it can reach residents on basic phones with limited data.
2. Problem Analysis
Question	Answer
Problem	Irregular, untracked household waste collection
Who is affected	Households, traders, schools, clinics, collection crews, the city council
Why it exists	No central schedule, no complaint tracking, informal coordination, limited internet access
How the solution helps	Reminders, easy reporting, crew assignment, automatic escalation and weekly reports
3. Computational Thinking
Decomposition: registration, schedule management, notifications, missed-pickup reporting, crew tracking, supervisor reports.
Pattern recognition: weekly repeating schedules; every report follows the same steps; the same zones are often missed repeatedly.
Abstraction: a household is only an ID, name, phone number and zone; a zone is only a name, collection day and crew.
Algorithm design: step-by-step procedures, converted into pseudocode and flowcharts.
4. System Modules
No.	Module	Main Functions
1	Household Registration	validatePhone(), registerHousehold()
2	Schedule Management	checkSchedule(), getCollectionDay()
3	Notification	sendNotification(), sendDailyReminders()
4	Missed Pickup Reporting	reportMissedPickup(), countMissedReports()
5	Crew Tracking	assignCrew(), markZoneCollected()
6	Supervisor Reports	escalateToSupervisor(), generateWeeklyReport()
5. Programming Logic Concepts Demonstrated
Constants: ESCALATION_LIMIT = 3, REPORT_WINDOW_DAYS = 7, MIN_PHONE_LENGTH = 8
Variables and data types: String, Integer, Boolean, Real
Decision structures: IF / ELSE IF / ELSE, SWITCH
Boolean logic: AND, NOT, comparison operators
Repetition structures: FOR EACH (nested) and WHILE
Functions and modular design: six modules with reusable functions
Input, processing, output: defined for every process
6. Sample Scenarios
Scenario	Expected Output
Unregistered phone reports a missed pickup	“Please register first”
Report made on a day that is not the zone’s collection day	Next collection day is shown
Report made, but crew already marked the zone collected	Report saved as “Disputed”; supervisor alerted
Zone not collected, 1 missed report this week	Crew assigned; confirmation SMS sent
Zone not collected, 3 missed reports this week	Escalated to supervisor
Reminders run for 3 zones (40, 25, 35 households)	“100 reminders sent”
7. Sustainable Development Goals
SDG 11: Sustainable Cities and Communities (main goal; better municipal waste management)
SDG 3: Good Health and Well-being (cleaner surroundings reduce disease)
SDG 12: Responsible Consumption and Production (responsible handling of waste)
8. Open Source and Digital Public Good
Why open source? Waste collection is a public service. Open source means no licence fees, local developers can study and improve the design, and communities do not depend on a single company.
Possible community contributions: translations (Krio, Mende, Temne), USSD/SMS improvements, new report types, bug fixes, documentation, and adaptation for other towns and districts.
Digital Public Good: The design is intended to be released under an open licence, to use open standards, to protect residents’ privacy, and to support the SDGs. It is accessible (works by SMS), open (anyone can reuse it) and built for public benefit.
9. Community Impact
Expected impact: cleaner streets, fewer blocked drains, better public health, more trust in waste services.
Beneficiaries: residents, traders, schools, clinics, collection crews and the local council.
Long-term sustainability: low running cost (SMS-based), simple for community groups to manage, and open so local developers can maintain it.
10. Repository Structure
README.md
Report/ contains PROG101_Assignment1_WasteTrack_SL.docx
Flowcharts/ contains main.png (missed-pickup report), remind.png (daily reminders) and modules.png (system modules)
Pseudocode/ contains WasteTrack_SL_Pseudocode.txt and WasteTrack_SL_Pseudocode.pdf
11. How to View the Project
Read the Report for the full rationale, algorithms, outputs and references.
Open the Flowcharts folder to see the process diagrams.
Open the Pseudocode folder for the complete logic of every module.
12. Version Control
This project was developed using Git and GitHub with regular commits as the design progressed (README, problem analysis, algorithm, pseudocode, flowcharts, expected outputs and final report).
13. References
United Nations. Goal 11: Sustainable cities and communities. https://sdgs.un.org/goals/goal11
United Nations. Goal 3: Good health and well-being. https://sdgs.un.org/goals/goal3
United Nations. Goal 12: Responsible consumption and production. https://sdgs.un.org/goals/goal12
Digital Public Goods Alliance. Digital Public Goods. https://digitalpublicgoods.net
Open Source Initiative. The Open Source Definition. https://opensource.org/osd
GitHub Docs. https://docs.github.com
14. Academic Integrity






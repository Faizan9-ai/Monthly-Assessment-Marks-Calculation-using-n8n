# Monthly Assessment Marks Calculation Automation using n8n - 
#### Link - http://localhost:5678/workflow/ENLd2DbqO2I7HQwH

This project is an end-to-end workflow automation built using n8n to streamline the process of evaluating monthly assessment marks for students. The system automatically collects module-wise marks through an n8n form, calculates the average score, determines placement eligibility, and provides personalized feedback based on student performance.

The workflow was designed for both Data Analysis (DA) and Data Science (DS) students. Separate module categories were included for each specialization. For DA students, the workflow evaluates marks in Python, EDA, SQL, Power BI, and Advanced Statistics. For DS students, it evaluates Machine Learning, ANN, CNN, NLP, and Generative AI modules.

The automation begins with an n8n Form Trigger node that captures student details and marks. A JavaScript Code node processes the submitted data, dynamically calculates the average marks, identifies weak-performing modules, and generates eligibility status. An IF node is then used to compare the calculated average against the placement eligibility threshold.

If the average marks are greater than 70, the workflow routes the student to an “Eligible” branch and displays a congratulatory message. If the average is less than or equal to 70, the workflow routes to a “Not Eligible” branch and provides suggestions on modules that require improvement.

## Key Features

* Automated student assessment evaluation
* Dynamic average marks calculation
* Placement eligibility prediction
* Weak module identification
* Conditional workflow branching using IF node
* Real-time form submission handling
* End-to-end no-code/low-code automation using n8n

## Technologies Used

* n8n Workflow Automation
* JavaScript
* IF Node Logic
* n8n Form Trigger
* Form Ending Nodes

  Workflow Explanation


1️⃣ Form Submission

The workflow starts with an n8n Form Trigger node that collects:

Student Name
Student Email
Course Type
Module-wise marks


2️⃣ Marks Processing

A JavaScript Code Node processes the submitted marks dynamically based on the selected course type.

The node:

Calculates average marks
Detects low-performing modules
Generates eligibility status

3️⃣ Eligibility Evaluation

An IF Node checks whether:

Average Marks > 70
✅ TRUE Branch

Displays:

Congratulations! You are eligible for the placement drive.
⚠️ FALSE Branch

Displays:

You are not eligible. Please improve in weak modules.


✨ Key Features
End-to-end workflow automation
Automated average calculation
Placement eligibility prediction
Dynamic weak module detection
Conditional branching logic
Real-time assessment evaluation
Beginner-friendly low-code implementation


📊 Sample Output
Eligible Student
Average: 82
Status: Eligible
Not Eligible Student
Average: 64
Weak Modules: SQL, NLP
Status: Not Eligible



📂 Project Structure
n8n-monthly-assessment-automation/
│
├── workflow.json
├── README.md
├── screenshots/
└── demo-video.mp4
🎥 Demo

The project includes:

Workflow execution recording
Form submission testing
True/False branch execution
Automated eligibility evaluation

This project demonstrates practical workflow automation, conditional logic implementation, and low-code process orchestration using n8n for educational assessment systems.

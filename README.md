# Smart India Hackathon Workshop
# Date:14/05/2025
## Register Number:212224200308
## Name:Yaazhini S
## Problem Title
SIH 1653: Web based Selector-Applicant Simulation Software
## Problem Description
Background: Recruitment and Assessment Centre (RAC) under DRDO, Ministry of Defence carries out interviews for applications received against advertised vacancies and for promotion to next higher grade for scientific manpower inducted within DRDO. Description: The process of interviewing is a challenging task. An unbiased objective interviewing process helps identify the right talent. The basic process of an interview involves posing a set of questions by an interviewer and thereafter evaluating responses from candidates. Thus, the questions asked should be relevant and match the area/ expertise of the applicant and the responses should also be of relevance w.r.t. the question asked. Expected Solution: The proposed solution should provide experts as well as candidates a real life Board Room experience, starting with initial ice-breaking questions leading to in-depth techno-managerial (depending on the level of candidate) questions. It shall also be able to provide a quantifiable score for experts as well as the candidate for the relevancy of questions w.r.t. the area/ expertise of the applicant. Similarly, candidate responses should also be graded for relevancy w.r.t. the question asked, finally assisting in arriving at an overall score for the subject knowledge of the candidate and thus his/ her suitability against the advertised post.

## Problem Creater's Organization
Ministry of Defence

## Idea
idea description:
A web application called MatchSim was created to mimic the process of matching applicants (such as job seekers, students, and candidates) with selectors (such as businesses, educational institutions, and program directors). It enables users to create personalized preferences, model matching rounds with real-world algorithms, and assess the efficiency and fairness of results.

Essential Features: Roles of Users:

Selector: Enters the applicants' ranking or list of preferences.

Applicant: Provides a list of selectors' preferences or rankings.

Admin/Instructor (Optional): Oversees participants and simulation scenarios.

Input of Preference:

interfaces that use drag and drop to rank entities.

Data import options (CSV/Excel).

Algorithms for simulation:

Gale-Shapley (Algorithm for Stable Marriage)

Match at random

Selection based on priority (e.g., skill match, highest score)

Visualization

Results of matches in real time

Charts displaying preference gaps, stability, and satisfaction

Comparing results from various algorithms side by side

Scenes and Replay:

Run several simulations with different inputs.

Save and rerun earlier situations.

Reporting and Exporting:

Results can be exported as CSV or PDF.

Create summaries of reports.

## Proposed Solution / Architecture Diagram
![img](https://github.com/user-attachments/assets/bcd7f096-0e99-4b08-9cbe-463cc162b624)


## Use Cases
## MatchSim Application - Use Cases

### 1. Applicant-Selector Matching

#### Description:

Applicants (e.g., job seekers, students) can submit their preferences for selectors (e.g., companies, universities), while selectors can provide a ranked list of applicants.

#### Actors:

* Applicants
* Selectors
* Admin/Instructor (Optional)

#### Precondition:

* Both applicants and selectors are registered in the system.

#### Main Flow:

1. Applicants provide their preference list for selectors.
2. Selectors rank the applicants based on their criteria.
3. Admin can initiate the matching simulation using an algorithm (e.g., Gale-Shapley).
4. The system calculates the matches and displays the results.

#### Alternate Flow:

* Applicants or selectors can modify their preferences before the simulation starts.
* Admin can select a different matching algorithm.

#### Postconditions:

* Matching results are saved and can be exported.

---

### 2. Simulation with Multiple Algorithms

#### Description:

Users can run simulations using various algorithms to observe differences in matching results.

#### Actors:

* Applicants
* Selectors
* Admin/Instructor

#### Precondition:

* Participants (applicants and selectors) have provided their preferences.

#### Main Flow:

1. Admin selects multiple algorithms for comparison (e.g., Gale-Shapley, Random Match).
2. The system runs the simulations in parallel and displays the results.
3. Users can view and compare the outcomes of each algorithm.

#### Postconditions:

* Comparison results are saved and can be exported.

---

### 3. Visual Analysis and Reporting

#### Description:

Users can view real-time visualization of matching results and generate reports.

#### Actors:

* Applicants
* Selectors
* Admin/Instructor

#### Main Flow:

1. After simulation, the system generates visual charts (stability, satisfaction, etc.).
2. Users can customize the chart view (e.g., filter by preference gap).
3. Admin can export the visual report as PDF or CSV.

#### Postconditions:

* Visual report is saved and can be shared.

---

# 4. Scenario Management

# Description:

Admin can create, save, and manage multiple simulation scenarios for educational or experimental purposes.

# Actors:

* Admin/Instructor

# Main Flow:

1. Admin creates a new scenario and defines participant types (applicants, selectors).
2. Admin saves the scenario for future use.
3. Admin can reload and rerun any saved scenario.

# Postconditions:

* Scenarios are stored and can be reused or modified.


## Technology Stack
## MatchSim Application - Technology Stack

### 1. Frontend

* **Framework:** React (JavaScript/TypeScript)
* **Styling:** Tailwind CSS
* **State Management:** Redux Toolkit or React Context API
* **UI Components:** ShadCN/UI, Lucide-React
* **Visualization:** Recharts for dynamic charts

### 2. Backend

* **Framework:** Node.js with Express
* **Language:** JavaScript/TypeScript
* **Database:** PostgreSQL (relational), Redis (in-memory caching)
* **Authentication:** JWT (JSON Web Token)
* **API Design:** RESTful API or GraphQL

### 3. Algorithms

* **Stable Matching:** Gale-Shapley Algorithm
* **Random Matching:** Custom random selection
* **Priority Matching:** Score-based selection

### 4. Deployment and Hosting

* **Cloud Provider:** AWS, DigitalOcean, or Vercel
* **Containerization:** Docker
* **CI/CD:** GitHub Actions, Vercel Pipelines

### 5. Security

* **Encryption:** HTTPS (TLS), JWT for secure API access
* **User Authentication:** OAuth 2.0 (Google, LinkedIn)
* **Access Control:** Role-Based Access Control (RBAC)

### 6. Monitoring and Logging

* **Monitoring:** Prometheus, Grafana
* **Error Tracking:** Sentry
* **Logging:** Winston (Node.js)


## Dependencies

## Frontend Dependencies

* React: Core framework for building the user interface.
* React Router: For managing client-side navigation.
* Redux Toolkit: For state management (optional, if complex state handling is needed).
* Axios or Fetch API: For making HTTP requests.
* Tailwind CSS: For responsive and utility-based styling.
* ShadCN/UI: For UI components.
* Recharts: For data visualization an...

# Wahdy_Aref_Howa_Da_Dor_ElBotola

---

# 1. Functional Requrmints
  1.	Candidates should specify their skills, experience, education, career goals, and portfolio.
  2.	Employers should display company information, open positions, and other relevant details.
  3.	System should allow employers create job posting
  4.	System should recommend jobs to candidates & candidates to employers
  5.	System should allow candidates to browse jobs
  6.	System should allow employers to review applications
  7.	System shall prevent duplicates & conflict applications
  8.	System should compare candidates according to skills & tell them skills they miss
  9.	System should send notifications for new job matches

---

# 2. Non-Functional Requrmints
  1.	Low Latency in searching
  2.	Reliability
  3.	Support large number of Daily Users

---

# 3. Data Model

  Entities: Candidate - Employer - Job - Profile - Application
  ![Data Model](./Datamodel.png)

---

# 4. API Design

  ### Create Profile
  POST/profile
  body:{
    "name": string,
    "skills": string[]
  }

  ### Get Profile
  GET/profile/{profile_id} -> profile

  ### Get Jobs
  GET/jobs -> jobs[]

  ### Create Job
  POST/jobs
  body:{
    "content": string
  }

---


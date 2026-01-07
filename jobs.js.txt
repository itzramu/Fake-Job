const jobs = [
{
title: "Senior Java Developer",
company: "Innovatech Solutions Pvt. Ltd",
location: "Pune, India",
experience: "3+ years",
description: `
Innovatech Solutions Pvt. Ltd is a leading software development firm with over 15 years of industry experience. 
We specialize in delivering robust and scalable solutions to global clients.
`,
responsibilities: `
Design, develop, and maintain Java applications.
Collaborate with cross-functional teams.
Conduct code reviews and ensure coding standards.
Troubleshoot and resolve technical issues.
`,
requirements: `
Bachelor’s degree in Computer Science.
Strong Java and Spring/Hibernate experience.
Knowledge of SQL and databases.
`
},

{
title: "Senior Python Developer",
company: "TechNova Systems Pvt. Ltd",
location: "Bengaluru, India",
experience: "4+ years",
description: `
TechNova Systems provides enterprise-grade software solutions worldwide.
The role involves building scalable backend systems using Python.
`,
responsibilities: `
Develop REST APIs and backend services.
Optimize application performance.
Participate in architecture discussions.
`,
requirements: `
Strong Python skills.
Experience with Django or Flask.
Knowledge of databases.
`
},

{
title: "Full Stack Developer",
company: "BrightWave Technologies",
location: "Hyderabad, India",
experience: "3–5 years",
description: `
BrightWave Technologies specializes in modern web solutions across industries.
`,
responsibilities: `
Develop frontend and backend features.
Integrate APIs and databases.
Maintain existing applications.
`,
requirements: `
JavaScript, React, Node.js.
SQL/NoSQL databases.
`
},

{
title: "Software Test Engineer",
company: "QualitySoft Solutions Pvt. Ltd",
location: "Chennai, India",
experience: "2+ years",
description: `
QualitySoft Solutions delivers quality assurance services globally.
`,
responsibilities: `
Design and execute test cases.
Report and track defects.
Perform regression testing.
`,
requirements: `
Manual and automation testing.
Selenium knowledge.
`
},

{
title: "Data Analyst",
company: "InsightWorks Analytics",
location: "Mumbai, India",
experience: "2–4 years",
description: `
InsightWorks Analytics helps businesses make data-driven decisions.
`,
responsibilities: `
Analyze datasets.
Create dashboards and reports.
`,
requirements: `
SQL, Excel, Python or R.
`
},

{
title: "DevOps Engineer",
company: "CloudEdge Technologies",
location: "Remote, India",
experience: "4+ years",
description: `
CloudEdge Technologies focuses on cloud-native solutions.
`,
responsibilities: `
Manage CI/CD pipelines.
Automate deployments.
`,
requirements: `
AWS/Azure, Docker, Kubernetes.
`
},

{
title: "Android App Developer",
company: "AppSphere Solutions",
location: "Pune, India",
experience: "3+ years",
description: `
AppSphere Solutions builds innovative mobile applications.
`,
responsibilities: `
Develop Android apps.
Integrate REST APIs.
`,
requirements: `
Java/Kotlin, Android SDK.
`
},

{
title: "UI/UX Designer",
company: "DesignHub Pvt. Ltd",
location: "Bengaluru, India",
experience: "2–5 years",
description: `
DesignHub creates user-centric digital experiences.
`,
responsibilities: `
Design wireframes and prototypes.
Collaborate with developers.
`,
requirements: `
Figma or Adobe XD.
`
},

{
title: "Machine Learning Engineer",
company: "AI Horizon Labs",
location: "Hyderabad, India",
experience: "3+ years",
description: `
AI Horizon Labs builds intelligent ML-driven systems.
`,
responsibilities: `
Develop and evaluate ML models.
Deploy models into production.
`,
requirements: `
Python, ML libraries.
`
}
];

const container = document.getElementById("jobs");

jobs.forEach(job => {
  const div = document.createElement("div");
  div.className = "job";
  div.innerHTML = `
    <h2>${job.title}</h2>
    <p><b>Company:</b> ${job.company}</p>
    <p><b>Location:</b> ${job.location}</p>
    <p><b>Experience:</b> ${job.experience}</p>
    <div class="section-title">Description</div>
    <p>${job.description}</p>
    <div class="section-title">Responsibilities</div>
    <p>${job.responsibilities}</p>
    <div class="section-title">Requirements</div>
    <p>${job.requirements}</p>
  `;
  container.appendChild(div);
});


**Languages:**

*   [English](README.md)
*   [中文](README.zh.md)

# AI-Powered Resume Crafting Workflow

This repository outlines a structured, AI-assisted workflow for creating a professional and polished resume. By interacting with an AI assistant (like Gemini), you can systematically build your resume from scratch, ensuring all key information is captured and professionally presented.

The entire process is designed to be **resumable and stateful**. All your progress is saved in a `.gemini_task.json` file, allowing you to pause and continue at any time without losing information.

---

## The Workflow

The process is divided into three main phases:

### Phase 1: Information Gathering

This is the foundational stage where the AI assistant collects all the necessary information through a guided, conversational process.

1.  **Initialization:** A `.gemini_task.json` file is created to track the state and store all the data for your resume.
2.  **Basic Information:** Collects your name and contact details.
3.  **Personal Summary:** Guides you in writing a compelling professional summary, offering examples and suggestions tailored to different career profiles (e.g., senior expert, team collaborator, recent graduate).
4.  **Work Experience:** Systematically gathers details for each role: company, title, dates, responsibilities, and key achievements.
5.  **Project Experience:** Uses a structured approach to detail your projects, including a description, your role, responsibilities, contributions, and the tech stack used. The assistant helps refine the language to be professional and impactful.
6.  **Education:** Records your educational background.
7.  **Skills:** Automatically extracts skills from your experience, helps categorize them (e.g., programming languages, databases, cloud services), and suggests related skills you might have missed.

### Phase 2: Resume Generation & Iteration

Once the information is collected, the focus shifts to creating and refining the resume document.

8.  **Draft Generation:** The assistant compiles all the collected information into a well-structured Markdown resume. Drafts are saved with a date suffix (e.g., `resume_YYYYMMDD.md`) for version control.
9.  **Review and Refine:** This is an iterative cycle where you can request changes of any size—from fixing a typo to restructuring an entire section. The assistant can provide professional advice on different resume structures (like the STAR method) to help you make informed decisions.

### Phase 3: Final Delivery

10. **Export to PDF:** The final step is to convert the approved Markdown resume into a high-quality PDF, ready for job applications. The assistant will provide guidance on how to do this effectively.

---

## How to Use

Simply start interacting with the Gemini CLI in this project's directory. 
Input below prompt
`build resume`
The assistant will guide you through the process outlined above, starting with the initialization step.

---


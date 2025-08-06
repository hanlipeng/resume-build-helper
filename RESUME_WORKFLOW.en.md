### **Resume Crafting Workflow**

This document outlines a structured workflow for creating a professional resume.

### **Phase 0: Task Initialization and State Management**

Before any specific steps begin, a task state and data persistence file is created based on a template.

*   **Template**: Uses the `.gemini_task.json.example` file in the project root as a template.
*   **Generation**: The template's structure is read and populated with the actual data for the current resume task, generating a `.gemini_task.json` file.

This file is central to the entire collaborative process and is used for:

*   **Task Tracking**: Real-time recording of the status of each step in the resume creation process (e.g., pending, in-progress, completed).
*   **Data Persistence**: Securely storing all information collected at each stage (such as personal summary, project experience, skills list, etc.).
*   **Interruptible/Resumable**: Ensuring that our work can be paused at any time and seamlessly resumed from where it was left off, with no loss of progress or information.

### **Phase 1: Information Gathering**

1.  **Basic Information Collection**: Gathers name and contact information through a question-and-answer process.

2.  **Personal Summary Composition**:
    *   Guides the user in writing a personal summary that highlights professional strengths and career goals.
    *   When the user is unsure, proactively provides professional examples in various styles (e.g., Senior Expert, Team Collaborator, Recent Graduate) as references.

3.  **Work Experience Organization**: Collects the company, position, dates, responsibilities, and achievements for each job through a Q&A format. Allows the user to add and modify information at any time.

4.  **Project Experience Structuring**:
    *   Adopts a structured, iterative approach:
        1.  **Initial Information Collection & Framework Establishment**: Quickly builds a standardized description framework including `Project Summary`, `My Role`, `Key Responsibilities & Contributions`, and `Tech Stack` by gathering core project information (name, background, tech stack, main tasks).
        2.  **Multi-turn Dialogue & Content Refinement**: Refines details through multiple rounds of conversation to ensure accuracy.
        3.  **Professional Language Polishing**: Transforms descriptive language into more professional, high-impact resume language, using strong action verbs, emphasizing results and value, and logically categorizing the tech stack.
        4.  **Final Confirmation & Saving**: Solidifies the final version after confirmation.

5.  **Education Background Recording**: Records school, major, degree, and dates via Q&A.

6.  **Professional Skills Aggregation**:
    *   **Initial Extraction**: Automatically extracts a preliminary list of skills based on existing work and project experience.
    *   **Guided Supplementation by Category**: Guides the user to add more skills through categories (e.g., programming languages, databases, cloud services).
    *   **Proactive Association & Suggestion**: Proactively suggests related, potentially omitted skills based on the user's provided tech stack.
    *   **Final Confirmation**: Provides a clearly categorized, complete skills list for the user's final approval.

### **Phase 2: Resume Generation and Iteration**

7.  **Generate Initial Draft**:
    *   Integrates all collected and confirmed information into a well-structured Markdown resume.
    *   The resume is saved in the `resume` folder; if the folder does not exist, it is created.
    *   Uses a filename with a date suffix (e.g., `resume_YYYYMMDD.md`) for version control.

8.  **Review and Iterative Modification**:
    *   This is a cyclical process that continues until the user is fully satisfied.
    *   **Supports any level of modification**: From simple text corrections to restructuring entire sections.
    *   **Provides professional structure recommendations**: When the user wants to restructure, proactively offers various industry-standard professional structure options (e.g., STAR method, results-oriented), explaining their pros and cons to aid decision-making.
    *   **Real-time Updates & Previews**: Updates the file and provides a preview after each modification to ensure what you see is what you get.

### **Phase 3: Final Delivery**

9.  **Final Version Export**: Provides guidance on how to convert the final, confirmed Markdown file into a high-quality PDF suitable for job applications.

# PRompts

## Product Requirement Document

You are an expert Technical Product Manager specializing in source code analysis and PRD (Product Requirements Document) creation.  Given a source code folder (provided as input), your task is to generate a comprehensive PRD document describing the software product represented by that code. The PRD should be well-structured, detailed, and placed in a "docs" subfolder within the same directory as the source code.  You should infer as much information as possible from the code, including functionality, architecture, and potential user needs.  If information cannot be reliably inferred from the code, state it as an assumption or area requiring further clarification.

**Process:**

1. **Source Code Analysis:** Thoroughly examine the provided source code folder.  Pay attention to:
    * **Structure:** Directory organization, file names, and relationships between files.
    * **Content:** Code within files, including function definitions, data structures, algorithms, and comments.
    * **Technology:** Programming languages, frameworks, libraries, and any external dependencies.
    * **Functionality:** Identify core features, modules, and how they interact.  Trace data flow and control logic.

2. **PRD Generation:** Create a PRD document within a "docs" subfolder.  The PRD should adhere to the following structure and contain the specified information:

    * **1. Document Overview:** Briefly describe the purpose and scope of the PRD.
    * **2. Objective:** Define the overall goal of the software product.
    * **3. Scope:** Clearly define what is included and excluded from the product.
    * **4. User Personas and Use Cases:**
        * **Personas:** Describe representative users, their needs, and their goals.
        * **Use Cases:** Detail how users interact with the product to achieve specific goals.  Include step-by-step descriptions where possible.
    * **5. Functional Requirements:** List the specific functionalities the product must perform.  For each requirement:
        * Describe the input and expected output.
        * Specify any constraints or limitations.
        * Indicate whether the requirement is inferred or assumed.
    * **6. Non-Functional Requirements:** Describe the quality attributes of the product.  Address:
        * **Performance:**  Expected response times, throughput, etc. (If inferable)
        * **Scalability:** How the product can handle increasing load. (If inferable)
        * **Security:**  Potential vulnerabilities and security measures. (If inferable)
        * **Maintainability:** How easy it is to modify and maintain the code. (If inferable)
        * **Usability:**  How easy it is for users to interact with the product. (If inferable)
    * **7. Technical Specifications:**
        * **Technology Stack:** List all programming languages, frameworks, libraries, databases, and other technologies used.
        * **Architecture:** Describe the overall architecture of the system (if inferable).
        * **Key Components:** Identify and describe the main components of the system.
    * **8. Risks and Assumptions:**
        * **Risks:** Identify potential challenges or problems that could affect development.
        * **Assumptions:** List any assumptions made during the analysis of the source code.  Clearly distinguish between inferred information and assumptions.
    * **9. Dependencies:** List any external systems, libraries, or services that the product depends on.
    * **10. Timeline and Milestones (Optional):** If the source code suggests any development timelines or milestones, include them here.  Otherwise, state that this information is not available.
    * **11. Appendix (Optional):** Include any supporting information, such as code snippets or diagrams, if necessary.

3. **Output:** The final output should be a well-formatted PRD document (e.g., Markdown, PDF, or a similar format) located in the "docs" subfolder.

**Important Considerations:**

* **Clarity:** The PRD should be clear, concise, and easy to understand for both technical and non-technical stakeholders.
* **Completeness:** The PRD should be as complete as possible, given the information available in the source code.
* **Accuracy:** The information in the PRD should be accurate and consistent with the source code.
* **Assumptions:** Clearly state any assumptions made during the analysis.  Prioritize inferring information from the code over making assumptions.  When assumptions are necessary, explain the reasoning behind them.



### Job to be Done
```
## Job to be Done Analysis

Analyze the following solution description and create a comprehensive "Jobs to be Done" (JTBD) documentation.  Your documentation should clearly articulate the jobs that customers "hire" this solution to do.  Leverage the JTBD framework, including defining the core job, related jobs, and desired outcomes.  Use Mermaid.js diagrams to visually represent the JTBD framework and relationships between jobs whenever appropriate and helpful.

**Solution Description:**

[Insert the full solution description here.  Be as detailed as possible.]

**Instructions:**

1. **Core Job Definition:** Identify the primary job that customers are trying to get done when they use this solution.  Express this job in a concise, action-oriented statement.  Focus on the customer's goal, not the solution itself.  Use the "When [situation], I want to [motivation], so I can [desired outcome]" format.

2. **Related Jobs:** Identify any related jobs that customers might also be trying to get done alongside the core job.  These can be jobs that are:
    * **Complementary:** Jobs that are often done in conjunction with the core job.
    * **Competing:** Jobs that customers might choose to do instead of the core job.
    * **Supporting:** Jobs that make it easier to accomplish the core job.

3. **Desired Outcomes:** For each job (core and related), define the desired outcomes.  These are the specific, measurable results that customers want to achieve.  Focus on the value the customer receives, not the features of the solution.  Use metrics and quantifiable results where possible.

4. **Mermaid Diagrams:**  Use Mermaid.js to create visual representations of the JTBD framework.  Consider diagrams such as:
    * **Job Map:**  A hierarchical diagram showing the relationship between the core job and related jobs.
    * **Progress Diagram:** A diagram illustrating the steps a customer takes to get the job done.
    * **Outcome Hierarchy:** A diagram showing the relationship between desired outcomes and the overall value proposition.

5. **JTBD Documentation Format:** Organize your analysis into a clear and structured document.  Consider using headings and subheadings to separate the different sections (e.g., Core Job, Related Jobs, Desired Outcomes, Mermaid Diagrams).

6. **Example:**  (This is a simplified example - adapt it to the specific solution)

    **Core Job:** When I'm traveling for business, I want to easily manage my expenses, so I can get reimbursed quickly and without hassle.

    **Related Jobs:**
        * Complementary: When I'm traveling, I want to book flights and hotels easily.
        * Supporting: When I'm managing expenses, I want to categorize them correctly.

    **Desired Outcomes (Core Job):**
        * Submit expense reports in under 5 minutes.
        * Receive reimbursements within 2 business days.
        * Reduce errors in expense reports.

    **(Mermaid Diagram - Example Job Map):**

    ```mermaid
    graph LR
        A[Traveling for Business] --> B(Manage Expenses)
        A --> C(Book Flights/Hotels)
        B --> D(Categorize Expenses)
    ```

**Output:**  Deliver the complete JTBD documentation, including the written analysis and Mermaid.js code for the diagrams.  Ensure the diagrams render correctly.
```


## Technical Architecture Documentation

Generate comprehensive technical architecture documentation in Markdown format. This documentation should cover the overall system architecture and provide detailed documentation for each individual source code file.  Use Mermaid.js for creating diagrams wherever appropriate to visually represent the architecture, use cases, and system interactions.

**Overall System Architecture Documentation:**

Create a Markdown file (e.g., `architecture.md`) documenting the overall system architecture.  This document should include:

* **Architecture Overview:** A high-level description of the system's architecture, including its key components, their interactions, and the technologies used. Explain the architectural patterns employed (e.g., microservices, layered architecture, event-driven architecture).
* **Use Cases:** Describe the primary use cases that the system supports. For each use case, explain the user interactions, system processes, and expected outcomes.
* **System Diagrams:** Include relevant diagrams to visualize the architecture and system interactions.  Use Mermaid.js to create these diagrams. Examples include:
    * **Component Diagram:** Showing the relationships between different components.
    * **Deployment Diagram:** Illustrating how the system is deployed.
    * **Sequence Diagram:** Demonstrating the flow of messages between components for specific use cases.
    * **Class Diagram:** Showing the structure of the code and relationships between classes (if applicable and helpful).
* **Technology Stack:** List all technologies used in the system, including programming languages, frameworks, databases, and other tools.
* **Key Design Decisions:** Explain the rationale behind important architectural decisions.



## Per-File Technical Documentation:**

For *each* source code file, create a separate Markdown file (e.g., `[filename].md`).  These individual file documents should include:

* **File Overview:** A brief description of the file's purpose and functionality within the system.
* **Class/Function Descriptions:**  Detailed explanations of each class and function within the file, including their purpose, parameters, return values, and any dependencies.
* **Use Cases (Relevant to the File):** Describe any specific use cases or scenarios that this file is involved in.  Explain how the code within the file contributes to these use cases.
* **System Diagrams (If Applicable):**  If a specific file implements a significant part of the system or interacts with other components in a complex way, include a diagram to illustrate these interactions.  Use Mermaid.js.  For example:
    * **Class Interaction Diagram:** Showing how classes within the file interact.
    * **Flowchart:** Visualizing the logic within a function.
* **Code Snippets (Optional but Recommended):** Include relevant code snippets to illustrate key functionalities or complex logic.  Use proper code formatting within the Markdown document.

**Mermaid.js Usage:**

* Use Mermaid.js code blocks within the Markdown files to define the diagrams.
* Ensure that the Mermaid.js code is valid and renders correctly.

**Output:**

The output should be a collection of Markdown files: one for the overall architecture and one for each source code file.  All these files should be contained within a single directory (e.g., `docs`).

**Example (Architecture.md - Snippet):**

```markdown
## System Architecture

The system follows a microservices architecture...

### Components

* **User Service:** Handles user authentication and management.
* **Product Service:** Manages product information.

### Diagram

```mermaid
graph LR
    A[User Service] --> B(Product Service)

**Example ([filename].md - Snippet):**

```markdown
## [filename].py

This file implements the user authentication logic.

### Classes

#### UserAuthenticator

This class handles user login and password verification...

### Diagram

```mermaid
classDiagram
    class UserAuthenticator {
        +authenticate(username, password)
    }
```


### Database Schema


Create comprehensive and well-organized documentation for a database schema. The documentation should include the following:

Database Schema Overview:
Provide a high-level description of the database, including its purpose, key entities, and relationships.
List all tables, their primary keys, and a brief description of their roles.
Detailed Table Descriptions:
For each table, include:
Table name.
A description of its purpose.
A list of columns with their data types, constraints (e.g., primary key, foreign key, unique, nullable), and descriptions.
Relationships with other tables (e.g., one-to-one, one-to-many, many-to-many).
Mermaid Diagrams:
Generate ERD (Entity-Relationship Diagram) using Mermaid syntax to visually represent the database schema, including tables, columns, and relationships.
Create a system architecture diagram using Mermaid to show how the database interacts with other components of the system (e.g., APIs, applications, services).
Additional Technical Details:
Include any indexes, triggers, or stored procedures relevant to the schema.
Mention any normalization techniques applied (e.g., 1NF, 2NF, 3NF) and why they were used.
Formatting and Style:
Use clear headings, bullet points, and tables for readability.
Ensure the Mermaid diagrams are properly formatted and easy to understand.
Example:
Provide an example query that demonstrates how the schema might be used in practice (e.g., a JOIN query involving multiple tables).
Output the documentation in Markdown format, with Mermaid diagrams embedded directly in the document.



### Document source code
Write a separate, detailed technical documentation in Markdown format for each source code file in the project. Each documentation should include the following sections:

File Overview:
Provide a brief description of the file's purpose and its role in the overall system.
Mention the programming language, framework, or libraries used in the file.
Architecture:
Explain how the file fits into the broader system architecture.
Describe any modules, classes, or functions defined in the file and their responsibilities.
Include a Mermaid.js diagram to visually represent the file's structure and its interactions with other components in the system.
Use Cases:
List the primary use cases or scenarios where the file's functionality is utilized.
Provide examples of how the file is integrated into the system workflow.
Code Walkthrough:
Break down the key components of the file (e.g., classes, functions, methods) and explain their purpose, inputs, outputs, and behavior.
Include code snippets with comments to illustrate critical sections.
Dependencies:
List any external dependencies (e.g., libraries, APIs, or other files) that the file relies on.
Explain how these dependencies are used and why they are necessary.
System Diagrams (if applicable):
Use Mermaid.js to create diagrams that visually represent:
The file's role in the system architecture.
Data flow, control flow, or interaction patterns involving the file.
Relationships between the file and other components.
Error Handling and Edge Cases:
Describe how the file handles errors, exceptions, or edge cases.
Provide examples of potential issues and how they are mitigated.
Testing:
Explain how the file is tested (e.g., unit tests, integration tests).
Include examples of test cases or testing strategies relevant to the file.
Future Improvements:
Suggest potential enhancements, optimizations, or refactoring opportunities for the file.
Formatting and Style:
Use clear headings, bullet points, and code blocks for readability.
Ensure all Mermaid.js diagrams are properly formatted and easy to understand.
Output each documentation as a separate Markdown file, named after the source code file (e.g., README_<filename>.md).

### Document 3rd party
Create 3rd party dependencies documentation.  List of 3rd party modules and 3rd party services that are used.

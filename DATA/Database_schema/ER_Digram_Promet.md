Please create an Entity-Relationship (ER) diagram for a Kanban board web application based on the following requirements:

The system is a task management application with the following key entities:

1. Users - People who use the system, can create tasks and collaborate
2. Tasks - The core entity representing work items 
3. Columns - Representing the Kanban workflow states (Backlog, To-Do, Doing, Done)
4. Projects - Collections of related tasks that users can be invited to
5. Comments - Allow users to communicate about specific tasks
6. Files/Attachments - Documents or files attached to tasks
7. Focus Timer - Records time spent when a task is in the "Doing" state
8. AI Interactions - Stores user conversations with the AI chatbot

For each entity, include:
- Primary key attributes
- Important attributes based on the requirements
- Cardinality of relationships between entities
- Foreign key relationships

Important relationships to capture:
- Users can create multiple tasks
- Tasks belong to exactly one column at a time
- Tasks must be part of a project
- Only one task can be in the "Doing" column at a time per user
- Users can be assigned to multiple projects
- Each focus timer session is linked to a specific task
- AI interactions are associated with users who initiated them

The diagram should support:
- User authentication via Supabase
- Restrictions on task modifications based on ownership
- Timer functionality when tasks move to the "Doing" state
- AI-powered analysis of task data

Please design an ER diagram that captures these requirements and supports the functional needs of the application.
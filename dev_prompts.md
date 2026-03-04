
The research prevents Claude from making ignorant changes. 
The plan prevents it from making wrong changes. 
The TODO list directs implementation trajectory. 
And the implementation command lets it run without interruption once every decision has been made.

## Research prompts

> Read this folder in depth, understand how it works deeply, what it does and all its specificities. when that’s done, write a detailed report of your learnings and findings in research.md

> Study the notification system in great details, understand the intricacies of it and write a detailed research.md document with everything there is to know about how notifications work

> Go through the task scheduling flow, understand it deeply and look for potential bugs. There definitely are bugs in the system as it sometimes runs tasks that should have been cancelled. Keep researching the flow until you find all the bugs, don’t stop until all the bugs are found. When you’re done, write a detailed report of your findings in research.md

Verify that Claude actually understood the system, and correct misunderstandings before any planning happens.

## Planning prompts

> I want to build a new feature <name and description> that extends the system to perform <business outcome>. Write a detailed plan.md document outlining how to implement this. Include code snippets.

> The list endpoint should support cursor-based pagination instead of offset. Write a detailed plan.md for how to achieve this. Read source files before suggesting changes, base the plan on the actual codebase.

 Verify and edit generated plan.md file. Fix assumptions, reject approaches, add constraints, provide domain knowledge that Claude doesn’t have. Claude is excellent at understanding code, proposing solutions, and writing implementations. But it doesn’t know my product priorities, my users’ pain points, or the engineering trade-offs I’m willing to make. 

## TODO list

> Add a detailed todo list to the plan, with all the phases and individual tasks necessary to complete the plan - don’t implement yet.

## Implementation

> Implement it all. When you’re done with a task or phase, mark it as completed in the plan document. Do not stop until all tasks and phases are completed. Do not add unnecessary comments or jsdocs, do not use any or unknown types. Continuously run typecheck to make sure you’re not introducing new issues.



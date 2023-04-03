# CS555 Agile Methods for Software Development

## Aughdon Breslin, Prof. Zhongyuan Yu

### Lecture 7 - 3/21/2023

Refactoring (fun part)

- Changing the internal structure of software to make it easier to understand and cheaper to modify without changing its observable behavior.

Why fix a part that isn't broken?

- Each part of your system's code has 3 purposes:
  - Execute the functionality
  - Allow change
  - Communicate well to developers who read it

### Lecture 5 - 2/21/2023

Scrum

Today's Topics

- Origin of Scrum
  - Defined vs Empirical Processes
- Compare Plan Driven to Chaos to Scrum
- Scrum Practices
  - Process
  - Roles
  - Meetings
  - Artifacts

Origin of Scrum

- Software managers needed a process to control software projects
- Plan-based methods assumed that the development process was predictable
  - Any problem could be solved with a little more planning, but some projects required more adaptation than expected to react to changing customer requirements
- Defined vs Empirical processes

Customer Chaos Model

- Many customers asking developers for many features
- Developers try to accommodate "loudest" voices
- Leads to chaos and low morale and low productivity

Scrum Process

- Product Owner
  - Owner thinks of idea
- Product Backlog
  - Breaks it down into a list of features
- Sprint Planning
  - Break down list of features into separated tasks
- Sprint Backlog
- Sprint Execution
  - Daily Scrum
- Potentially Shippable Product Increment
- Sprint Review
  - Review the product's development, surprises, complications
  - Should include product owner
- Sprint Retrospective
  - Review the team's dynamics, work ethic
  - Should not include product owner

Scrum Roles

- Stakeholders
  - Internal stakeholders, customers, users
  - Product owner
- Scrum Team
  - Scrum master
  - Development team
  - Also product owner

Product Owner

- Represents the customer and their needs
- Agile principle #4: Business people and developers must work together daily throughout the project
- Active member of the scrum team
  - Product Visionary
    - What should the product do? What are the features? Provides user stories
  - Manages and maintains the Product Backlog of desired features
    - Sets priorities for sprints so that the developers are working on the most important features
- Responsible for ROI
- Has final say over the product and releases
  - Decides whether to release increments to customers/users

Development Team

- Small: 3-10 software developers
  - <3 may encounter skill constraints, >10 requires too much coordination
- Cross-functional
  - Possess all needed skills: development, test, specialists
- Self-organizing
  - Team chooses process, roles, and tasks, not a boss

Scrum Master

- Scrum master is a servant-leader
  - Does not make technical or business decisions
  - Developers report to the team, not to the scrum master
- Different from Plan Driven Project Manager
  - PM is responsible for accountability and enforcement
- Helps development team practice Scrum with best practices
  - Manages the Scrum artifacts (Burn Down charts, Kanban Boards)
  - Facilitates Scrum events
  - Removes impediments
- Helps product owners in several ways:
  - Finding techniques for Product Backlog management
  - Understand the project planning and facilitate Scrum events as needed

What should be considered in the Product Backlog? (Quiz Question)

- Features
  - All of the product requirements
- Technical work
  - Underlying technology like docker that is used in the project
- Knowledge acquisition
  - Serious bugs

Backlogs

- Product Backlog
  - All features needed in product or service
  - Any stakeholder can add items, including dev team
  - May include non-visible features, like underlying tech
- Release Backlog
  - Subset of Product Backlog
  - Features needed in next product release
  - Defined by the product owner
- Sprint Backlog
  - Subset of Release Backlog
  - Features to be completed in next sprint

Managing the Product Backlog

- User stories should be DEEP
- Detailed Appropriately:
  - High Priority items have more detail
- Emergent:
  - Allows frequent changes to meet changing needs
- Estimated:
  - Effort is estimated by the developers
- Prioritized:
  - Current priority assigned by Product Owner
  - Items should be continually reprioritized as project develops

Grooming the Product Backlog

- Creating and refining
  - Anyone can suggest items, tasks should be continually broken down and estimated
- Prioritizing
  - Reprioritize items to meet changing requirements, new knowledge
- Estimating
  - Always estimate how long something will take

Daily Standup Meeting

- Who: Dev Team, Scrum Master
  - Stakeholders are welcome to observe if they insist, but they cannot be asking questions, lecturing, or talking about the project
    - Developers may not want to talk about problems they are running into if stakeholders are there
- Features and priorities are "locked" for duration of sprint to create some stability
- Team meets daily to discuss progress
  - Bring up the issue during the meeting, get feedback, but have somebody help to resolve the issue after the meeting.

Sprint Review Meeting

- Who: Product Owner, Stakeholders, Dev Team, Scrum Master
  - Demonstrate features implemented during the sprint to the customer
- Review progress
  - Compare planned features to actual features
  - Re-estimate incomplete features and add to product backlog
  - Collect new features as user stories
  - Update product architecture if needed
- Reflect on sprint: What went well? What must improve?
- Brainstorm and plan for next sprint
  - Informal, no PowerPoint allowed (shouldn't be an additional stressor on the developer)

Sprint Retrospective Meeting

- Who: Development Team, Scrum Master
- Reflect on process
  - What are we doing well? What surprised us?
- Improve the process for the next sprint
- Next, start Sprint Planning for the next sprint
  - Which features are needed the most?
  - Revise the Product/Release back log
- Minimum ten minutes for reflection to improve the process

Sprint Artifacts

- Product Backlog
  - For each User Story, each task should be within To Do, In Progress, Blocked, or Done
- Burn Down Chart
  - Graphical view of accomplishments and remaining work
  - Shows estimated vs actual time taken to complete a task
  - Slope of the line is the velocity, which is used to predict the end

### Lecture 3 - 2/7/2023

Agile Culture Use Cases and User Stories

Today's Topics

- (Review) RUP and XP
- Compare cultures in Plan Driven vs Agile organizations
- Use Cases (in RUP)
- User stories (in Agile)

Plan Driven and Agile Organizations

- Compare organizations and cultures in Plan Driven and Agile organizations
  - Quiz Question: What does the red stapler in Office Space picture mean?
    - Milton loves his red stapler. He can take any L as long as red stapler is still here. The red stapler becomes his self-worth. He will sacrifice anything to keep his red stapler. In Agile, there will be someone who will die for the old deliverables, even if they are no longer relevant. This can become destructive for the team as this person will become an obstacle. For example, someone who spent years on documentation thats no longer useful may not be willing to get rid of that documentation. This prevents the team from being able to be truly agile.
  - Roles of developers, managers, and executives
    - There are a lot of projects that fail; it's the manager's responsibility to ensure the project succeeds.

Corporate Culture

| Plan Driven Cultures                           | Agile Cultures                                             |
| ---------------------------------------------- | ---------------------------------------------------------- |
| Managers assign teams                          | Self organizing teams<br /                                 |
| Individuals work for the manager               | Individuals work for the team                              |
| Individual measured on individual achievements | Individuals measured on team achievements                  |
| Manager assigns tasks                          | Team members select tasks                                  |
| Manager responsible for improvement            | Team responsible for reflection and continuous improvement |
| Infrequent deliveries                          | Frequent/continuous deliveries                             |
| Infrequent feedback from customers             | Frequent/continuous feedback from customers                |
| "Us and them" e.g., testing, Ops               | "Us" e.g., testing, Ops                                    |

What can go wrong with the team?

- Dysfunctional Teams
  - Fail to self organize: "Tell me what to do..."
  - Hostility to members: "That's not my job..."
- Inability to adapt to change
  - Losing private office is hard
- Lacking commitment

Role of Managers

| Plan Driven Cultures                           | Agile Cultures                                               |
| ---------------------------------------------- | ------------------------------------------------------------ |
| Define solutions to be implemented by the team | Asking questions while allowing the team to create the solution |
| Define roles and responsibilities              | Help team to self organize                                   |
| Leading the effort                             | Enabling the team while clearing roadblocks to success       |
| Command and Control of the team                | Trusting the team                                            |
| Manager owns the problem                       | Team owns the problem                                        |

Role of Executives

| Plan Driven Cultures                                        | Agile Cultures                                 |
| ----------------------------------------------------------- | ---------------------------------------------- |
| Clear, unchanging direction defined early in the process    | Embrace changes                                |
| Manage by business case                                     | Rapid delivery and inspection                  |
| Attempt to understand entire problem and outcome in advance | Quick prototype solutions to understand impact |

Agile doesn't work for everyone

- Not all teams successfully transition to Agile Methods
- Failure may be attributed to:
  - Lack of clarity across the team
  - Using only the worst of Waterfall and Agile together
    - Forcing frequent short deliverables without the Agile advantages
    - Inadequate training or support for Agile Methods
      - Yesterday: product manager; today: scrum master
    - Failing to use automated testing and/or continuous integration
    - Continuing to plan everything in advance and not allowing change
    - Failing to change employee performance metrics
    - Failing to inspect and adapt

Plan Driven Requirements

- Gathering requirements is typically the first step in a plan driven SDLC
- Business Analyst interviews the customer to extract features required from the system
  - Example:
    - The system shall allow the user to enter her name, address, and email.
    - The system shall be available 24/7/365 with 99% reliability.
- Business Requirements Document (BRD)
  - Formal contract between the customer and the team delivering the product

Business Requirements Document (BRD)

- All requirements are gathered and reviewed by the business analysts before handing over to development
  - Little or no discussion between customers and developers
- Describes all of the features needed by the customer
  - Functional requirements, e.g., features
  - Non-functional requires, e.g., availability
- Limitations
  - Assumption of completeness
  - Difficult to change
  - Not created by developers and thrown over the wall to the developers
- Example Domain
  - MSS: Music Streaming System
    - Spotify, Apple Music, Pandora
    - Users choose music to stream to their phone, laptop, or device
    - Web based solution

Use Cases

- Developed by Ivar Jacobson in 1980s for OO based methods
- Part of UML and RUP (Rational Unified Process)
- Each use case describes:
  - A scenario
  - The actors (may be people or systems)
  - A sequence of actions between the actors
  - An observable result of value to a particular actor
  - Actor's intention/what does the actor want?

Use Case Method

1. Identify the actors
   - Who uses the system?
   - Who gets information from the system?
   - Who provides information to the system?
   - Who supports the system?
   - What other systems interact with this system?
   - Remember that actors may be other systems?
     - MSS Example: Users, marketing, content owners, streaming servers, etc.
2. Identify the use cases
   - What are the intentions of each actor with respect to the system?
   - Give a descriptive name (Start with an action verb, keep it concise and provide short description)
     - MSS Example: Play song (play song and control playback with play, pause, skip, rewind), Explore music (search for artists, genres), Collect user profile (gather liked songs, playtime, etc.)
3. Identify actor/use case relationships
   - Draw diagrams showing the logic flow, use case relationships, and interaction possibilities
4. Outline scenarios
   - Basic Flow (sunny day scenario): Describe sequence of events in basic flow
   - Alternate Flow (rainy day scenario): Describe sequence of events in alternate flows
     - MSS Example:
       - Basic Flow: User selects song and plays from beginning to end.
       - Alternate Flow: User selects song but its not available, what happens?

MSS Use Case Method Example

1. Name: Play song
2. Brief description: The user selects a song from MSS and plays the song
3. Actors: User
4. Basic Flow:
   1. User visits MSS homepage
   2. Selects song
   3. Song plays until completion
5. Alternate Flow:
   1. User visits MSS homepage
   2. Selects song
   3. Song is not available for listening
   4. Pop-up message informs user that the song is not available

Use Cases vs. User Stories

- Use Cases - RUP (more rigorous) approach for capturing requirements
  - Focuses on the functionalities of a feature or process
- User Stories - Agile approach for capturing requirements
  - Defines the who, what, and why of a product feature

User Stories: Agile Approach

- Customers communicate their needs via short statements
  - Customers provide the user stories with help from developers
  - Each User Story is a reminder for the customer and developer to discuss the issue
- Each statement describes the goal of an actor
  - "As a user, I want ... so that ..."
- Customer should decide priority of each user story
- MSS Example Play Song:
  - "As a user I want to be able to play a song so I can listen to it from beginning to end"
  - Priority 1 (Core feature is very important)

4 C's of User Stories

- Card:
  - Short description of the user story
- Conversation:
  - A user story is a promise of a conversation between the customer and developers
- Confirmation:
  - Each user story includes tests to confirm that the feature has been delivered
- Context:
  - Provides a richer understanding of a User Story, plus how it relates to other stories

The Conversation

- The collaborative conversation facilitated by the Product Owner which involves all stakeholders and the team.
- As much as possible, this is an in-person conversation

The Confirmation

- The Product Owner must confirm that the story is complete before it can be considered "done"
- Specific acceptance criteria that is different from the current definition of "done" can be established for individual stories, but the current criteria must be well understood and agreed to by the team.
- All associated acceptance tests should be in a passing state.

User Story Components

- Title: A short handle for the story. Present tense describes what a user needs to solve their problem
- Diagrams and Pictures: Clarifying information to make sure developers are on the same page working within a system
- Acceptance Criteria: what criteria must be met for this feature to be considered complete. 

Estimating Time for User Stories

- Developers estimate how long each story will take

Planning Poker (Quiz Question)

- Goal: Estimate relative effort for each user story
- Participants:
  - Developers estimate effort
  - Scrum Master optimizes the process
  - Product Owner answers questions
- Process:
  - For each user story:
    - Describe the user story
    - Each developer assigns effort
    - Continue until consensus

Story Points

- Estimation is hard: it should consider a slew of factors

Criteria for User Stories

- Each story should add value to the customer
  - Customer write user stories (with help from developers if needed)
- Stories need to be small enough that several can be completed per iteration
  - Place big stories with several small stories
- Stories should be as independent from one another as possible
- Stories must be testable; if it cannot be tested, it is not a requirement
- Include non-functional requirements as User Stories

INVEST in User Stories

Limitations of User Stories

- What can go wrong?

User Story Limits and Solutions (Quiz Question)

- Lack of look-ahead
  - Developers need quick responses from customers
- Lack of Context
  - User Stories are expressed in simple, concise statements
- Lack of Completeness
  - Gaps may arise as the user stories and products evolve

User Story vs Use case

- Target audiences are different, use cases are high level communication between managers and developers, user stories are more specific forms of communication between developers with rigorous descriptors

### Lecture 2 - 1/31/2023

Today's Topic

- (Review) Software development method comparison
- Rational Unified Process (RUP)
- Boehm's Spiral Model
- Overview of Extreme Programming (XP)

Rational Unified Process (RUP)

- Developed at Rational Software in late 1990s after acquisition of several Object-Oriented companies
- Based on 6 Best Practices of Software Engineering
  1. Develop iteratively
  2. Manage requirements
  3. Use component-based architectures
  4. Model software visually (UML)
  5. Continuously verify software quality
  6. Control changes

Best RUP Practices

- Develop Software Iteratively
  - Solutions are too complex to get right in one pass
  - Use an iterative approach and focus on the highest risk items in each pass
  - Customer involvement
  - Accommodate changes in requirements
- Manage Requirements
  - Use cases and scenarios help to identify requirements
  - Requirements provide traceable thread from customer needs through development to end product
- Use component-based Architecture
  - Focusing on early development and baselining of a robust architecture prior to full-scale development
  - Architecture should be flexible to accommodate change
  - Focus on reusable, component-based software
- Visually model software
  - Capture structure and behavior in Unified Modeling Language (UML)
  - UML helps to visualize the system and interactions
- Verify software quality
  - Verification and Validation is part of the process, not an afterthought
  - Focus on reliability, functionality, and performance
- Control changes to software
  - Change is inevitable
  - Actively manage the change request process
  - Control, track, and monitor changes

RUP Phases

- Inception
  - Scope system for cost and budget, create basic use case model
- Elaboration
  - Mitigate risks by elaboration of use case model and design of software architecture
- Construction
  - Implement and test software
- Transition
  - Plan and execute delivery of system to customer
    - Each phase ends with a milestone; stakeholders review progress and make go/no-go decisions

RUP Disciplines

- Business modeling
  - Create and maintain traceability between business and software modules
- Requirements
  - Describe what the system should do
- Analysis and Design
  - Show how the system will be realized in the implementation phase
- Implementation
  - The system is realized through implementation of reusable components
- Test
  - Find defects as early as possible
- Deployment
  - Produce product release and deliver to users
- Configuration and Change Management
  - Manage access to project work products
- Project Management
  - Manage risks, direct  people, coordinate with other stakeholders
- Environment
  - Ensure that process, guidance and tools are available

Twelve Extreme Programming Practices

1. The Planning Game
   - Meeting that occurs once per iteration, typically weekly
   - Business people decide:
     - Scope
     - Priority
     - Release dates
   - Technical people decide:
     - Estimates of effort
     - Technical consequences
     - Process
     - Detailed scheduling
   - Advantages:
     - Reduction in time wasted on useless features
     - Greater customer appreciation of the cost of a feature
     - Less guesswork in planning
2. Small releases
   - Every release:
     - should be as small as possible
     - must completely implement its new features
     - should contain the most valuable business features
       - Contrast with RUP where you focus on the biggest risk first
   - Advantages:
     - Frequent feedback
     - Tracking
     - Reduce chance of overall project slippage 
3. Metaphor
   - Simple explanation of the project
     - Agreed upon by all members of the team
     - Simple enough for customers to understand
     - Detailed enough to drive the architecture
   - Advantages:
     - Encourages a common set of terms for the system
     - Reduction of buzz words and jargon
     - Quick and easy way to explain the system
4. Simple design
   - Runs all the tests
   - Has no duplicated logic like parallel class hierarchies
   - States every intention important to the developers
   - Has the fewest possible classes and methods
   - Advantages:
     - Time is not wasted adding superfluous functionality
     - Easier to understand what is going on
     - Refactoring and collective ownership is made possible
     - Helps keep the programmers on track
5. Testing
   - Developers continually write unit tests, which need to pass for development to continue.
   - Customers write tests to verify that the features are implemented
   - Tests are automated to become a part of the system to continuously run and ensure the system is working.
   - Advantages:
     - Unit testing promotes testing completeness
     - Test-first gives developers a goal
     - Automation gives a suite of regression tests
6. Refactoring
   - Developers restructure the system without changing its behavior to remove duplication, improve communication, simplify, or add flexibility.
     - Developers ask if they can see how to make the code simpler while maintaining functionality
   - Advantages:
     - Becomes easier to make the next changes
     - Increases the developer knowledge of the system
7. Pair programming
   - All code written with two people at one machine
   - Driver: Thinks about the best way to implement
   - Navigator:
     - Thinks about viability of whole approach
     - Thinks of new tests
     - Thinks of simpler ways
     - Switch roles frequently
   - Two heads are better than one
8. Collective ownership
   - Entire team takes responsibility for the whole of the system
   - Not everyone knows every part equally well, but everyone knows something about every part
   - If developers see an opportunity to improve the code, they go ahead and improve it
   - Advantages:
     - Helps mitigate the loss of a team member who is leaving
     - Promotes the developers to take responsibility for the system as a whole rather than parts of the system.
9. Continuous Integration
   - Integrate and test at least once per day
   - All tests must pass
   - Advantages:
     - Becomes easy to tell what broke which parts of the code
       - Problems are more-easily spotted from recently changed code
     - Reduces the duration, which is otherwise lengthy
     - Enables the short releases practice as the time required before release is minimal.
10. Sustainable pace
    - 40 hours per week; overtime is a symptom of a serious problem
    - XP only allows one week of overtime
    - Advantages:
      - People should be fresh and eager every morning.
      - Value is placed on the developers' well-being.
      - Management is forced to find real solutions.
11. Whole team
    - Customer is a member of the team
      - Real customer will use the finished system
    - Programmers need to ask questions of a real customer
      - Clarify requirements or explain what's needed
    - Customer sits with the team
      - Customer can get some other work done while sitting with programmers
12. Coding standards
    - Communication through the code
    - The least amount of overhead
    - Voluntary adoption by the whole team
    - Advantages:
      - Supports collective ownership
      - Reduces the amount of time developers spend reformatting other peoples' code
      - Reduces the need for internal commenting
      - Calls for clear, unambiguous code

### Lecture 1 - 1/24/2023

Grading

- Quizzes (30%)
- Project/Presentation (40%)
- Final Exam (20%)
- Bi-Weekly Social Media Discussion (10%)
- Participation and bonus points (+)

Syllabus

- RUP and Extreme Programming (XP)
- User Story
- Project Release
- Scrum
- Testing
- Pair Programming
- Refactoring
- Lean (Optimal Grindset)
- Crystal
- Feature-Driven Development (FDD)
- DSDM
- Scaled Agile Framework (SAFe)

Team Project

- Members:
  - unclear :(

- Evaluation:
  - Software content (50%)
  - XP and Scrum process (50%)
  - Team member evaluation (adjusted 20%)
- All deliverable are team assignments:
  - Only one member of the team needs to submit the deliverable to the Canvas
  - GitHub for Config Management

Software Development Method Comparison

- Waterfall Model
- V (Verification/Validation) Model
- Boehm's Spiral Model
- Iterative Models
- Agile Methods
- Big Bang/Chaos

Quiz Q possibly on slide 22

- How much of work is programming? 15-25% depending on group size
  - Other goes to designing, testing, team communicating

Planning

- What's the domain? How complete/stable are the requirements?
- What's the cost of mistakes/delays?
- What are the risks & rewards?

Software Development Life Cycle

- Software Specification
  - Define the functionalities
- Software Development
  - Create the code
- Software Validation
  - Verify the code works
- Software Evolution
  - Meet changing needs

|          | Sequential  | Iterative                                                    |
| -------- | ----------- | ------------------------------------------------------------ |
| Rigid    | Waterfall/V |                                                              |
| Flexible |             | Chaos/Big Bang<br />Agile Methods<br />Iterative<br />Spiral |

Waterfall

- Requirements
  - Captured in a product requirements document
- Design
  - Resulting in the software architecture
- Implementation
  - The development, proving, and integration of software
- Verification
  - Systematic discovery and debugging of defects
- Maintenance
  - Stage where the product gets transferred to the user
  - The installation, migration, support, and maintenance of complete systems

Quiz Q2 on slide 31

- When is waterfall useful?
  - Must get project right the first time
    - Interacting with hardware systems, which are difficult to change
  - Cost of failure is very high
    - Critical systems with safety or security requirements
  - Complete and stable requirements
    - Very large, multi-organizational software projects

V (Verification/Validation) SDLC Model

- Add verification/testing to each step of the waterfall model
- Most complete rigorous testing before proceeding to next step
- Verification Process
  - Requirement Gathering
    - Acceptance Test Designs
  - Functional Design
    - Functional Test Designs
  - Internal System Design
    - Integration Test Designs
  - Module Design
    - Unit Test Design
  - Coding
- Validation Process
  - Unit Testing
    - Unit Test Design
  - Integration Testing
    - Integration Test Designs
  - Functional Testing
    - Functional Test Designs
  - User Acceptance Testing
    - Acceptance Test Designs

Boehm's Spiral Model

- Incremental Development and Interactions
  1. Objective Setting
  2. Risk Assessment and Reduction
  3. Development and Validation
  4. Planning for next iteration

Iterative models SDLC

- Identify requirements up front that are mostly stable
  - Build subsets of requirements sequentially or concurrently
- Benefits
  - Parallel effort by multiple teams
  - Delivers early functionality for customers to review

Agile methods SDLC

- Umbrella term for frequent iterative/incremental programming development approaches
- Frequent iterations and deliverables
- Close collaboration between developers and customers
- Supports changing requirements
- Frequent retrospection: learn and improve from experience

Reasons to Use Agile Methods

- Big, upfront planning is not practical because of unstable or ambiguous requirements
- Delivery through small baby steps through iterative and incremental development to reduce risk
- Visibility with customers: customers are part of the team instead of observers
- Frequent reflections by team members

Big Bang/Chaos SDLC

- Little to no planning
- Figure it out as you go (typically for very small projects)
- Not highly recommended

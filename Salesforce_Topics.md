# Salesforce Study Topics

## Salesforce Basics
- Sandbox types
- Editions
- Experience Primary Clouds
- Order of Execution
- Configurations vs Configuration
- Multitenant Architecture
- Data Management
- Defer Sharing Rule Calculations
- Defer Group Membership Calculations
- Types of cloud computing (IaaS, PaaS, SaaS)

## Data Model
- Objects and Fields
- Relationships
- Record Types
- Page Layouts
- Validation Rules
- Field Dependencies
- Data Import and Export
- Field History
- Custom Metadata Types
- External Objects
- Lightning Experience (Dynamic actions, Dynamic forms)
- Limits
- Performance issue. Customer has a lot of records and reports are slow. How to fix?
- Often growing data objects. What to do?
- Customer has fields limits 500 on the object. We need to add more fields.
- How to support data quality?
- Optimal number of child records for lookup.
- Designing Enterprise Data Architecture (Logical Data Model, Data lyfecycle, Archive & Retention Strategy, Reporting Strategy)
- Data Migration
- Logic bypassing (Feature Flags)

## Salesforce Apex
- Collections
- Triggers
- Class Database
- Best Practices
- Limits (SOQL, DML, Heap, CPU)
- Class Sharing
- Async Apex
- Dynamic SOQL
- Platform Events
- Tests
- Exceptions handling
- Custom Metadata Type vs Custom Settings
- Libraries
- Dependency Injections
- Platform Cache
- Security (Apex default context, Enforce field-level security, isAccessible vs SECURITY_ENFORCED)
- How to implement Logger in Apex?
- We're hitting limits very often (CPU, Heap). How to investigate and how to solve?

## LWC
- Bundle Structure
- Component Lifecycle
- Conditional Rendering
- Events Handling
- Decorators
- Data Binding
- Loops and iterative rendering
- Nested components
- Using apex
- Styling components with CSS
- Slots
- Lightning Data Service
- Lightning Message Service
- Components Inheritance
- Navigation and routing in LWC
- Error handling
- Debugging
- Performance optimization
- Third-party libraries (d3)
- Shadow & Lightning DOM
- How to implement custom lookup component?
- Building custom base components
- Pagination implementation
- Testings
- empApi

## JavaScript
- Arrays (Built-in operators, Operations, Loops)
- Variables (Var vs Let vs Const)
- Functions (Context, this; Call, Bind, Apply; Closures; Global scope; Callbacks; Arrow functions)
- Expressions (Logical operators, == vs ===, Hoisting)
- Promises (Chaining, Callback hell (pyramid of doom), error handling, async/await, Promise.all(), Promise.any(), Promise.race())

## Flow
- Flow Types
- Use Cases (Automation)
- Building Flows (Elements, Resources, Debugging, Testing)
- Flow Execution (Record Context: Before-save vs After-save Flows, Triggering Flows via Apex or Buttons, Callouts in flows, Asynchronous flows)
- LWC usage
- Reusable Components (Subflows: modular flow design, Custom Components in Flows: Leveraging LWC)
- Error Handling (Fault Paths, Error Email Notifications, Debugging Complex Flow Errors)
- Flow Optimization and Best Practices (Performance Optimization for Large Data, Limits and Considerations)
- Deployment and Management (Deploying Flows Between Environments, Monitoring and Updating Active Flows)

## Git
- Basics (git clone, git checkout, git commit, git push, git pull, git fetch, .gitignore)
- Viewing History (git log)
- Undoing things (git reset, git amend)
- Branching (git checkout, git merge, git rebase)
- Branching Strategies
- Conflicts resolution

## Software Engineering Processes
- Methodologies (Scrum, Agile, Kanban, Waterfall, Lean)
- Estimation Techniques
- Team Management (Bus factor, Group dynamics)
- Team Performance (How to measure, High-performing Team Characteristics, How to Support Team Performance, Team Performance Challenges)
- Conflicts resolution (Open Communications, Active Listening, Identify the Root Cause, Set Clear Expectations)
- Mentoring (Experience)
- Relationships with a customer (How to establish, Clear Communication, Realistic Expectations, Ask Feedback)
- Code Quality metrics (Code Coverage, Code Duplication, Cyclomatic Complexity, Technical Debt, Code Documentation)
- Production bug resolution steps (Understand whether it's necessary to fix it or not (business needs). Prioritize bug. Who should be involved? Provide steps for resolution. Which process should be taken to fix it)
- What is Functional and Non-Functional Requirements
- Definition of Ready (DoR), Definition of Done (DoD)
- Task decomposition
- Code review process & tools

## Salesforce Security Model
- Object-level security
- Field-level security
- Record-level security
- Profiles, Permission Sets, Permission Set Groups, Muting Permissions
- Custom Permissions
- Sharing Sets
- Share Groups
- Share Object (AccountShare, ...)
- Apex Sharing (Row cause, Owner changing behavior, Share table)
- Profiles + Roles Architecture

## SOQL
- Structure (Sections, GROUP BY, HAVING, ORDER BY)
- Relationships (Nested queries, Depth)
- Aggregate functions
- WITH SECURITY_ENFORCED
- OFFSET
- Limits
- SOQL Injection Defenses
- Optimization (Indexes, Selectivity, Query Plan Tool)
- Frameworks (SOQL Builder)

## SOSL
- Structure (Sections, FIND, FORMAT, IN, LIMIT, OFFSET)
- Limits
- Performance optimization

## Integrations
- Storing credentials
- Testing
- Error handling
- Connected App
- Remote Site Settings
- Named Credentials
- HTTP (Request/Response Structure, Cookies, Methods)
- REST (Uniform interface, Client-Server, Stateless, Cacheable, Layered System, What is a Resource)
- SOAP (Envelope, Header, Body)
- SSO/User provisioning
- Identity and Access Management
- How to setup Integration from scratch (Auth methods, Volume of data, Integration Patterns, Architecture, Middleware, Mapping, Logging, Retry mechanism, FR/NFR)
- CDC
- Salesforce standard APIs (REST, SOAP, Bulk, Metadata, Streaming, Composite, Pub/Sub, GraphQL)
- Data Cloud

## Setup
- Users (Public Groups, Queues, User Management)
- Audit Trail
- Application configuration (App Manager)
- Static Resources
- Platform Events
- Salesforce AI Capabilities

## Aura
- Calling Apex
- Events Types
- Conditional rendering and Lists
- Attributes
- Bundle structure

## Visualforce
- Controllers
- View state
- JavaScript Remoting
- Pagination

## AI
- Theory (model, prompt, token, temperature, top K/P, hallucinations)
- How do you use it?
- Models (what is model? which models do you use?)
- Tools (which tools do you use?)
- Prompting Techniques
- Agentforce

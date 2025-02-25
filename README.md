![Alt Text](https://billor.us/images/logo.svg)

# Billor Coding Challenge: Financial API

## Objective

Develop a RESTful API using NestJS and PostgreSQL with a focus on financial operations. The application should manage financial accounts, transactions, and reporting in a secure, scalable, and testable architecture. This challenge is designed to thoroughly assess a developer's expertise in NestJS, database integration, and adherence to best practices in building complex financial systems.

## Functional Requirements

1. **Account Management:**
   - Implement CRUD operations for financial accounts with details such as account name, number, balance, and type (e.g., checking, savings).
   - Enforce data validation and integrity rules.

2. **Transaction Management:**
   - Support operations for deposits, withdrawals, and transfers between accounts.
   - Record each transaction with details including date, amount, type, and the involved account(s).
   - Apply business rules to prevent negative balances or invalid operations.

3. **Financial Reporting:**
   - Provide endpoints to retrieve account statements with filters by date, transaction type, etc.
   - Generate periodic (e.g., monthly) movement reports for financial analysis.

4. **Authentication and Authorization:**
   - Implement JWT-based authentication to secure the API.
   - Differentiate user roles (e.g., administrator and standard user) to control access to specific operations.

5. **Security and Data Validation:**
   - Properly handle errors and validate all inputs.
   - Implement safeguards against common vulnerabilities (e.g., SQL injection, XSS).

## Advanced Challenges

1. **Multi-Currency Support and Exchange Rate Management:**
   - Allow operations in multiple currencies.
   - Integrate with an external API to fetch current exchange rates and perform real-time conversions.

2. **Scheduled and Recurring Transactions:**
   - Enable scheduling of transactions (e.g., recurring payments or transfers).
   - Utilize background job processing (e.g., with Bull or Agenda) for executing scheduled tasks.

3. **Event-Driven Architecture:**
   - Implement an event bus to handle communication between modules.
   - Publish events for key operations (such as transaction processing or account updates) and allow other parts of the system to react accordingly.

4. **CQRS and Domain-Driven Design:**
   - Separate read and write operations using the CQRS pattern.
   - Structure the project with a focus on domain-driven design to encapsulate business logic.

5. **API Rate Limiting and Throttling:**
   - Introduce rate limiting to prevent abuse and ensure API stability under high load.

6. **Advanced Security Measures:**
   - Implement audit logging to track user activities and changes to financial data.
   - Integrate additional security measures such as account lockouts, IP whitelisting, or third-party security monitoring.

7. **GraphQL Endpoint (Optional):**
   - Provide a GraphQL interface in addition to REST, enabling more flexible and efficient data queries.

8. **Integration with External Payment Gateways:**
   - Simulate integration with payment processors to handle external transactions and refunds.

9. **Microservices Architecture (Optional):**
   - Consider decomposing parts of the API into microservices to handle scalability and separation of concerns.

10. **Real-time Notifications:**
    - Implement WebSocket-based notifications for real-time updates on transaction statuses and account activities.

11. **Comprehensive Testing Strategy:**
    - Develop a full suite of tests including unit, integration, and contract tests for API endpoints and external integrations.

12. **Containerization and CI/CD Pipeline:**
    - Containerize the application and database using Docker.
    - Set up a CI/CD pipeline for automated testing, building, and deployment.

## Technical Requirements

- **Technologies:**
  - **NestJS** as the framework.
  - **PostgreSQL** as the primary database.
  - Use an ORM such as TypeORM or Prisma for database interactions.
  - **JWT** for secure authentication and authorization.
  - **Docker** for containerization.
  - (Optional) Tools for background processing (e.g., Bull) and real-time communication (e.g., WebSockets).

- **Best Practices:**
  - Maintain a modular, scalable project structure.
  - Write clean, well-documented code.
  - Utilize design patterns and best practices in API development.
  - Manage database schema changes with migrations.
  - Implement robust error handling and logging mechanisms.

## Evaluation Criteria

- **Functionality:**  
  Does the API meet all specified requirements, including advanced features such as multi-currency support, scheduled transactions, and event-driven architecture?

- **Code Organization:**  
  Is the project structure clear, modular, and maintainable? Does it adhere to NestJS and general software development best practices?

- **Database Integration:**  
  Is the ORM integration and migration strategy well-implemented? Is the financial data model robust and scalable?

- **Security:**  
  Are authentication, authorization, and input validations effective? Are advanced security measures properly implemented?

- **Performance and Scalability:**  
  Is the API designed to handle high loads with rate limiting, background processing, and potential microservices architecture?

- **Test Coverage:**  
  Are there comprehensive tests covering unit, integration, and contract aspects of the system?

- **Documentation:**  
  Is the project, including setup and technical decisions, well-documented?

## Submission

- Host your source code on a public repository (e.g., GitHub).
- Provide clear instructions on how to set up and run the project, including environment configuration, database setup, and test execution.
- (Optional) Include a brief report explaining your technical and architectural decisions.

Good luck!

1. User Interface (UI) Layer
  - Web Application: Developed a responsive, interactive user experience.
  - Mobile Application: Carryout Web App Project to develop with Web Application
    - reason: more efficient instead split between Web and Mobile

2. Application Layer
  - Frontend:
    - VueJS 
      - VueJS Components: For building reusable UI components.
      - NuxtJS: Global Framework and Design Pattern (equvalent NextJS for react)
      - CapacitorJS: Mobile App Container for Web Development, support any kind native interactive
      - Pinia: For state management.
      - Vuetify: For UI components and Blueprints
  - Backend:
    - NestJS: For creating a scalable and maintainable API with TypeScript.

3. Business Logic Layer
  - Loan Processing Engine: Handles the core loan origination logic.
  - Workflow Automation: Orchestrates various steps like application submission, document verification, credit scoring, and approval.
  - Rule Engine: Manages business rules for loan eligibility, risk assessment, and compliance.

4. Integration Layer
  - API Gateway: Using Nginx
  - Microservices: Implemented with Docker containers, managed by Kubernetes for scalability.
  - Third-Party Integrations:
     - Credit Bureaus: For fetching credit scores.
     - Payment Gateways: to receive payment from brower
     - Document Verification Services: For KYC (Know Your Customer) compliance.

5. Data Layer
  - Database:
     - MySQL: Primary relational database with replication for high availability.
     - Redis: For caching frequently accessed data to improve performance.

6. Security Layer
  - Authentication: Using OAuth2 and JWT for secure user authentication.
  - Authorization: Role-based access control (RBAC) to manage user permissions. (ex: user:read, user:delete)
  - Data Encryption: Encrypting sensitive data at rest and in transit using SSL/TLS.

7. DevOps Layer
  - CI/CD Pipeline: GitHub Actions for continuous integration and delivery.
  - Infrastructure as Code: AWS CloudFormation for managing infrastructure.
  - Monitoring and Logging:
     - Monitor: Grafana for monitoring system performance.
     - Logging (ELK stack):
       - Logstash: convert any log from service to structured data
       - Elasticseach: Fast query logging
       - Kibana: for log visualization

8. Cloud Services
  - AWS Services:
    - EC2: For hosting application servers.
    - S3: For storing documents and media.
    - RDS: Managed MySQL database service.
    - Lambda: For serverless functions handling specific tasks.

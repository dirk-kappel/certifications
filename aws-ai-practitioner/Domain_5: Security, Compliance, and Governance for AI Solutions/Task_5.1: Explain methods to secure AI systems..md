## Identify AWS services and features to secure AI systems (for example, IAM roles, policies, and permissions; encryption; Amazon Macie; AWS PrivateLink; AWS shared responsibility model).
**IAM Roles, Policies, and Permissions**:
- AWS Identity and Access Management (IAM) enables fine-grained control over who can access AI services and resources, ensuring that only authorized users and services have appropriate permissions.

**Encryption**:
- Ensures data is protected both in transit (using SSL/TLS) and at rest (using AWS services like KMS for encryption). It is essential for protecting sensitive information during model training and deployment.

**Amazon Macie**:
- A machine learning-powered service that helps discover, classify, and protect sensitive data, such as personally identifiable information (PII), in AI systems.

**AWS PrivateLink**:
- Provides private connectivity between VPCs and services in AWS, ensuring secure communication for AI models and data processing without exposing traffic to the public internet.

**AWS Shared Responsibility Model**:
- Outlines the division of security responsibilities between AWS and the customer, with AWS securing the cloud infrastructure and the customer securing their AI models, data, and applications.

## Understand the concept of source citation and documenting data origins (for example, data lineage, data cataloging, SageMaker Model Cards).
**Data Lineage**:
- Tracking the flow of data from its original source to its final destination, ensuring transparency and accountability in data usage for AI systems.

**Data Cataloging**:
- Organizing and documenting metadata to make data discoverable, accessible, and understandable, helping teams to trace where data came from and how it was used.

**SageMaker Model Cards**:
- Amazon SageMaker provides Model Cards, which include details on model performance, limitations, data sources, and ethical considerations, ensuring proper documentation and citation of data origins.

## Describe best practices for secure data engineering (for example, assessing data quality, implementing privacy-enhancing technologies, data access control, data integrity).
**Assessing Data Quality**:
- Regularly check data for accuracy, completeness, and consistency to ensure it’s suitable for training AI models.

**Implementing Privacy-Enhancing Technologies**:
- Utilize techniques like data anonymization, differential privacy, or federated learning to safeguard sensitive information during model training and inference.

**Data Access Control**:
- Enforce role-based access control (RBAC) or attribute-based access control (ABAC) to limit who can view or modify data, ensuring only authorized personnel or systems can access sensitive data.

**Data Integrity**:
- Implement checksums, hashes, or digital signatures to verify that data has not been tampered with during storage, processing, or transmission.

## Understand security and privacy considerations for AI systems (for example, application security, threat detection, vulnerability management, infrastructure protection, prompt injection, encryption at rest and in transit).
**Application Security**:
- Ensure that AI models and applications are secure by design, using techniques like code reviews, vulnerability scanning, and penetration testing to identify and address potential risks.

**Threat Detection**:
- Use AWS services like Amazon GuardDuty to monitor for unusual activity, malicious behavior, or unauthorized access within the AI system.

**Vulnerability Management**:
- Regularly update and patch software dependencies, AI frameworks, and infrastructure to fix known security vulnerabilities.

**Infrastructure Protection**:
- Protect AI models and data by securing cloud infrastructure using network security (VPC, security groups) and physical security features offered by AWS.

**Prompt Injection**:
- Prevent adversarial attacks where malicious inputs (e.g., prompts) are designed to manipulate AI models into generating harmful outputs, using input validation and model defense techniques.

**Encryption at Rest and in Transit**:
- Encrypt all sensitive data both during storage (at rest) and when being transferred over networks (in transit) to ensure privacy and protect against data breaches.

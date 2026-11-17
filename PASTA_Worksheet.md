# PASTA Threat Model Worksheet: Sneaker company

Completed threat modeling analysis of the **Process of Attack Simulation and Threat Analysis (PASTA)** framework.

## I. Define business and security objectives

Make 2-3 notes of specific business requirements that will be analyzed.
- Will the app process transactions?
- Does it do a lot of back-end processing?
- Are there industry regulations that need to be considered?
_______
- Buyers should directly message sellers with questions and have the ability to rate sellers to encourage good service
- Users should have several payment options 
- Proper payment handling is important to avoid legal issues

## II. Define the technical scope

List of technologies used by the application:
- Application programming interface (API)
- Public key infrastructure (PKI)
- SHA-256
- SQL

Write 2-3 sentences (40-60 words) that describe why you choose to prioritize that technology over the others.
_______
Prioritize SQL for proper payment handling and avoidance of SQL injection to prevent legal issues and data manipulation or theft. SQL directly interferes in the database that contains sensitive customer and seller information, including PII and transaction records. To ensure business regulatory compliance is met, this technology should be prioritized.

## III. Decompose application

![PASTA Data Flow Diagram](./data_flow_diagram.png)

## IV. Threat analysis

List 2 types of threats in the PASTA worksheet that are risks to the information being handled by the application.
- What are the internal threats?
- What are the external threats?
_______
SQL Injection and Unauthorized API access 

## V. Vulnerability analysis

List 2 vulnerabilities in the PASTA worksheet that could be exploited.
- Could there be things wrong with the codebase?
- Could there be weaknesses in the database?
- Could there be flaws in the network?
_______
Lack of prepared statements and Broken API token

## VI. Attack modeling

![PASTA Attack Tree](./attack_tree.png)

## VII. Risk analysis and impact

List 4 security controls that you’ve learned about that can reduce risk.
_______
- Password policy
- Principle of least privilege
- SHA-256
- Incident response procedures

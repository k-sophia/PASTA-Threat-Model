# PASTA-Threat-Model

Project originally completed as part of the **Google Cybersecurity Professional Certificate (Coursera)** (titled *“Apply the PASTA threat model framework”*)

## 🛡️ Scenario (from Coursera)

A company for sneaker enthusiasts and collectors is preparing to launch a mobile app that makes it easy for their customers to buy and sell shoes. 

Perform a threat model of the application using the **PASTA framework**. Go through each of the seven stages of the framework to identify security requirements for the new sneaker company app.


### 📋 Business Description
> *"Our application should seamlessly connect sellers and shoppers. It should be easy for users to sign-up, log in, and manage their accounts. Data privacy is a big concern for us. We want users to feel confident that we’re being responsible with their information.*
>
> *Buyers should be able to directly message sellers with questions. They should also have the ability to rate sellers to encourage good service. Sales should be clear and quick to process. Users should have several payment options for a smooth checkout process. Proper payment handling is really important because we want to avoid legal issues."*

### 💻 Technology Stack
The app will be exchanging and storing user data using the following technologies:
- **Application Programming Interface (API):** Uses third-party APIs to add functionality without having to program it from scratch.
- **Public Key Infrastructure (PKI):** Uses symmetric encryption (AES) to encrypt sensitive data (such as credit card information) and asymmetric encryption (RSA) to exchange keys between the app and a user's device.
- **SHA-256:** Uses to protect sensitive user data, like passwords and credit card numbers.
- **Structured Query Language (SQL):** Uses SQL to store information about the sneakers and the sellers, and to access data during a purchase.


## 📊 PASTA Framework Methodology

| Stage | Objective | Project Activity |
| :--- | :--- | :--- |
| **I. Define Business Objectives** | Identify business goals, functional requirements, and compliance constraints. | Make 2–3 notes of business objectives identified from the business description. |
| **II. Define Technical Scope** | Evaluate the architecture and prioritize high-risk technologies. | Write 2–3 sentences (40–60 words) describing why one technology is prioritized over the others. |
| **III. Decompose Application** | Map how components communicate and process data across layers. | Review the Data Flow Diagram and consider how the evaluated technologies protect user data during processes. |
| **IV. Threat Analysis** | Identify potential threats targeting scoped technologies and data flows. | List 2 types of threats that pose risks to the information handled by the sneaker company's app. |
| **V. Vulnerability Analysis** | Pinpoint exploitable weaknesses in the design, database, or codebase. | List 2 types of vulnerabilities that could be exploited. |
| **VI. Attack Modeling** | Connect assets, threats, and vulnerabilities into viable exploitation paths. | Review the Attack Tree diagram and consider how threat actors can potentially exploit these attack vectors. |
| **VII. Risk Analysis & Impact** | Select security controls to mitigate identified risks before launch. | List 4 security controls that can reduce the chances of a security incident. |


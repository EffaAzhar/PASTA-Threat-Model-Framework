# PASTA-Threat-Model-Framework
# What is PASTA:
The Process for Attack Simulation and Threat Analysis (PASTA) is a risk-centric threat modeling framework. It's designed to help organizations identify and analyze potential security threats in a way that aligns with their business objectives. This makes it a more practical and effective approach for many organizations.

**Key Features of PASTA:**
* **Risk-Centric:** PASTA emphasizes the importance of understanding and prioritizing risks based on their potential impact on the business.
* **Business Alignment:** It helps align security efforts with business objectives and compliance requirements.
* **Stages of PASTA:** it has 7 stages
    1. **Define Business and Security Objectives:** Decide goals and objectives of the threat modeling exercise.
    2. **Define Technical Scope:** Identify the system components and data flows to be analyzed.
    3. **Decompose the Application:** Identify existing controls that will protect data from threats and make data flow daigram. Break down the application into smaller, more                                            manageable components.
    4. **Perform a Threat Analysis:** Identify potential threats and vulnerabilities. Reasearch to collect most up-to-date information on the type of attacks being used.
    5. **Perform Vulnerability Analysis:** Assess the severity and exploitability of identified vulnerabilities.
    6. **Conduct Attack Modeling:** Test vulnerabilities that were analyzed in stage five by stimulating attacks. It is done by creating Attack Tree.
    7. **Analyze Risk and Impact:** Evaluate the likelihood and impact of potential attacks.

# Apply PASTA on Given Scenario:
Using the Process of Attack Simulation and Threat Analysis (PASTA) threat model framework to determine whether a new shopping app is safe to launch.
Review the following scenario. You’re part of the growing security team at a company for sneaker enthusiasts and collectors. The business is preparing to launch a mobile app that makes it easy for their customers to buy and sell shoes. You are performing a threat model of the application using the PASTA framework. You will go through each of the seven stages of the framework to identify security requirements for the new sneaker company app.

# Stages of PASTA:
1. **Identify Mobile APP Business Objectives:** Mobile app is developed to seamleesly connect sellers and shopper. Objectives of the app are:
    * It should be easy for users to sign-up, log in, and manage their accounts.
    * Buyers should be able to directly message sellers with questions
    * Data privacy is the big concern beacuse App includes bank transection and  proper payment handling is really important because we want to avoid legal issues.
2. **Define Technical Scope:** List of technologies used by the application:
    * Application programming interface (API)
    * Public key infrastructure (PKI)
    * SHA-256
    * SQL


      First Evaluate Application Programming Interface (API) for PASTA threat modeling because APIs are often entry points for attackers and can expose sensitive data if not             properly secured. Focusing on API security within a risk-centric framework like PASTA allows for the identification and mitigation of vulnerabilities that could have               significant business impact

3. **Decompose the Application:**
4. **Perform a Threat Analysis:** Two types of threats in the PASTA worksheet that are risks to the information being handled by the application.  injections and Session Hijacking.
5. **Perform Vulnerability Analysis:** Considering the attack surface of the technologies listed in Stage 2 following vulnerabilities are listed;
    * Compromised Keys: If private keys are compromised, attackers can impersonate legitimate entities and intercept or manipulate communications.
    * Broken API Token: Attackers can use a compromised token to gain unauthorized access.
    * SQL Injection: Failing to properly sanitize user input can lead to SQL injection vulnerabilities, allowing attackers to execute malicious SQL code.
    * Broken Authentication: Weak authentication mechanisms or flaws in authentication processes can allow attackers to bypass authentication and gain unauthorized access.
    * Lack of Rate Limiting: Without rate limiting, attackers can overload the API with requests, leading to denial-of-service (DoS) attacks.
6. **Conduct Attack Modeling:**
7. **Analyze Risk and Impact:** Foloowing are security controls to counter security threats:
    * **Implement Principle of Least Privilidge:** Users are granted access only to the specific resources.
    * **Prepare Staement:** a coding technique that execute SQL statements before passing them onto database.
    * **Input Sanitization:** programming that removes user input which interpreted as a code.
    * **Multi-factor authentication (MFA):** Require users to provide multiple factors for authentication (e.g., password, one-time code, biometric verification)
    * **Short session timeouts:** Automatically log users out after a period of inactivity.
    * **Regenerate session IDs:** Issue a new session ID after every successful login or at regular intervals.

 

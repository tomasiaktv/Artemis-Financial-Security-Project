# Artemis-Financial-Security-Project
Project Summary

Artemis Financial is a consulting company that develops individualized financial plans for its clients, including retirement planning, investments, savings, and insurance strategies. The company wanted to modernize its public web application and strengthen its software security practices. Specifically, Artemis Financial required the implementation of secure communication using HTTPS and the addition of a cryptographic checksum verification process to ensure data integrity during transmission.

The primary issue addressed was improving the security of client financial data by implementing encryption mechanisms, verifying file integrity through hashing, and performing vulnerability analysis on application dependencies.

Identifying Security Vulnerabilities

During the vulnerability assessment process, I analyzed the application architecture, reviewed dependencies, and evaluated potential cryptographic weaknesses. One key strength of my approach was implementing SHA-256 as a secure hashing algorithm instead of weaker deprecated algorithms such as MD5 or SHA-1. I also upgraded the application to enforce HTTPS using TLS encryption.

Coding securely is critical because financial applications manage sensitive personal and financial information. A security breach could result in financial loss, identity theft, reputational damage, and legal consequences. Strong security practices protect both customers and the company’s long-term stability.

Software security adds value by increasing customer trust, reducing risk exposure, ensuring regulatory compliance, and protecting intellectual property.

Challenges and Learning Experience

One challenging part of the vulnerability assessment was configuring and running OWASP Dependency-Check due to modern NVD API requirements and environment configuration issues. However, this process was valuable because it demonstrated how third-party dependencies can introduce vulnerabilities even when custom code is secure.

This experience reinforced the importance of maintaining updated frameworks and regularly scanning software components for known security flaws.

Increasing Layers of Security

I increased layers of security in several ways:

Implemented SHA-256 cryptographic hashing for checksum verification

Configured HTTPS with a self-signed SSL certificate

Refactored code to encapsulate cryptographic logic securely

Performed static analysis using OWASP Dependency-Check

Conducted manual functional testing to ensure no runtime errors

In the future, I would continue using static analysis tools such as OWASP Dependency-Check, SonarQube, and Snyk to assess vulnerabilities. I would also apply regular dependency updates and follow secure development lifecycle practices to decide on appropriate mitigation strategies.

Ensuring Functionality and Security

After refactoring the code, I verified functionality by:

Running the application and confirming successful startup

Accessing the secure HTTPS endpoint

Validating correct SHA-256 checksum generation

Reviewing console logs for errors

Running dependency vulnerability scans

To ensure no new vulnerabilities were introduced, I relied on both automated scanning tools and manual code review.

Tools, Resources, and Practices Used

Java Keytool for certificate generation

SHA-256 hashing via Java MessageDigest

Spring Boot SSL configuration

OWASP Dependency-Check for static vulnerability analysis

Secure coding best practices (encapsulation, avoiding deprecated algorithms)

Manual runtime and functional testing

These tools and practices will be useful in future projects involving secure web application development and vulnerability analysis.

Portfolio Value

For future employers, this project demonstrates:

Ability to perform a vulnerability assessment

Understanding of cryptographic principles

Implementation of HTTPS and TLS security

Secure code refactoring

Use of industry-standard security analysis tools

Knowledge of layered security architecture

This artifact showcases both technical implementation skills and secure development methodology, which are critical competencies in modern software engineering and cybersecurity roles.

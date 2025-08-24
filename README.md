# CS-305-Vulnerabilities-Assessment

 Artemis Financial asked me to examine & refactor their Java/Spring application for security vulnerabilities and create secure transmissions. I implemented a /hash feature with SHA-384 and configured HTTPS on 8443 using a keystore while validating results with a dependency scan.

I limited changes to what was required, added no new libraries, enabled TLS, and used a modern SHA-2 hash to strengthen integrity without widening the attack surface. Secure coding protects data and reputation while reducing incident and compliance costs.

The APIs and Input Validation review was what I found to be the most challenging because auto-exposed REST endpoints and user-supplied Spring Expression Language required tighter controls to prevent injection and unauthorized actions. The pom.xml and OWASP Report was most helpful. It quickly showed which dependencies were outdated, which gave me a clear solution to reduce known risks.

I added HTTPS on port 8443 for transport encryption and used SHA-384 for data integrity. In the future, I’d pair frequent dependency scanning with frequent code reviews. I would also update outdated dependencies to minimize risk.

I ran the app under HTTPS and verified the /hash endpoint responded correctly without errors. After refactoring, I rescanned with the OWASP Dependency Check to confirm no new vulnerable components were introduced by my changes.

Spring Boot SSL configuration, Java keytool, OWASP Dependency Check, and Eclipse were effective tools and easy to use. Some practices I will use in the future include keeping changes small, documenting them, and testing frequently.

In the future I can show my potential employers my proficiency with Dependency Check Report and my analysis based on it. I can showcase my refactor which demonstrates secure code. Together, they show I can harden an app, validate results, and document the security impact clearly.

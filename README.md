[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/W1FDCaWn)
# CECS 378 Reading Assignment: Introduction to Computer Security
## 20 Points

### Assignment Description
Answer the following questions from the chapter 1 reading ftyprom your textbook. You may work on these questions with one or two other partners, but *all* students must submit the document individually in their own repositories along with each student's name documented with the submission.

1. Define the term *computer security*.
   - In other words, Computer Security is the measurement and the operation that involves the three CIA Triads confidentiality, integrity, and availability of information system assets including hardware, software, firmware, and information being processed, stored, and communicated. 

2. What is the difference between passive and active security threats?
   - Passive threats are an attempt to make use of the information from the system that does not affect system resources. In contrast to passive threats, an active threat is an attempt to alter system resources or affect their operation. 

3. Explain the difference between an attack surface and an attack tree.
   - A surface attack consists of reachable and exploitable vulnerabilities in a system. For instance, public ports through Webs and other servers, and code listening on other ports. Another example of an attack surface is the code that processes incoming data, email, XML, office documents, and industry-specific custom data exchange formats.
   -  In other words, an attack tree is a branching, hierarchical data structure that represents a set of potential techniques for exploiting security vulnerabilities. The use of attack trees is meant to effectively make use of information available on attack patterns. For instance, an organization named CERT published security advisories to enable the implementation of a body of knowledge about general attack strategies and specific attack patterns. 

4. Consider an automated teller machine (ATM) in which users provide a personal identification number (PIN) and a card for account access. Give examples of confidentiality, integrity, and availability requirements associated with the system and, in each case, indicate the degree of importance of the requirement.
   - An ATM that is associated with confidentiality uses a visa or a credit card with a card number, an expiration date, and an account balance used for purchasing stuff that would be saved in a bank account. So this would be placed under the lower security risk.
   - Now an ATM that is associated with integrity ensures that there will be no protection since the attacker is able to alter the information in the system. So in this case, the ATM associated with this Triad would be at the medium security risk.
     - Availability: In a physical environment, an ATM can be available anywhere for anybody with a card to transfer money physically so the degree of importance would be at a higher level. 

5. Repeat question #4 for a telephone switching system that routes calls through a switching network based on the telephone number requested by the caller.
   - Integrity: Anybody with expertise in hacking can be able to listen in between two callers. In this case, this goes under the category of high-security risk
   - Confidentiality: Two callers being on the phone are collectively recorded. This is placed under medium security risk
   - Availability: Telephones can be physically available in public tourist places, so in this case, this is potentially a low-security risk
     
6. List and briefly define the fundamental security design principles.
   * Economy of Mechanism: the design of security that measures embodied in both hardware and software should be as simple and small as possible.
   * Fail-safe defaults: The accessibility of decisions should be based on permission rather than exclusion.
   * Complete mediation: means that every access must be carefully considered when adjusting privacy through access control.
   * Open design: means that the design of a security mechanism should be public rather than keep it private. 
   * Separation of privilege: defined as a practice in which multiple privilege attributes are required to achieve access to a restricted resource. 
   * Least privilege: means every process and every user of the system should operate using the least set of privileges necessary to perform the task. 
   * Least common mechanism: means the design should minimize the functions shared by different users, providing mutual security.
   * Psychological acceptability indicates that security mechanisms should not interfere with the work of users, and simultaneously meet the needs of those who authorize access. In addition to security mechanisms, these should be transparent to the users of the system and must comprehend the user’s model of protection. 
   * Isolation is one of the principles that apply to three contexts. To prevent disclosure or tampering, public access systems must be separated from critical processes such as data, processes, etc. If the information of the system is of high standards, then organizations should restrict numerous systems to isolate each data in each system in a physical or logical way. If an organization is going to handle it in physical isolation, then there should be no physical connection between an organization’s public access information and an organization’s critical information. Now in a logical way of handling it, deep layers of security services should be made between public systems and security systems that are responsible for protecting critical information.
   * Encapsulation is defined as a specific form of isolation based on object-oriented functionality. Protection is provided by encapsulating a collection of procedures and data objects in a domain of its own so that the internal structure of a data object is accessible only to the procedures of the protected subsystem 
   * Modularity defines one of the principles that refers to both the development of security functions, protected modules, and the use of modular architecture for mechanism design and implementation. The design goal of this principle is to correctly set up common security functions and services, for instance, numerous applications utilize cryptographic functions as common modules. Another secure design goal is to create a common cryptographic module that can be invoked by numerous protocols and applications. These goals will ensure that the security mechanisms will have enough functions and procedures to protect the module from tampering. 
   * Layering is the use of multiple protection approaches to address the people, technology, and operational functions of information systems. In using multiple, overlapping protection approaches, the circumvention of any individual protection will not leave the system unprotected. 
   * Least astonishment indicates a user interface should often communicate in a way that is least likely to astonish the user. For instance, the mechanism for authorization should be transparent enough for a user who has an excellent intuitive understanding of how the security goals map to the security mechanism.


8. Consider a desktop publishing system used to produce documents for various organizations.
    1. Give an example of a type of publication for which confidentiality of the stored data is the most important requirement.
          - Published articles are confidential to readers who purchase a subscription to a particular website to read the articles on the Internet. 
    2. Give an example of a type of publication in which data integrity is the most important requirement.
          - A handbook that exemplifies a type of publication in data integrity is read by other editors to make adjustments for an updated version. 
    3. Give an example in which system availability is the most important requirement.
          - Magazines would be a useful example for availability since these can be picked up by people in public tourist places. 
9. For each of the following assets, assign a low, moderate, or high impact level for the loss of confidentiality, availability, and integrity, respectively. Justify your answers.
    1. An organization managing public information on its Web server.
          C: H -> By means of a public website could result in getting hacked if personal information is shared with the public
          I: M -> As long as it's a public website with a set of restrictions to prevent hackers from altering the information, then no one would alter it. Otherwise, it could be hacked if it isn't secured
          A: L -> Individuals can have access to the web server since it's made public to everyone 

    2. A law enforcement organization managing extremely sensitive investigative information.
          C: L -> The organization can tell an individual sensitive information to keep a low profile 
          I: H -> A dangerous hacker could obtain the contents of the information and share it with the public
          A: M -> Sensitive info wouldn't be available physically in public unless someone who had the information can share it with individuals 
       
    3. A financial organization managing routine administrative information (not privacy-related information).
          C: M -> A bank manager to an individual who has a credit card with a PIN number can be intended to keep a secret 
          I: H -> An anonymous can easily hack the financial information if it is a public website
          A: L -> The information is available to users who can have access to it. 
   
    4. An information system used for large acquisitions in a contracting organization contains both sensitive, pre-solicitation phase contract information and routine administrative information. Assess the impact for the two data sets separately and the information system as a whole.
          C: L -> The customer can ensure that it is kept a secret from the company with a set of restrictions
          I: M -> The information in their system could be potentially hacked if the website isn't secured with public information being shared
          A: H -> Within a high risk of availability, there could be a problem where users can't have access to the information 
    5. A power plant contains a SCADA (supervisory control and data acquisition) system con- trolling the distribution of electric power for a large military installation. The SCADA system contains both real-time sensor data and routine administrative information. Assess the impact for the two data sets separately and the information system as a whole 
          C: H -> In high-risk security, the information could be compromised if the information is shared with an unauthorized user in the system 
          I: L -> In a lower-risk organization, the data and the information are being monitored at all times with less significant problems
          A: M -> Ensures that some users face moderate problems associated with their services 

10. Develop an attack tree for gaining access to the contents of a physical safe.

    1. Priority: Gain access to the contents of a physical safe
  
    2. Bypass the physical lock mechanism
          * Pick the lock to bypass the physical lock machine
               - Utilize lock-picking tools
               - Skilled in lock-picking
          * Know the combination
               - Make multiple attempts to guess the combination
               - Use the brute force attack to know the hidden combination
               - Observe and eavesdrop to know the combination
          * Get a copy of the key
               - Cast a variety of techniques to create a copy of the key
               - Take back the original key
           
    3. Breach the physical barriers
          *  Smash the safe
               - Use brute force methods such as detonators to breach the safe
          * Turn off the security mechanisms
               - Disarm cameras in the perimeter
               - Find a vulnerability that will manipulate the security systems of the lock
               - Override the codes to gain access with expertise in professional hacking
    4. Scroll through the contents with indirect means
          * Get a public key through authorized personnel
               - Utilize social engineering skills
               - Steal the physical keys or credentials of authorized personnel
          * Get the restricted contents while being authorized
               - Finally, gain access to coerce authorized personnel 
11. Consider the following general code for allowing access to a resource:
    ```
    DWORD dwRet = IsAccessAllowed(...);
    if (dwRet == ERROR_ACCESS_DENIED) { // Security check failed.
    // Inform user that access is denied. } else {
    // Security check OK.
    }
    ```
    1. Explain the security flaw in this program.
          - In the code above, it will ensure that access is denied. Otherwise, the security check is okay. If someone has access to the security features, then the IsAccessAllowed function fails. However, it should check for success and only a user is in the system if access is allowed. 
    2. Rewrite the code to avoid the flaw
    (Hint: Consider the design principle of fail-safe defaults).

       DWORD dwRet = IsAccessAllowed(...);

       if (dwRet == ALLOWED_ACCESS) {
          // Security check is successful
       }

       else {
          // Security check is denied
          // The user must be informed that access is denied
       } 

### Deliverables
Commit the answers to the questions in a readable file to your git repository by the due date and time indicated with your repository. Approved file submission formats are: .txt, .md, .pdf. .html (renderable) or anything that is web-readable on Github. Other formats will only be accepted with explicit approval.

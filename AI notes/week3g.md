### **CS 487 - Week 3: Awareness of User Needs**

---

#### **1. Introduction to Requirements Engineering**
- **Requirements Engineering** is the process of defining, documenting, and maintaining software requirements.
- The main objective is to understand **user needs** and constraints in the context of the environment and then ensure the system is designed to meet those needs.
  
---

#### **2. Types of Requirements**
   - **Functional Requirements**: 
     - Describe **what the system should do** (e.g., how the system reacts to inputs, how it behaves in certain situations).
     - These directly relate to user tasks and behaviors.
   - **Non-Functional Requirements**:
     - Define constraints on the system's **performance, usability, and security**. These typically apply to the system as a whole (e.g., execution speed, reliability).
     - Can be categorized as:
       - **Product Requirements**: Speed, reliability, usability.
       - **Organizational Requirements**: Policies, methodologies, delivery timelines.
       - **External Requirements**: Legal standards, interoperability with other systems.
   - **Domain Requirements**: Specific to the field of the system's use. For example, a banking system might have domain-specific requirements related to transaction security.

---

#### **3. User Requirement Challenges**
- **Ambiguity**: 
   - Achieving clarity is difficult due to the brevity expected in requirement documents. **Human language** can be vague, and users, engineers, and systems often "speak" in different languages.
   - Example: When users say "fast," it can mean different things to different people. Does fast mean 2 seconds or 10 seconds? This needs clarification.
  
- **Confusion**: 
   - Misunderstanding arises when requirements are mistaken for goals or design choices. It’s important to clearly differentiate **functional requirements**, **non-functional requirements**, and **system goals**.

---

#### **4. Requirement Capture Techniques**
   - **Interviewing Stakeholders**: Understanding user workflows, constraints, and business objectives.
   - **Ethnography**: Observing users in their actual work environments to understand real-world challenges and unarticulated needs.
   - **Use Cases**: Defining interactions between the user and the system, identifying scenarios that describe how users accomplish their goals using the system.

---

#### **5. Requirements Validation**
   - Requirements must be validated to ensure they are **complete**, **consistent**, **realistic**, and **verifiable**.
   - A common method of validating requirements is by ensuring that each requirement can be tested. This is closely related to **user acceptance testing (UAT)**, where the system is tested to verify it meets the users' needs.

---

#### **6. Requirements and Testing**
   - **User Acceptance Testing (UAT)** is where the **final product** is tested against the users' needs to verify that it meets the functional requirements.
   - The relationship between requirements and testing is integral, as a **violation of a requirement** results in a **failed test**. This makes requirements the basis not only for system design but also for testing procedures.

---

#### **7. The Iterative Approach**
   - Instead of the **waterfall model**, an **iterative model** is suggested:
     - Develop a small, functioning portion of the system (Version 1).
     - Present it to users for feedback and refine in subsequent iterations (Version 2, 3, etc.).
     - This process of **“surfacing” periodically** ensures users can provide feedback throughout development, reducing the chances of misunderstanding requirements.
     - The approach allows for continuous refinement of the system until it matches user expectations.

---

#### **8. Functional vs. Non-Functional Requirements**
   - **Functional Requirements**:
     - Examples: The system must allow users to create accounts, generate reports, or process transactions.
   - **Non-Functional Requirements**:
     - Speed: How quickly the system responds (e.g., the system must generate a report within 5 seconds).
     - Security: The level of protection required (e.g., the system must prevent unauthorized access).

---

#### **9. Challenges in Gathering Requirements**
   - **Communication Barriers**: Users and developers often have different vocabularies. The terminology gap makes it difficult for users to express what they want clearly.
   - **Scope Management**: Ensuring the project doesn’t expand uncontrollably due to unclear requirements or constant changes in user expectations.
   - **Changes Over Time**: Requirements can shift over the course of development. Iterative processes help manage this by delivering incremental updates.

---

#### **10. Capturing Requirements Effectively (H-H-I)**
   - To ensure requirements are captured correctly:
     1. **Human to Human Interaction (H-H)**: Open communication between users and engineers to understand needs.
     2. **Human to System Interaction (H-S)**: Understanding how the system should work to serve the users.
     3. **System to System Interaction (S-S)**: Ensuring system interoperability and seamless communication between subsystems.

---

#### **11. System Documentation**
   - A well-organized **requirements document** includes:
     - **Introduction**: Scope and purpose of the system.
     - **User Requirements**: Detailed functional needs from a user's perspective.
     - **System Requirements**: Technical specifications.
     - **Glossary**: Definitions of technical terms.
     - **Appendices**: Any additional relevant information.

---

#### **12. Ethnography in Software Engineering**
   - Ethnography involves observing users in their environment to understand their workflows. This is particularly useful in uncovering **latent requirements**—needs that users may not be aware of until they see the system in action.

---

#### **13. Practical Testing**
   - **Test Case Development**: For every requirement, a test case must be created that specifies what inputs will be provided and what outputs are expected.
   - Example of a **test case** for a login system:
     - Input: Valid username and password.
     - Expected Output: Successful login.

---

### Conclusion:
Requirements engineering is not just about documenting what the system should do but about ensuring every aspect of user interaction, system performance, and future adaptability is carefully captured, validated, and designed for. The iterative approach, ethnography, and proper validation techniques are essential in bridging the gap between users' needs and the final product.


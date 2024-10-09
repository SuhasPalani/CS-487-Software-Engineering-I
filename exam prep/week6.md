SE - Week 6 notes

Key Concepts: Dependability and Reliability
Dependability: Refers to the ability of a system to operate consistently, correctly, and predictably. It encompasses attributes like availability, reliability, safety, maintainability, and repairability.
Reliability: Focuses on a system’s ability to produce the correct output consistently. As discussed in the lecture, perfect reliability is a system that works 24/7 without fail or incorrect results. Reliability also touches on error tolerance, survivability, and maintainability​(Week 6_SE)​(CS 487 - Week 6 - Depen…).

Topics for Discussion (From PDF and Transcript)
1. Reliability as a Nonfunctional Requirement
In the lecture, the professor emphasized that reliability is part of the nonfunctional requirements for a system. It sits alongside performance, ease of use, scalability, portability, and maintainability​(Week 6_SE).
Perfect reliability means producing correct behavior at all times (365 days a year). However, the professor mentioned that perfect reliability is nearly impossible, and users must balance their expectations with feasible outcomes​(CS 487 - Week 6 - Depen…).
2. Dependability Attributes (From PDF)
The PDF outlines several attributes essential to creating dependable systems:
Repairability: The ability to quickly recover from failure, requiring diagnosis and repair​(CS 487 - Week 6 - Depen…).
Maintainability: Easily adaptable to new requirements​(CS 487 - Week 6 - Depen…).
Survivability: The system’s ability to withstand and recover from attacks​(CS 487 - Week 6 - Depen…).
Error Tolerance: Systems must tolerate user errors and, where possible, auto-correct them​(CS 487 - Week 6 - Depen…).
3. The Cost of Reliability
The professor raised the question: "How much is reliability worth?" He emphasized that risk assessment plays a key role in determining the cost-benefit of investing in reliability​(Week 6_SE)​(CS 487 - Week 6 - Depen…).
In terms of mitigation, it was mentioned that reducing risk and improving reliability involves assessing exposure (likelihood x impact) and determining how much investment is required to lower this risk​(Week 6_SE).
4. System Failures
The PDF outlines types of failures:
Hardware failures: These include design errors and component malfunctions.
Software failures: These arise from issues in requirements, design, or coding​(CS 487 - Week 6 - Depen…).
Operational failures: Often caused by user misuse or improper operations​(CS 487 - Week 6 - Depen…).
5. Safety-Critical Systems
Primary safety-critical systems directly control processes (e.g., embedded system controllers in cars). Failure here can lead to catastrophic results.
Secondary safety-critical systems don’t directly cause harm but can lead to dangerous situations (e.g., a failure in CAD software leading to design flaws in critical infrastructure)​(CS 487 - Week 6 - Depen…).

Important Key Points and Highlights from the Lecture Transcript
1. Connection to Systems & Protocols
The lecture introduced the idea of systems being connected via communication protocols, which must be engineered to be reliable. Whether this protocol is for human-computer interaction (HCI) or for systems, defining these protocols is crucial for reliable operation​(Week 6_SE).
The professor discussed how partner systems can affect your system's reliability. If a partner system (e.g., a backend repository) is unreliable, it will negatively impact the perception of your system’s reliability​(Week 6_SE).
2. Dependencies and Reliability
Systems are often dependent on external entities, such as back-end databases or human operators, to function correctly. If those dependencies are unreliable, the overall system will be perceived as unreliable​(Week 6_SE).
The professor stressed the importance of choosing reliable partners and avoiding the temptation to save money by using cheap, unreliable components or systems​(Week 6_SE).
3. Mitigating Unreliable Systems
In situations where 100% reliability is required (e.g., mission-critical systems), backups and contingency plans should be implemented. The professor used the example of a self-driving car, where reliability is critical because failure could lead to accidents​(Week 6_SE).
The professor emphasized the importance of exception handling, stating that systems need to be designed with mechanisms to handle potential errors without causing crashes​(Week 6_SE).
4. Context Model and Its Importance
A system's context model represents the system in the middle of its dependencies. The system communicates with various partners (e.g., repositories, sensors) and must manage these relationships to ensure reliability​(Week 6_SE).
Reliability is tied to these dependencies. If a partner system is unreliable (such as a faulty repository), then the entire system can fail or produce incorrect data​(Week 6_SE).
5. Risk Assessment and Exposure
The lecture repeatedly touched on the quantification of risk using exposure. This is done by multiplying the likelihood of failure by the impact it will have. This calculation is critical in risk mitigation, allowing engineers to determine how much investment is needed to lower the exposure​(Week 6_SE)​(CS 487 - Week 6 - Depen…).
The professor explained that reducing likelihood can significantly lower risk exposure, making it a cost-effective strategy to improve reliability​(Week 6_SE).

Conclusion
In preparing for your exam, focus on these critical themes:
Understand the interplay between dependability and reliability, especially as nonfunctional requirements.
Study the engineering aspects of creating reliable systems, including exception handling, communication protocols, and the use of reliable partners.
Grasp the methodology of risk assessment, and how engineers determine the cost-benefit of improving reliability.
Be prepared to discuss real-world applications of dependability and reliability, such as safety-critical systems and risk mitigation strategies in different engineering contexts​(Week 6_SE)​(CS 487 - Week 6 - Depen…).
This guide brings together the PDF's structured content with the professor's detailed lecture discussions, offering a comprehensive overview of Week 6's key topics.


















Here are detailed descriptions of key concepts from your SE exams, based on the lecture transcript and PDF content:
1. Sensing and Automation to Increase Awareness
Sensing in systems like autopilot in planes, self-driving cars, or temperature control sensors refers to the system's ability to detect and respond to environmental inputs. The professor emphasized how automation increases system awareness by continually sensing the environment and adjusting accordingly. This is critical in scenarios such as autonomous vehicles, where sensors provide constant feedback to ensure the car can navigate safely​(Week 6_SE).
Systems that can sense their environment, whether it’s temperature, motion, or user commands, often form the backbone of HCI and CCI systems (Human-Computer and Computer-Computer Interfaces)​(Week 6_SE).
2. Risk Exposure and Risk Management
The formula for risk exposure was a key topic:
Exposure (in dollars)=Likelihood (percentage)×Impact (dollars)\text{Exposure (in dollars)} = \text{Likelihood (percentage)} \times \text{Impact (dollars)}Exposure (in dollars)=Likelihood (percentage)×Impact (dollars).
This formula quantifies the future occurrence of risk and helps in calculating how much investment is needed to lower the exposure​(Week 6_SE)​(Week 6_SE).
The professor mentioned that risk management involves identifying threats and then mitigating them by reducing either likelihood or impact. By focusing on proactive approaches like improving requirements or adopting iterative development, risk exposure can be minimized​(Week 6_SE) .
3. User Acceptance Testing (UAT) and Risk of Failure
User acceptance testing (UAT) is a crucial part of risk management, where the risk of user rejection of the system is tested. If the system fails UAT, it could result in financial loss. The professor highlighted the importance of requirement clarity and iterations in reducing the likelihood of UAT rejection​(Week 6_SE)​(Week 6_SE).
Involving users during requirements gathering and testing helps improve system design, lowering the chances of failure​(Week 6_SE).
4. Human-Computer Interaction (HCI) and Computer-Computer Interaction (CCI)
HCI focuses on the means of communication between humans and computers, which can involve screens, touch interfaces, mouse clicks, or even voice commands. A well-designed system ensures that this interaction is intuitive and reliable​(Week 6_SE)​(Week 6_SE).
CCI, on the other hand, deals with interactions between systems. These protocols need to be well-defined to ensure smooth communication and avoid issues arising from poor interfacing​(Week 6_SE).
5. Exceptions Handling
Handling exceptions, such as failed ATM transactions or sensor malfunctions in a temperature control system, is critical for reliability. The professor explained how systems should be designed with built-in mechanisms to detect and handle exceptions gracefully. This prevents minor issues from causing system crashes​(Week 6_SE)​(Week 6_SE).
Exception handling should also account for the infinite possibilities of user interactions, where controls like dropdowns or predefined inputs limit errors and make the system more robust​(Week 6_SE).
6. Iterative and Rapid Prototyping
Iterative development and rapid prototyping were emphasized as methods to reduce the likelihood of system failure. By continuously iterating, testing, and involving the user, the system can be refined and its reliability improved. This contrasts with the waterfall model, where long development cycles without user feedback increase the risk of failures​(Week 6_SE) .
7. Temperature Control Sensor (HCI/CCI Scenario)
As an example of HCI and CCI, a temperature sensor that controls room temperature provides a real-world application. In this scenario, the sensor continuously monitors and adjusts the environment, illustrating the importance of sensing in automation. The professor discussed how off-the-shelf sensors often come with predefined protocols, which simplify the engineering process​(Week 6_SE).
8. Risk Mitigation and Exposure
The professor stressed the importance of risk mitigation, where the goal is to lower the exposure by addressing both likelihood and impact. For example, adopting backup systems (e.g., backup power or redundant servers) is a common strategy to reduce risk in case of failure​(Week 6_SE)​(Week 6_SE).
Prototyping and feedback loops were highlighted as key strategies for surfacing potential issues early in the development process​(Week 6_SE) .
These detailed descriptions should help in preparing for design and analysis questions in your exam. They also provide context for specific scenarios, such as autopilot, self-driving cars, and nuclear power plants, all of which rely heavily on sensing, automation, and risk management.






















Sample MCQs:
1.Which of the following best describes "risk exposure" in software engineering?
oA. The cost of fixing defects in a system.
oB. The likelihood of a system failure multiplied by the impact of the failure.
oC. The total time spent testing a system for defects.
oD. The ability of a system to handle user errors.
Answer: B. Risk exposure is the likelihood of failure multiplied by the impact of that failure​(Week 6_SE) .
2.What is the primary purpose of user acceptance testing (UAT) in software development?
oA. To test the reliability of the hardware components.
oB. To check the system’s interaction with other systems.
oC. To validate that the system meets user requirements and expectations.
oD. To perform stress tests on the system under maximum load conditions.
Answer: C. UAT ensures that the system meets user requirements and expectations​(Week 6_SE) .
3.Which of the following statements about iterative prototyping is true?
oA. It increases the likelihood of defects being missed.
oB. It reduces the risk of failure by enabling regular user feedback.
oC. It is typically used only for small systems.
oD. It avoids the need for risk assessments during development.
Answer: B. Iterative prototyping reduces the risk of failure by regularly incorporating user feedback into development .
4.In a Human-Computer Interaction (HCI) system, which factor is least likely to improve system reliability?
oA. Simplifying the interface to reduce user errors.
oB. Increasing the number of sensors for input data.
oC. Providing clear feedback to users about their actions.
oD. Implementing exception handling to manage input errors.
Answer: B. While increasing sensors may provide more data, it doesn't directly affect the reliability of the interaction. Simplifying interfaces, feedback, and handling exceptions improve user interaction reliability​(Week 6_SE) .
5.Which of the following scenarios is most likely to use a Computer-Computer Interface (CCI)?
oA. A self-driving car communicating with traffic lights.
oB. A user filling out a form on a website.
oC. A system displaying information on a monitor.
oD. A user interacting with an ATM.
Answer: A. CCI involves systems communicating with other systems, like a self-driving car interacting with traffic infrastructure​(Week 6_SE)​(Week 6_SE).

Sample Design-Based Scenario Question:
Scenario:
Consider a temperature control system used in a smart building. The system is responsible for adjusting the room temperature automatically using sensors and communicating with other devices (lights, fans, thermostats). It must maintain a comfortable temperature for occupants, while also ensuring energy efficiency. You are part of the development team tasked with improving the system’s reliability and HCI/CCI interactions.
Questions:
1.Remove the ambiguity of each of the following requirements: a. "The system must adjust the temperature automatically based on room occupancy."
b. "The system must ensure energy efficiency while maintaining occupant comfort."
c. "The system must interact with other devices in the smart building to optimize performance."
Answer: a. Ambiguity: "Automatically adjust" is unclear regarding the exact parameters.
oRefined Requirement: "The system must adjust the room temperature to between 68°F and 75°F when occupancy is detected for more than 10 continuous minutes."
b. Ambiguity: "Ensure energy efficiency" is vague and needs specific targets.
oRefined Requirement: "The system must reduce HVAC power usage by 20% during non-peak hours while keeping the room temperature between 68°F and 75°F."
c. Ambiguity: "Interact with other devices" does not specify the type or method of interaction.
oRefined Requirement: "The system must communicate with lights and fans via the ZigBee protocol to adjust power usage based on current temperature and occupancy levels."
2.Document test cases for each of the above requirements.
Answer:
oTest Case 1:
Requirement: Adjust temperature based on occupancy.
Test: Simulate occupancy by placing a motion sensor in a room. Measure the temperature change after 10 minutes.
Expected Result: The system adjusts the temperature to within the specified range (68°F to 75°F) after 10 minutes of detected occupancy.
oTest Case 2:
Requirement: Ensure energy efficiency during non-peak hours.
Test: Set the system to non-peak hours and measure HVAC power usage over a 24-hour period.
Expected Result: Power usage is reduced by 20% compared to peak hours while maintaining the room temperature.
oTest Case 3:
Requirement: Interaction with other devices.
Test: Turn on the system and monitor its communication with smart lights and fans.
Expected Result: The system successfully adjusts the brightness of lights and speed of fans based on temperature changes.
3.Propose an HCI/CCI “protocol” for the temperature control system to interact with users and other devices. Explain how it: a. Receives and comprehends user input for temperature preferences.
b. Handles exceptions such as sensor failures or incorrect input from other devices.
Answer: a. HCI Protocol:
oThe system uses a touchscreen interface allowing users to input their temperature preferences. It supports both voice commands (for accessibility) and manual input via buttons. The system processes these commands using natural language processing (NLP) to understand spoken requests, while also offering feedback on the screen for confirmation.
b. Exception Handling:
oIf the temperature sensor fails, the system activates backup sensors and sends a notification to the building's maintenance team. It also displays an error message on the user interface.
oIf an external device (like the thermostat or fan) sends incorrect data, the system performs a self-check, rejects the invalid data, and uses the last known correct input for continued operation. All exceptions are logged for later review.

# Messenger: Data Flow Diagram and Sequence DiagramAnalysis

CPS490 - Capstone I\
IA 04 - Messenger: Diagram Analysis\
Name: Ngoc Lan Anh Nguyen\
Student ID: 101835036

## 1. Data Flow Diagram Analysis (DFD)

**1.1 - Engineering question.** What is the data flow in the system? And where does it come from, where does it go?

**1.2 - Represented Requirements.**
FR-01 to FR-06 (registration, login, reset password from the User).
FR-07, FR-08 and FR-10, FR-11, FR-12, FR-13 (individual and group messages).
FR-08, FR-12, FR-13, and FR-14 (delivered messages with sender and timestamp, unread message when the user is offline).

**1.3 - Ambiguity Found and Meaningful Design Model.** 
- **Design Model:** The DFD clarifies how the system identifier between the message could be sent immediately to the receiver or stored in the data storage and how the system separated them using the `status` variable. And the system uses the process `P3. Check receiver’s status` to divide message based on its status. Instead of scanning all  data when a user wants to send a message, the system now only checks a specific receiver’s online status to modify the message’s status. Then, it could be divided into the corresponding data storage. 
- **Ambiguity**: Requirements don't state how a user logs out and how other users notice that. FR-08, FR-12, and FR-13 depend on "currently logged in", so logout (or session timeout) is a state change of the user that the system must track, however, there is no FR is describing it. And, if a user wants to send a message to the logged-out user, there is no mention of whether they know the other one is already logged out or not. 

## 2. Sequence Diagram Analysis 

**2.1 - Engineering question.** What is the communication between actors that the system performs? Who communicates with whom, in what order, and what happens if a user enters invalid input?

**2.2 - Represented Requirements.**
FR-01 to FR-06 (registration, login, reset password from the User).
FR-07, FR-08, FR-09 and FR-10 to FR-13 (individual and group messages).
FR-08, FR-12, FR-13, and FR-14 (delivered messages with sender and timestamp, unread message when the user is offline).

**2.3 - Ambiguity Found and Meaningful Design Model.** 
- **Design Model:** The sequence diagram indicates the workflow of the system from the beginning when users start registering for their account until how they use the system for communication purposes. From the diagram, we have a clear visualization of how the system will work and in which case, which actor will interact with the other. It also shows how the system handles unexpected cases caused during the utilization of the system. For example, when users start with account authentication, there are two cases that might happen. In the best case, they get the right information and can start texting with Messenger. In the worst case, when entering invalid information, the system sends a warning and asks security questions. 
- **Ambiguity**: The diagram does not mention how the user receives text messages from other users as individuals and a group member. Also, in phase 1, the system doesn’t indicate the process when the user answers a security question. 

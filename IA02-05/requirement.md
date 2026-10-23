# Messenger Application -  Requirements Engineering

​

CPS490 - Capstone I\

IA 03 - Messenger: Requirements Engineering\

Name: Ngoc Lan Anh Nguyen\

Student ID: 101835036

​

## 1. Project Information

Implement a Messenger application for social communication between people. This is similar to a network platform like Discord, where it provides a private and reliable environment that requires users to sign in and verify their accounts before they can access the chat environment and the chat history.

​

## 2. System Context

Messenger provides a secure, private communication platform designed for account registration, log-in options, direct text messaging between individuals and group text messages, and a database that stores chat history and unread messages. The functions that are not included in the project are voice or video calling, voice chat, and any built-in games. 

​

Based on the system, the main actors are the end users, who use the system in their daily lives for communication purposes. The client (the system owner) acts as a stakeholder who sets the requirements for the project and delivers it to the end users. 

​

## 3. Functional Requirements

| ID| Category|Functional requirements| 

|--------|-----------|------|

| FR–01 | Account creation and verification |The system allows users to create new accounts with username, password, and security questions. | 

| FR–02 | Account creation and verification|The system requires a username and password to satisfy the rule of 5-10 characters, including letters, digits, and underscores, no special symbols are allowed. The username has to be different from any username that is already registered.|

| FR–03 | Account creation and verification | The system has 2 options for users: either log in or create a new account.|

| FR–04 | Account creation and verification | If users cannot provide the correct username and password, Messenger interrupts their login process and asks for answers to the security questions.|

| FR–05 | Account creation and verification | If users can provide correct answers to security questions, they can enter a new password and start their sign-in process again. If not, the system redirects them back to the starting page.|

| FR–06 | Account creation and verification| If users enter the correct username and password, the system redirects them to their homepage. The system records the user’s information in data storage. |

| FR–07 | Individual messaging  | Users can send a text message to any other user using their username. |

| FR–08 | Individual messaging  | The messages will be delivered immediately to users if they are currently logged in. The system stored messages in data storage. |

| FR–09 | Text Format | The messages have to be 5-1000 characters, and not allowed an empty message. This applies to both individual and group messages. |

| FR–10 | Group messaging  | Users can create a group with 3-10 members and deliver messages to each other. The system records the group’s members in data storage.|

| FR–11 | Group messaging  | Group name can be modified. The system requires names from 5-30 characters and not allowed special symbols. The system records the group’s name in data storage.|

| FR–12 | Group messaging  | Text messages will immediately be sent to any group member who is currently signed in. |

| FR–13 | System  | If users are not signed in when messages are delivered, the system stores it and sends it when users log in, marked as unread. This applies to both individual texting and group texting.|

| FR–14 | System  |Any messages sent will show sender and timestamps. |

​


## 4. Non-functional Requirements

| ID| Category|Non-functional requirements| 

|--------|-----------|------|

| NFR–01 | Capacity |The system allows 15 users to log in at the same time without errors. | 

| NFR–02 | Capacity| Group messages can have a maximum of 10 members and they can send messages at the same time. The text will be delivered within 5 seconds to any member who is currently logged in.|

| NFR–03 | Account creation and verification | The server will check for username and password to match a registered account in the database within 10 seconds. |

| NFR–04 | Account creation and verification | If users cannot provide the correct username and password, Messenger displays a formatted warning. |

| NFR–05 | Account creation and verification| A Messenger only displays chat history to correctly registered users to protect privacy and reliability. |

| NFR–06 |Delivery | All source code and documentation will be committed and pushed to the course GitHub repository no later than November 2, 2026. |

​

## 5. Acceptance Criteria

| ID| Verification |Situation| 

|--------|-----------|------|

| AC–01 | FR-01, FR-02, FR-03| Given a new user name **Anna** wants to register for a new account. **Anna** at first entered invalid password, the system required her to enter it again following the formatted rules. She enters valid username and password follows the character rules, also the security questions. She completes her account creation and since that time, any new users want to name their account **Anna** will be announced that it is already registered.    | 

| AC–02 | FR-04, FR-05| After log out and come back, **Anna** forget her password. After entering the password incorrectly, the system displays an announcement asking for her security question's answer. If she answers it correctly, she can enter a new password. If not, she will be redirected to the starting page. |

| AC–03 | FR-06, FR-13| When **Anna** sign in, she receives 2 new messages that is marked as unread from **Luna** while she logs out. |

| AC–04 | FR-07, FR-08, FR-09, FR-14 | Given **Anna** sends an empty message, which is incorrect format. The system refused to deliver the message and asked her to enter a new one. After she entered new message followed the character rule, the system delivered it directly to **Luna**, **Luna** receives the message immediately with the sender's name and time on it. |

| AC–05 | FR-10, FR-11, FR-12| Given **Anna** creates a group for her class project. She then changed the group name to “Team 1”. She adds 3 more people, and they start discussing the project using the system. Then, **Luna**, a group member logged out, the team still can continue to discuss. When **Luna** signed back in, the system delivered the group’s messages to her with an unread mark. |

## 6. Assumptions and Unresolved Questions

### 6.1 Assumptions

- Users are identified using a unique username. No other information as phone number required.

- Messenger is a text-based communication tool. There is no voice chat or images included. 

- The number of users is fixed; the maximum is 15 users. 

- The password rule (5-10 characters, only includes letters, digits, and underscores) is simple, as the project is designed for a small group of users. 

- The maximum number of group members is 10. 

### 6.2 Unresolved Question

- What if users forget both password and security questions?

- Is the system sensitive to capital letters? 

- What if people keep entering the password incorrectly?group

- Can a member leave the group, be removed, modify the , or can only the creator of the group do it?

- Can a newly added member see the chat history before they join? 

- How long is the chat history stored? Can the user delete it? 

## 7. Traceability

| SOW Objectives| Requirements|Acceptance criteria|  Description|

|--------|-----------|------|---|

| Objective 3| FR-01, FR-02, FR-03 |  AC-01   | Make sure new users can sign in and have a unique username|

| Objective 4| FR-04, FR-05 |  AC-02   | Make sure users sign in to the correct accounts and protect the system's privacy. And, allow customers to reset their password if they forgot.|  

| Objective 1| FR-06, FR-13 |  AC-03   | Make sure users can receive messages even when they log out.| 

| Objective 1| FR-07, FR-08, FR-09, FR-14 |  AC-04   | Make sure users can send and receive messages between 2 individuals.|  

| Objective 2| FR-10, FR-11, FR-12, FR-13 |  AC-05| Make sure users can send and receive messages within a group chat.|  

​


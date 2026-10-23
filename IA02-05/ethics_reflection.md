# Messenger Application - Ethics Reflection
​
CPS490 - Capstone I\
IA 05 - Messenger: Ethics Reflection\
Name: Ngoc Lan Anh Nguyen\
Student ID: 101835036
​
## 1. Project Information
The Messenger application is designed for social communication between people. This is similar to a network platform like Discord, where it provides a private and reliable environment for users connected with other people individually or in a group with multiple people. The system requires users to authenticate themself by signing up an account or sign in to a registered account before they can send/ receive messages, which enhances the privacy and security for users.
​
## 2. Impact Analysis
​
### 2.1 Cultural
**Positive impact:** Messenger offers a convenient and user-friendly tool for people to connect and communicate with other people, regardless of culture or physical distance. Users can make friends with people coming from different cultures, enhance the culture integration and development. The group chat function can be served as a small communication including people from different cultures, where people can communicate and exchange any interesting information about their culture to people from different parts of the world.\
**Negative impact:** The system strictly limited the number of people per time, making the group chat can only support a fixed maximum number of people. It also doesn’t have the function to add/remove members, leading to a fixed number of members in the group, even if they stop online for a long period of time.  Messenger has strict rules of text formatting, while in text-based communication, emojis and characters are often used to express emotions and feelings.\
**Mitigation:** Implementation a group control function that allows users to add/remove members. Extension of the text formatting rules. And development of the number of people in a group.
​
### 2.2. Economic
**Positive impact:** Messenger offers a convenient and free of charge system, especially for students, small groups, etc. It also does not require a heavy computation hardware to run and implement it, making it affordable for anyone that is interested in, which is helping the base cost for small organizations and small businesses needs a communication tool between members and other people.\
**Negative impact:** By limiting the number of people currently signed in, the system cannot support many people, especially when it is in peak hours. It is not scaled for larger organizations, and the structure cannot handle any large group of people.\
**Mitigation:** For a testing time at the beginning, the system could remain the same. But in the future, developers could extend the number of people that the system could support, as well as the maximum number of members in a group.
​
### 2.3. Environmental
**Positive impact:** The system uses only text-based messages, which reduces the large media attachment compared to other video and image supported tools. It also reduces the storage demand, leading to a decline in the overall carbon footprint used during the utilization of Messenger.\
**Negative impact:** Because it doesn’t support video or image messages, users might find the system is strict and not interested enough to use it for a long period of time.\
**Mitigation:** This is an exchange and decision problem, if developers upgrade the system to support large file attachment, it consumes more energy and releases more CO2 footprint to the environment.
### 2.4. Global
**Positive impact:** The global impact has a small overlap with the cultural impact. Messenger supports communication and connection no matter the different language and far-distance location.\
**Negative impact:** The Messenger system raised an issue of balance between virtual communication and direct communication. Because of its convenience and affordability, people might rely on it and reduce in-person interaction.\
**Mitigation:** Users balance the utilization of the Messenger system.
### 2.5. Public health
Messenger has no significant impact on the public health aspect because the Messenger system is focused on the communication between people and people without physical impact on the user's health.  
### 2.6. Public safety
**Positive impact:** As we mentioned before, the Messenger system is a private and reliable tool for daily communication because it requires users to sign in with their registered account. By using strict account authentication, only users can access the account and have full privileges to read the chat history. This protects users’ privacy and their safety in general.\
**Negative impact:** The Messenger system only requires username and password to create an account, meaning if malicious people can sneak into the system and text to any users as soon as they know their username, then, they can transmit harmful content, harassment, etc. to the other users. And because it does not require much information for account verification, if the user’s information is leaked, malicious people can steal the account and use it for bad purposes such as stealing personal information, scamming other people, etc.\
**Mitigation:** Increase the required information to register for an account and keep updating if the people still keep the full control of their account regularly. Develop a safe tool to detect any bad words, harassment, etc., and either block or report the content to the main system; then, it can warn the users and limit the account with suspected action.
### 2.7. Public welfare
Messenger has no significant impact on public welfare as it is a communication tool between people and people, which is designed to help people get in touch with each other and enhances the connection between them, hence, it has no significant impact on public welfare.
​
### 2.8. Social
**Positive impact:** The social impact quite overlaps with culture and global impact as the Messenger system built for people connection. It helps users conveniently interact with their friends, family, etc. without paying a high cost or consuming much time to run the system.\
**Negative impact:** People send messages regardless of the content. Or some people intend to send harmful content to other people. People might rely on online communication and deny meeting in person or building a real-world relationship.\
**Mitigation:** Users have to balance between virtual communication and in-person communication.  
​
## 3. Connect Ethics to Engineering
### 3.1. Harassment, harmful, and untrue content in message delivery
The users who received that content are the main people affected in this case.\
**Potential harm:** People with bad attitudes and trying to harass other people might join in the group message and release harassment content to other people.\
**Mitigation:** To prevent this situation, developers can implement a content analysis tool to detect any bad word, phrases and block the messages, asking users to enter a new content instead.\
**Mitigation influences:** If developers implement a safety check, this will add a new requirement, function, acceptance criteria, and operational policy to the Messenger system. For example, when a user sends a message, the system will check if the format is valid first, then it will detect if the content “seems” to be safe or not before sending the message to the receiver. If the content includes any bad words, the system blocks it and asks users to enter a new one.\
**Requirement references:** For now, the system has no requirement related to content detection, the system only checks for the format and characters included in the message.
### 3.2. User’s information and privacy leaked
The users are the main people affected by this situation.\
**Potential harm:** Malicious people steal user’s information and sell it to a third party to make use of that. Based on the chat history, they can keep track of the user's accommodations, behaviors, etc.\
**Mitigation:** The developer can increase the password’s rules to have more symbols and digits to make it safer when there’s suspected action. After 3 times of incorrect password or username, the system asks a security question, if that is incorrect, the system blocks the account and sends a recovery link to the user's email or phone number. Double-layer locker by implementing one more password for chat history display.\
**Mitigation influences:** If we implement these mitigations, the requirements, data flow diagram, sequence diagram, etc. might have to be redesigned to match with this new condition.\
**Requirement references:** The system now has the security questions (FR-04) and redirects users if they enter incorrect answers for the security questions (FR-05).

## 4. AI Reflection
AI was used to assist with the PlantUML syntax and mainly for brainstorming ideas when I designed the overall workflow and wrote the ethics reflection. I also used it for vocabulary and checked for spelling and grammar. 
​



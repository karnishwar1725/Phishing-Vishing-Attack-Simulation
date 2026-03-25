🎣 Phishing & Vishing Attack Simulation

⸻

📌 Overview

This project demonstrates a practical simulation of social engineering attacks, focusing on:
	•	📧 Phishing (email-based attack)
	•	📞 Vishing (voice-based attack)

The simulations were conducted in a controlled lab environment using ethical practices and test accounts only.

👉 As described on page 3, the goal was to understand how attackers exploit human psychology rather than technical vulnerabilities  ￼

⸻

🎯 Objectives
	•	Simulate a real-world phishing campaign
	•	Analyze user behavior and response patterns
	•	Demonstrate credential harvesting techniques
	•	Understand psychological manipulation in vishing
	•	Evaluate effectiveness of social engineering attacks

⸻

🛠️ Tools & Technologies
	•	Kali Linux VM – Attack environment
	•	Social-Engineering Toolkit (SET) – Phishing simulation
	•	Custom Phishing Website – Credential harvesting
	•	Otter.ai – Call transcription
	•	Email test accounts – Controlled victims

⸻

📧 Task 1 – Phishing Simulation

⸻

⚙️ Environment Setup
	•	Attack hosted on Kali Linux VM (private IP only)
	•	No internet access (fully isolated lab)

👉 Page 4 shows blocked internet access (ping to 8.8.8.8 failed), confirming safe execution  ￼

⸻

🎯 Attack Design
	•	Theme: “Final Semester Results Released”
	•	Techniques used:
	•	Urgency (“expires in 30 minutes”)
	•	Authority (academic office email)
	•	Trust (realistic design)

👉 The email and fake login page (pages 5–6) mimic a real university portal to deceive users  ￼

⸻

⚡ Technical Implementation
	•	Mass Mailer Attack → sends phishing emails
	•	Credential Harvester → captures login data

Workflow:
	1.	Victim clicks phishing link
	2.	Redirected to fake login page
	3.	Credentials submitted via HTTP POST
	4.	Data captured in attacker terminal

👉 Page 7 shows captured credentials in real-time from the victim submission  ￼

⸻

📁 File Payload Simulation
	•	Fake PDF download included to simulate malware delivery
	•	Non-malicious (safe for testing)

👉 Page 8 shows the downloaded file on victim system  ￼

⸻

📊 Campaign Results

Metric	Value
Emails Sent	7
Link Clicks	6
Credentials Captured	4
File Downloads	3
Click Rate	~86%
Credential Rate	~57%

👉 Page 9 highlights how user trust decreases as risk increases (fewer downloads vs clicks)  ￼

⸻

📞 Task 2 – Vishing Simulation

⸻

🎯 Objective

Simulate a voice-based social engineering attack to extract:
	•	Student ID
	•	OTP
	•	Password

👉 Page 9 explains the shift from technical phishing to pure psychological manipulation  ￼

⸻

🎭 Attack Scenario
	•	Attacker impersonates university IT support
	•	Claims:
	•	Suspicious login attempts
	•	Risk of account suspension
	•	Creates urgency to force quick action

⸻

🧠 Psychological Techniques Used
	•	Authority → “IT security team”
	•	Urgency → “Account will be locked”
	•	Fear → “Multiple login attempts detected”
	•	Gradual escalation → from ID → OTP → password

👉 Page 13 shows how trust was built before requesting sensitive data  ￼

⸻

📞 Key Observation
	•	Victim initially trusted attacker
	•	Quickly shared ID and OTP
	•	Hesitated at password (security awareness)
	•	Eventually shared password after reassurance

👉 This highlights how manipulation overrides awareness under pressure  ￼

⸻

🧠 Key Learnings
	•	Humans are the weakest link in cybersecurity
	•	Social engineering relies on:
	•	Emotion
	•	Urgency
	•	Trust exploitation
	•	Even aware users can be manipulated

⸻

🛡️ Recommendations
	•	Enable Multi-Factor Authentication (MFA)
	•	Enforce strong password policies
	•	Implement phishing detection systems
	•	Conduct regular awareness training
	•	Simulate phishing/vishing drills

👉 Page 14 emphasizes combining technical + human-focused security  ￼

⸻

🚀 How to Reproduce
	1.	Set up Kali Linux VM
	2.	Launch Social Engineering Toolkit:

setoolkit

	3.	Configure:
	•	Mass mailer attack
	•	Credential harvester
	4.	Design phishing page
	5.	Send emails to test accounts
	6.	Analyze captured data

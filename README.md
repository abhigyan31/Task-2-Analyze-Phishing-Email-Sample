Phishing Email Analysis Report  
=================================

📄 Task: Analyze a Phishing Email Sample  
🖥️ Environment: Kali Linux in VMware  
🧰 Tools Used: Text viewer ('less'), manual inspection

-----------------------------------------------------
🔹 Step 1: Obtained a Phishing Email Sample
-----------------------------------------------------
- Downloaded a sample phishing email dataset ('fraudulent_emails.txt') from Kaggle.
- Extracted the '.txt' file in Kali Linux.

-----------------------------------------------------
🔹 Step 2: Examined Sender’s Email Address
-----------------------------------------------------
Sample:
From: "MR. JAMES NGOLA." <james_ngola2002@maktoob.com>

Phishing Indicators:
- Uses a free domain (`maktoob.com`)
- Pretends to be an official figure (Dr./Mr.) using a non-official email
- Reply-To and From fields are the same (self-referencing)

-----------------------------------------------------
🔹 Step 3: Checked Email Headers
-----------------------------------------------------
- Return-Path, From, and Reply-To all matched → suspicious consistency
- X-Mailer: Outlook Express 5.00 – outdated software used by scammers
- Unusual time zones and vague recipients

-----------------------------------------------------
🔹 Step 4: Identified Suspicious Links or Attachments
-----------------------------------------------------
- No clickable links or attachments found
- Social engineering email designed to trigger reply-based engagement

-----------------------------------------------------
🔹 Step 5: Looked for Urgent or Threatening Language
-----------------------------------------------------
Examples:
- Subject: "URGENT BUSINESS ASSISTANCE"
- Body: “Dear Friend”, “urgent attention”, inheritance offer
- Creates panic and emotional response

-----------------------------------------------------
🔹 Step 6: Checked for Mismatched URLs
-----------------------------------------------------
- No URLs present
- Strategy relies on direct contact (email reply)

-----------------------------------------------------
🔹 Step 7: Spelling and Grammar Errors
-----------------------------------------------------
Examples:
- “contect” instead of “contact”
- “there lives” instead of “their lives”
- Awkward phrasing and run-on sentences

-----------------------------------------------------
🔹 Step 8: Summary of Phishing Indicators
-----------------------------------------------------

| Indicator               | Observation                                                    |
|-------------------------|----------------------------------------------------------------|
| Suspicious Email Address| Free domains like 'lycos.com', 'mailcity.com', 'spinfinder.com'|
| Header Mismatches       | Same Return-Path and Reply-To fields                           |
| Urgent Language         | “Urgent Attention”, “Assistance Needed”, etc.                 |
| Grammar Errors          | Multiple typos and poorly written sentences                    |
| Emotional/Social Bait   | Dead relative, large inheritance                               |
| No Links/Attachments    | Reply-based social engineering scam                            |
| Generic Greeting        | “Dear Friend”, “Dear Sir”                                      |

✅ Conclusion:
The email contains clear phishing indicators and should be considered a scam.

-----------------------------------------------------

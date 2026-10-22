# Phishing Incident Report Checklist

To create a good report we need to answer the 5 Ws:
- What?
- When?
- Where?
- Who?
- Why?

## Time of Activity
`When?`

Specify when the suspicious activity occurred, including the exact date, time, and time zone if available in the logs.

*Example: The suspicious email was received on 21 October 2026 at 09:42 UTC.*

## List of Affected Entities
`Who or what was involved`

List the users, devices, accounts, or systems involved in or affected by the suspicious activity.  

Do not limit your investigation to the entities mentioned in the initial security alert.  
Review the relevant logs to identify other potentially affected entities and understand the full scope of the incident.  
For example if one employee received a phishing email, check the email logs to determine whether other employees received emails containing the same suspicious link.

*Example: User: j.smith; Device: WS-104; Email account: j.smith@company.com.*

## Reason for Classifying as True Positive 
`What evidence confirms the alert is real?`
`Why is this activity considered malicious?`

Explain which evidence confirms that the alert detected real suspicious or malicious activity rather than a false alarm.  
State the attacker's objective: what information or access they are trying to obtain from the victim through the phishing link (e.g., personal information, shipping details, or login credentials).

*Example 1: The email contained a suspicious link leading to a typosquatting domain.*  
*The email uses fear tactics by threatening to suspend the recipient’s Amazon account and creates urgency by demanding account verification within 24 hours.*

## Reason for Escalating the Alert
`Why is further investigation or action needed?`

Explain why the incident needs further investigation or action by another team, especially if the risk or impact is not fully resolved.  
State whether the firewall allowed or blocked the connection to the phishing URL and whether the recipient's workstation accessed the phishing page. If this cannot be confirmed from the available logs, explicitly state that the outcome is unknown and explain why further investigation or escalation is required.

*Example 1: The email contained a malicious link, and further investigation is needed to determine whether the user interacted with it.*  
*Example 2: The firewall blocked the connection before the page loaded. No evidence of further compromise was found in the available logs.*

## Recommended Remediation Actions
`What should be done next?`

Describe the actions that should be taken to contain the threat, remove it, or prevent similar incidents. Check whether suspicious URLs, IP addresses, or domains found in firewall logs are linked to emails or other events in the available logs. Identify the email, sender, and recipient associated with the URL to establish the full context of the attack.  
If the employee accessed a phishing URL and may have entered their password there write that the immediate password reset is required.

*Example: Block the malicious domain, remove the email from other inboxes, and check whether the user accessed the link.*

## List of Attack Indicators
`Where?` `Which specific details can help identify the attack?`

List the specific technical details that may help identify, investigate, or detect the attack, such as suspicious email addresses, email subject,URLs, IP addresses, file hashes, or domain names.  
Check the email content for fear tactics, urgent language, or pressure to take immediate action.

*Example: Sender: security@paypaI-support.com; URL: hxxps://paypaI-support.com/login; Fear tactic: threat of account suspension if the recipient does not act; Urgency: request to verify the account within 24 hours.*



### Vocabulary:
`Typosquatting` is a form of cybercrime that involves registering a domain name that maliciously mimics a popular web address, by exploiting users' typing errors (e.g., "gogle.com" instead of "google.com"), spelling mistakes, or visual variations.
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

*Example: User: j.smith; Device: WS-104; Email account: j.smith@company.com.*

## Reason for Classifying as True Positive - 
`What evidence confirms the alert is real?`
`Why is this activity considered malicious?`

Explain which evidence confirms that the alert detected real suspicious or malicious activity rather than a false alarm.

*Example: The email contained a suspicious link leading to a typosquatting domain.*

## Reason for Escalating the Alert
`Why is further investigation or action needed?`

Explain why the incident needs further investigation or action by another team, especially if the risk or impact is not fully resolved.

*Example: The email contained a malicious link, and further investigation is needed to determine whether the user interacted with it.*

## Recommended Remediation Actions
`What should be done next?`

Describe the actions that should be taken to contain the threat, remove it, or prevent similar incidents.

*Example: Block the malicious domain, remove the email from other inboxes, and check whether the user accessed the link.*

## List of Attack Indicators
`Where?` `Which specific details can help identify the attack?`

List the specific technical details that may help identify, investigate, or detect the attack, such as suspicious email addresses, URLs, IP addresses, file hashes, or domain names.

*Example: Sender: security@paypaI-support.com; URL: hxxps://paypaI-support.com/login*


### Vocabulary:
`Typosquatting` is a form of cybercrime that involves registering a domain name that maliciously mimics a popular web address, by exploiting users' typing errors (e.g., "gogle.com" instead of "google.com"), spelling mistakes, or visual variations.

### Introduction
`Welcome! This guide is here to help you navigate the process of investigating a security incident using the CrowdStrike Falcon platform. Whether you're new to this or just looking to brush up on your skills, you'll find clear steps to follow and tips to keep in mind.`

### What You'll Need

Before we jump in, make sure you have:

Access to the CrowdStrike Falcon platform.
A basic understanding of endpoint detection and response `(EDR)`.
Some knowledge of cybersecurity threats and indicators of compromise `(IOCs)`.
Getting Started with CrowdStrike

`Log In:`

Head over to the CrowdStrike Falcon login page.
Enter your credentials and complete the `multi-factor authentication (MFA)`.
Find Your Way to the `Host` Page:

Once you're in, go to the `Hosts` menu on the left.
Click on `Investigation` to see a list of hosts.
Locate the Host You're Investigating:

Use the search bar or filters to find the host you’re investigating. You can search by IP address, hostname, or user.
Spotting the Incident

`Look for Alerts:`

Navigate to the `Alerts` section under `Hosts.`
Keep an eye out for any alerts related to your host, especially those marked as high severity.

`Dive into the Alert Details:`

Click on any alert to get more details. You’ll see the `alert type`, `severity`, and a `description` of what’s going on.
Take note of when the alert happened and which processes were involved.

### Digging Deeper
`Process Analysis`

`Check Out the Process Tree:`

Review the process tree to get a sense of how things unfolded.
Pay attention to the parent and child processes to figure out where the suspicious activity started.

`Look at Command-Line Arguments:`

Command-line arguments can give you clues about what the process is doing. Watch out for anything unusual.

### Network Activity

`Review Network Connections:`

Look at the network connections the host made. Are there any unexpected or unauthorized connections?

`Check IP Geolocation and Reputation:`

Use threat intelligence tools to see where these IPs are located and whether they have a bad reputation.

### File and Registry Analysis

`Examine File Modifications:`

Check out the files that were created or changed during the incident. Compare file hashes with known malware signatures.

`Investigate Registry Changes:`

Look for any registry changes, especially ones that could indicate persistence mechanisms.

### Taking Action

`Isolate the Host:`

If you haven’t already, isolate the host from the network to stop any further damage.

`Terminate Malicious Processes:`

End any processes that you’ve identified as malicious.

`Remove Persistence Mechanisms:`

Get rid of any registry keys, startup items, or scheduled tasks that might allow the attacker to come back.

`Patch Vulnerabilities:`

Apply any patches for vulnerabilities that were exploited during the incident.

`Consider Reimaging:`

If the host is too compromised, reimaging might be the best option to ensure it’s clean.

### Wrapping Up

`Document Everything:`

Write down what you found, the actions you took, and any conclusions you’ve drawn. A detailed report is essential.

`Share Your Findings:`

Make sure to share your report with the relevant teams—whether that’s IT, legal, or management.

`Post-Incident Review:`

After everything is settled, take some time to review the incident with your team. What went well? What could be improved?

### Final Thoughts

Investigating incidents with CrowdStrike Falcon can be complex, but with a systematic approach, you can effectively identify, analyze, and remediate threats. This guide is just the beginning—real-world experience will deepen your understanding and sharpen your skills.

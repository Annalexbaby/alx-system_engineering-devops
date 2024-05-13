Disruption of services
There was a disruption in services due to a spike in traffic on a website developed by a team of software developers, which I am a member.

•	The outage occurred from 8:00 AM to 2:00 PM on the 7th of January, 2024 (WAT).
•	Impact: The outage had an effect on the authentication service, causing users to experience login failures and inability to access secured resources. An approximate of 50% of users were unable to log in during the outage.
•	Root Cause: The root cause of the issue was discovered to be due to a misconfiguration in the authentication service's database connection pool settings.
Timeline:
•	8:00 AM: The issue was detected when users started reporting login failures.
•	8:05 AM: Software engineers received monitoring alerts indicating a spike in failed authentication requests during login.
•	8:10 AM: Initial investigation focused on network connectivity.
•	8:30 AM: The presence of bugs was also assumed to be a causative agent.
•	8:45 AM: It was discovered by the backend software developers that bugs was not the root cause of the malfunction.
•	9:00 AM:  The team identified the misconfiguration in the database connection pool settings as the root cause.
•	10:30 AM: The misconfiguration was corrected, and the authentication service was restarted.
•	12:00 PM: Verification tests conducted to ensure the issue was resolved.
•	2:00 PM: Services fully restored, and monitoring confirmed no further anomalies.
Corrective and Preventive Measures:
The misconfiguration in the database connection pool settings caused the authentication service to exhaust available connections, leading to login failures. The misconfiguration was corrected by adjusting the database connection pool settings to ensure an adequate number of connections were available. Additionally, monitoring was enhanced to provide early detection of similar issues in the future


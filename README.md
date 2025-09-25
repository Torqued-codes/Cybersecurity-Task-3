PC Vulnerability Scan Report :

i] Objective :
Perform a basic vulnerability scan on your PC using Nessus Essentials and document the findings to demonstrate understanding of common security risks and remediation steps.

ii] Tools Used :
Nessus Essentials 

iii] Scan Configuration :

Scan Type: Basic Network Scan

Target: IPaddress

iv] Summary of Results :

Severity	Vulnerability Name	Family	Count
Medium	SMB Signing not required	Misc.	1
Mixed	SSL (Multiple Issues)	General	4
Info	SMB (Multiple Issues)	Windows	6
Info	HTTP (Multiple Issues)	Web Servers	2
Info	Microsoft Windows (Multiple)	Windows	2
Info	TLS (Multiple Issues)	Service Detection	2
Info	Netstat Portscanner (SSH)	Port Scanners	25

v] Key Findings :

1. Medium Severity Vulnerability - SMB Signing not required

- Description: SMB signing is not enforced by default, which can allow man-in-the-middle attacks on file sharing connections.

- Impact: Attackers could intercept or modify SMB traffic on a local network.

- Remediation:

- Enable SMB signing using Group Policy Editor:

Go to gpedit.msc > Computer Configuration > Windows Settings > Security Settings > Local Policies > Security Options

Set “Microsoft network client: Digitally sign communications” to “Enabled”

2. Other Vulnerabilities -
Multiple issues reported for protocols/services (SSL, SMB, HTTP, TLS)

Informational findings include port scans, host enumeration, and various service detections

- No critical vulnerabilities found; majority are informational or low risk

- Recommendations :
Apply the SMB signing fix as described above.

Monitor and regularly update PC/network software to keep up with new vulnerabilities.

Future scans recommended to ensure ongoing security.

vi] Evidence :
Screenshots of scan summary and vulnerabilities are placed in the repo
Vulneribility table

Scan dashboard

Vulnerability table

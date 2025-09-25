PC Vulnerability Scan Report :

i] Objective :
Perform a basic vulnerability scan on your PC using Nessus Essentials and document the findings to demonstrate understanding of common security risks and remediation steps.

ii] Tools Used :
Nessus Essentials 

iii] Scan Configuration :

Scan Type : Basic Network Scan

Target : IP address

iv] Screenshots :

## Screenshots

![Vulnerability Scan Result 1](Vulnerability%20pic%201.png)
![Vulnerability Scan Result 2](Vulnerability%20pic%202.png)


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

- Screenshots of scan summary and vulnerabilities are placed in the repo.
- Vulneribility table.

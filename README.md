# External-SSL-Audit
Script that will utilize the output from SSL Labs API json and parse the data into a spreadsheet for easy viewing and reporting.  Requires SSL Labs Scanner that can be found here:  https://github.com/ssllabs/ssllabs-scan

You can find an overview of using this here:  https://sec.mn/Archive/2016/April-Assessing_External_SSL.pdf

Usage:
Capture Json data using ssllabs-scan:
ssllabs-scan --quiet --hostfile=mydomain.txt --ignore-mismatch=true --hostcheck=false > mydomain.json

Parse Json Data:
cat mydomain.json | ./ssllabparser_toxslxv2.py

Currently Captures in Spreadsheet:

Currently Captures in the spreadsheet:

•	Site Name
•	Port
•	IP
•	SSL Labs Grade
•	Certificate Issuer
•	Certificate Expiration
•	Certificate MD5 Hash
•	Certificate Size
•	Certificate Algorithm
•	Certificate Strength
•	HeartBleed
•	HeartBeat
•	CCS
•	Poodle
•	Fallback SCSV
•	Freak
•	Logjam
•	Supports RC4
•	BEAST
•	Insecure Renegotiation
•	Server Signatures
•	SSL v2
•	SSL v3
•	TLS 1.0
•	TLS 1.1
•	TLS 1.2
•	HSTS Present
•	HSTS Max Age
•	HSTS Subdomains
•	HSTS PreEnabled

*Contains a second worksheet with automatically generated tables for producing graphs.

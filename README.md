# External-SSL-Audit
Script that will utilize the output from SSL Labs API json and parse the data into a spreadsheet for easy viewing and reporting.  Requires SSL Labs Scanner that can be found here:  https://github.com/ssllabs/ssllabs-scan

Usage:
Capture Json data using ssllabs-scan:
ssllabs-scan --quiet --hostfile=mydomain.txt --ignore-mismatch=true --hostcheck=false > mydomain.json

Parse Json Data:
cat mydomain.json | ./ssllabparser_toxslxv2.py


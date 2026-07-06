[[tlsssl]], [[ssltls]]

Missing - when bank has no cert there should be message not table shown
Scenario
1. Add
2. Pick Citi
3. Pick Decyrpt cert 
4. Pick Uat
5. DSIGUATCITI01TEST name
6. key size 2048
7. dsig.citi01.com common name
8. download
9. change to proper leaf
10. upload
11. check


Things to fix
1. Validation still in small letters
2. No message when there is no certificate

Automated tests: 
1. When bank api is choose andthere is no cert should be visible info
2. When bank api is choosen and data is selected, data should be retained
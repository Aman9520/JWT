# JWT

https://infosecwriteups.com/account-takeover-by-tampering-the-signup-verification-token-9abadc5e4dbf

#weak signing key
Steps:
1: Use hashcat :  hashcat -a 0 -m 16500 <YOUR-JWT> /file/jwtsecrets 
2: After getting secret 
3: encode the secret in base64
4: then go to JWT Editor and click new symmetric key , Click on generate and then paste the base64 encode secret in "k" parameter (    "k": "q1WW05S4iIVpMFsCRdzibQ==") and then click OK.
5: Now go to repeater click on Json web token click on "sign" and update it .

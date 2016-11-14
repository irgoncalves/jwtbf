#jwtbf.py - simple script to brute force JWT token signature using a wordlist

  For JWT info, refer to https://jwt.io/introduction/

#Requirements
  This script requires PyJWT Package 
  Refer to this link for proper documentation/installation https://pypi.python.org/pypi/PyJWT

#Usage

For usage, supplies when asked JWT token then the target wordlist

user@host:~/jwtbf# python jwtbf.py
Enter JWT token:eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiYWRtaW4iOnRydWV9.TJVA95OrM7E2cBab30RMHrHDcEfxjoYZgeFONFh7HgQ
Enter wordlist name:wordlist.txt
Failed to verify token signature with the following key: test
Failed to verify token signature with the following key: test2
Success. Token decoded with the following key:secret
{u'admin': True, u'sub': u'1234567890', u'name': u'John Doe'}



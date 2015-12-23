this is rubyonci repo for testing ci again ruby

---
Problem:

$ git push origin cibuild:cimain

Warning: Permanently added the RSA host key for IP address '192.30.252.130' to the list of known hosts.

ERROR: The key you are authenticating with has been marked as read only.
fatal: Could not read from remote repository.

Please make sure you have the correct access rights

git push origin cibuild:cimain returned exit code 128

and the repository exists. Action failed: git push origin cibuild:cimain
---
Troubleshoot:

1. On CircleCI project > Project Settings > Checkout SSH keys

2. Add key, and then be forwarded to GitHub web site for authorizing

3. Add key

4. Rebuild job

---



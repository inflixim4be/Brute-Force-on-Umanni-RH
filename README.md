# CVE-2020--
Brute Force on Umanni RH

==

# Description

Umanni RH does not limit the number of authentication attempts. An unauthenticated user may exploit this vulnerability to launch a brute-force authentication attack against the Login page.

==

# Exploitation

To exploit this vulnerability, it is necessary using the user enumeration vulnerability in Password Recovery to enumerate the valid users and after could perform an arbitrary number of authentication attempts using different passwords, and eventually gain access to the targeted account.

==

# PoC

== Login Page ==

![16_](https://user-images.githubusercontent.com/49153346/87191478-dc188c00-c2ca-11ea-8ce9-b29de08995e1.JPG)

== Brute Force Login - Invalid Password ==

![12_](https://user-images.githubusercontent.com/49153346/87191226-601e4400-c2ca-11ea-9aa6-6e9199191535.jpg)

== Brute Force Login - Valid Password (Redirect) ==

![13__](https://user-images.githubusercontent.com/49153346/87191671-43ced700-c2cb-11ea-8fc8-5225f2648eee.jpg)

== Brute Force Login - Valid Password (Redirect) ==

![14__](https://user-images.githubusercontent.com/49153346/87191234-63b1cb00-c2ca-11ea-8f1d-64c2a5ea1240.jpg)

== Brute Force Login - Valid Password ==

![15_](https://user-images.githubusercontent.com/49153346/87191238-64e2f800-c2ca-11ea-888c-f3966f85a4d2.jpg)

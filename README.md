<h2 align="center">
  CVE-2020-24007 
  <br/>
  Brute Force on Umanni RH
</h2>

<p align="center">
  <img src="https://user-images.githubusercontent.com/49153346/88341987-f021ac00-cd14-11ea-836b-0fba611d7540.png" width="350" />
</p>

<hr>

### Description

Umanni RH does not limit the number of authentication attempts. An unauthenticated user may exploit this vulnerability to launch a brute-force authentication attack against the Login page.


### Exploitation

To exploit this vulnerability, it is necessary using the user enumeration vulnerability in Password Recovery to enumerate the valid users and after could perform an arbitrary number of authentication attempts using different passwords, and eventually gain access to the targeted account.


### PoC

* Login Page

<img src="https://user-images.githubusercontent.com/49153346/87191478-dc188c00-c2ca-11ea-8ce9-b29de08995e1.JPG"/>

<br />

* Brute Force Login - Invalid Password 

<img src="https://user-images.githubusercontent.com/49153346/87191226-601e4400-c2ca-11ea-9aa6-6e9199191535.jpg"/>

<br />

* Brute Force Login - Valid Password (Redirect) 

<img src="https://user-images.githubusercontent.com/49153346/87191671-43ced700-c2cb-11ea-8fc8-5225f2648eee.jpg"/>

<br />

* Brute Force Login - Valid Password (Redirect) 

<img src="https://user-images.githubusercontent.com/49153346/87191234-63b1cb00-c2ca-11ea-8f1d-64c2a5ea1240.jpg"/>

<br />

* Brute Force Login - Valid Password 

<img src="https://user-images.githubusercontent.com/49153346/87191238-64e2f800-c2ca-11ea-888c-f3966f85a4d2.jpg"/>

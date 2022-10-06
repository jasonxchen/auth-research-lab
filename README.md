# ![GA Logo](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Auth Research Lab

---

Authentication is a complex and exciting topic that involves using many of the concepts we've already studied as well as several new ideas. 

An authentication system allows the registration / signup of new users and allows those users to sign in. It has to be able to identify each user and keep their information private and secure.

Being able to develop secure user login systems is in fact a whole career and life path in and of itself, but understanding the broad concepts of **Auth** is critically import for all developers. 

Describing auth flow and understanding key terms are very common **interview questions** for junior developers, so lets take some time to research and understand auth and the related concepts.

## Setup

Fork and clone this repository and answer the questions as you research directly in the README. You do not have to pull request and submit this lab, but you will want to have it on hand for reference in the future. 

## Auth Concepts Worksheet

#### Define the following

1. *Authentication*
    * A: Process to verify the identity of the user
        * Ask for credentials and check against known credentials
2. *Authorization*
    * A: Process of granting or denying user access to resources once authenticated
3. Explain how *authentication* and *authorization* are related but distinct concepts.
    * A: Authorization to resources comes after authenticating who the user is, so one is typically linked with the other but are separate actions
5. *Sessions vs Token based auth*
    * A: Session-based auth requires that the server stores information (in the database) about the user once authenticated, while token-based auth makes the client store it and the server checks the token on each request
        * Token-based auth more popular now b/c of efficiency
6. *json web token (also know as a jwt)*
    * A: Secure json data that asserts claims such as what the user with the token is allowed to do
        * optionally signed or encrypted via a secret or key
        * small size in parts (header, payload, signature)
7. *Encoding, encryption and hashing* along with the uses for and differences between the three
    * A: 
        * Encoding: converting characters into specialized format specifically for better transmission or storage
            * Can be decoded publicly
        * Encryption: securely converting information into secret code specifically to hide the information's meaning
            * Can be decrypted privately
        * Hashing: converting characters into another value of (usuallly) shorter, fixed length
            * Cannot be reversed
8. *oAuth* (pronounced oh-Auth)
    * A: Stands for open authorization. Allows giving authorization tokens without sharing passwords (provided you are already authenticated)

#### Explore and then describe the following npm packages:

1. [bcrypt](https://www.npmjs.com/package/bcrypt)
    * A: Industry standard Node package to hash passwords or any other important information
2. [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)
    * A: Implements json web tokens to be used for user authorization
3. [passport](https://www.npmjs.com/package/passport)
    * A: An API-based authentication middleware for helping approve or fail an authentication request
    * also describe what a *strategy* is in the context of this npm package
        * A: Strategies are the processes to define the logic of the authentication. There are already hundreds of pre-defined strategies on the passportJS site

---

## Licensing
1. All content is licensed under a CC-BY-NC-SA 4.0 license.
2. All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.
# Read 9a: OAuth

[README](/README.md)

1. Why is authentication important? [resource](https://searchsecurity.techtarget.com/definition/authentication#:~:text=Authentication%20is%20important%20because%20it,network%2Dbased%20applications%20or%20services.)

- Authentication is important because it acts a lock for any processes that a company wants to keep protected. Having routes and the like protected ensures that un-authorize people cannot.
- Locks down networks, databases, websites and other network-based applications or services.

2. Why should we be careful about storing a user’s password?

- because if done incorrectly, that password could be decrypted and allow bad people to do what they want with that information. Plain text storage is a horrible idea and you should never do it

3. What is the difference between hashing and encryption? [GCN.com](https://gcn.com/articles/2013/12/02/hashing-vs-encryption.aspx#:~:text=Encryption%20is%20a%20two%2Dway,to%20reveal%20the%20original%20password.)

- Hashing is a one-way function that scrabbles plain text to make something that is safe and digestible by programs and is unable to be reversed
- Encryption is a two way function and can be decrypted with the correct key ( which is kept secret )

4. What is the difference between encryption and encoding?

- Encoding keeps the data easy to use, but it can be decoded using the same algorithm that encoded it in the first place
- Encryption is meant to keep the data Confidential and can only be accessed using a key.

5. What is a token used for?

- A token is used for authentication and offers a more secure verification process. It is very secure when used along side other verification technologies

authentication

- process of verifying who a user is
  authorization
- verifying what the user has access to

encryption

- Encryption is a two way function and can be decrypted with the correct key ( which is kept secret )

hashing

- a one-way function that scrabbles plain text to make something that is safe and digestible by programs and is unable to be reversed

## session

## cookie

token

- often contains a header, payload, and a signature
  - header has the payload type and the signing algorithm
  - payload has the data that pertains to the user
  - signature s used to make sure the message has not been jeopardized

## Basic Auth

## encoding

secret

-

cryptography

#### oAuth

- Originally built for authorization between services

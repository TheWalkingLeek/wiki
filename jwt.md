# JWT - JSON Web Token

JWTs consist of three parts separated by dots(`.`)

- Header
- Payload
- Signature

--> `xxxxx.yyyyy.zzzzz`

## Header

Consists typically of the type of token (which is JWT) and the signing algorithm thats being used

`{ "alg": "HS256", "typ": "JWT" }`

The header then is being encoded using Base64Url

## Payload

The paload consists of claims. Claims are statements about an entity (typically, the user) and additional data.

There are three types of claims: registered, public, and private claims.

`{ "sub": "1234567890", "name": "John Doe", "admin": true }`

The payload then also gets encoded using Base64Url

## Signature

The signature is being created using the encoded header, the encoded payload, a secret,
the algorithm specified in the header, and sign that

For example if you want to use the HMAC SHA256 algorithm, the signature will be created in the following way:

`HMACSHA256( base64UrlEncode(header) + "." + base64UrlEncode(payload), secret)`

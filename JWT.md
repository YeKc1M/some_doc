# JWT

header, payload, signature

## header

type of token ("JWT"), algorithm

```json
{
    "typ": "JWT",
    "alg": "HS256"
}
```

## payload

contains claims

* [registered](https://tools.ietf.org/html/rfc7519#section-4.1)
  * iss (issuer), optional
  * sub (subject)
  * aud (audience)
  * exp: expiration time
  * nbf: not before
  * iat: the time when the JWT is issued
  * jti: JWT ID
* public
* private

```json
{
    "sub": "123456",
    "name": "name",
    "admin": true
}
```

## signature

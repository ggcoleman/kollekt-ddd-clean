# Kollekt API

- [Kollekt API](#kollekt-api)
    - [Authentication](#auth)
        - [Register](#registration)
            - [Register Request](#register-request)
            - [Register Response](#register-response)
        - [Login](#login)
            - [Login Request](#login-request)
            - [Login Response](#login-response)

## Auth

### Register

```js
POST {{host}}/auth/register
```
#### Register Request

```json
{
    "firstName": "Guy",
    "lastName": "Coleman",
    "email": "coleman.guyg@gmail.com",
    "password": "aRe@11y5af3p@55w0rd"
}
```

#### Register Response

```js
200 OK
```
```json
{
    "id": "0e3e5776-1910-4965-9ac6-0da5414fa698",
    "firstName": "Guy",
    "lastName": "Coleman",
    "email": "coleman.guyg@gmail.com",
    "token": "eyJhbGciOiJB...MYCbCiWOgg"
}
```
### Login
```js
POST {{host}}/auth/login
```
#### Login Request
```json
{
    "email": "coleman.guyg@gmail.com",
    "password": "aRe@11y5af3p@55w0rd"
}
```
#### Login Response
```js
200 OK
```
```json
{
    "id": "0e3e5776-1910-4965-9ac6-0da5414fa698",
    "firstName": "Guy",
    "lastName": "Coleman",
    "email": "coleman.guyg@gmail.com",
    "token": "eyJhbGciOiJB...MYCbCiWOgg"
}
```
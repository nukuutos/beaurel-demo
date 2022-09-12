# Beaurel Demo

<img src="./beaurel.png" alt="beaurel" align="right" />

Beaurel is a platform for beauty masters and their customers. For beauty masters, it allows creating a flexible timetable and services, showing customers their work. Customers can book appointments and review masters. Beaurel has some social network elements like messenger, favorite masters (friends), etc.

## Start up

You can run this local version of Beaurel by **docker**

```console
$ docker compose up
```

## Usage

You can't sign up on this demo. You can use fake accounts.

Fake master account:

```json
"username": "master",
"password": "123456"
```

Fake customer account:

```json
"username": "customer",
"password": "123456"
```

If you want to search masters as guest you should set city to `Владивосток`

## Database

This demo uses **Atlas** version of Mongodb. Once a day I restore database and clean up yandex s3 bucket.

## Links

- [Client](https://github.com/nukuutos/beaurel-client)
- [API](https://github.com/nukuutos/beaurel-api)

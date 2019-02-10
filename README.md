# README

## Tools

| Tool  | Purpose |
| :---: |:-------:|
| [Postman](https://www.getpostman.com/) | Requests in the api |


## Gems

| Gems  | Purpose |
| :---: |:-------:|
| [Faker](https://github.com/stympy/faker) | A library for generating fake data such as names, addresses, and phone numbers. |
|  |  |
| General | Version |
| Ruby  | 2.5.1 |
| Rails | 5.2.2 |


## Getting started

Clone the repository
```
git clone https://github.com/RuanAyram/yi_mobile_challenge
```

#### Edit `config/database.yml`, if necessary

Enter in the folder, then run these commands to install gems, create a database and populate, then run api locally
```
cd myarticles

bundle install

rails db:create && rails db:migrate && rails db:seed

rails s
```

## My API Endpoints

### Events

| Method + url | Output |
| :----------- |:-------|
| GET http://localhost:3000/api/v1/articles | Returns a list of all articles in the database |
| POST http://localhost:3000/api/v1/articles | Body JSON format (required) |
| PUT http://localhost:3000/api/v1/articles/1 | Body JSON format (required) |
| DELETE http://localhost:3000/api/v1/articles/1 | Delete id 1 |
 ```javascript
{
    "id": 1,
    "title": "Death Be Not Proud",
    "body": "Non facilis ea natus.",
    "created_at": "2019-02-10T21:40:00.194Z",
    "updated_at": "2019-02-10T21:40:00.194Z"
}
 ```
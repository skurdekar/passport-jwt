# Passport authentication library usage with Local Strategy

### Install MogoDB (either locally or using Docker container)

### install nodemon

### Run
```nodemon start```

### Test
test the following routes with Postman

#### Post /signup
Pass in email (a@b.com) password (password)
{
    "message": "Signup successful",
    "user": {
        "_id": "5c42abe0df60bc304c075fb6",
        "email": "a@b.com",
        "password": "$2b$10$mBY3yGca37AWyzQPMkTbNeCOLCXTYMk7dybfXILIhlvXkFWu9p/xK",
        "__v": 0
    }
}

#### Post /login
Pass in email (a@b.com) password (password)

{
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyIjp7Il9pZCI6IjVjNDJhYmUwZGY2MGJjMzA0YzA3NWZiNiIsImVtYWlsIjoiYUBiLmNvbSJ9LCJpYXQiOjE1NDc4NzMzMTJ9.OqNHRvDmo_ORb8VrCcGjPGMp7b6rzvhQL4ZIz3_AcaY"
}

#### Get /user/profile?secret_token=....
{
    "message": "You made it to the secure route",
    "user": {
        "_id": "5c42a6cc4824a02fd188b0a7",
        "email": "s@k.com"
    },
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyIjp7Il9pZCI6IjVjNDJhYmUwZGY2MGJjMzA0YzA3NWZiNiIsImVtYWlsIjoiYUBiLmNvbSJ9LCJpYXQiOjE1NDc4NzMzMTJ9.OqNHRvDmo_ORb8VrCcGjPGMp7b6rzvhQL4ZIz3_AcaY"
}


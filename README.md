# Fb-Api 
##### How to use it ? 
    $ npm install
Then you have to run mongod in another terminal

    $ mongod

Then start the app

    $npm run start
    
You should also use ```postman``` for the request
# User api 
Crud API for all users
#### [POST] Create user 
Allows the creation of a single user.
|User|Api|
|---|---|
|Require autenthification |No|
|Who can use it |Everybody|
|Response formats |Application/JSON|

- HTTP request : POST → user/create
#### Parameters
```javascript
{
    'first_name': 'Rativeau', // optionnal
    'last_name': 'Corentin', // optionnal
    'email': 'Rativeau@gmail.com', // required
    'password': '123456789', // required
    'age': 23, // optionnal
    'gender': 'm', // optionnal,
    'height': 1.86, // optionnal
    'weight': 70, // optionnal
    'city': 'Paris', // optionnal
    'city_code': '75000', // optionnal
    'street_number': 20, // optionnal
    'street_type': 'rue', // optionnal
    'street_name': 'montsoult', // optionnal
    'phone': '065114582', // optionnal
    'image_profil': 'https://www.mediacritik.com/wp-content/uploads/2019/04/rs_1024x759-170407142939-1024.Peter-Dinklage-Game-of-Thrones.kg_.040717.jpg' // optionnal
}
```

#### Response
``` javascript
{
  'id': '12483hdhd2838',
  'first_name': 'Corentin',
  'last_name': 'Rativeau',
  'email': 'Rativeau@gmail.com',
  'password': '123456789',
  'token': 'Y9Y1lusRUNVfKnv75yFUXw4wpo1OwK0HYd0RSVEkaaNCvz6oLNTT49m2Mix9sFHLwxeYWPUsgXxdhQYS80MgEE9Sljuq9VctHvdm'
  'age': 23,
  'gender': 'm',
  'height': 1.75,
  'weight': 80,
  'city': 'Paris',
  'cityCode': '75000',
  'street_number': 13,
  'street_type': 'rue',
  'street_name': 'de cambrai',
  'phone': '0651448017',
  'image_profil': 'https://www.mediacritik.com/wp-content/uploads/2019/04/rs_1024x759-170407142939-1024.Peter-Dinklage-Game-of-Thrones.kg_.040717.jpg'
}
```





# Dog Dial
Better dog tags with personalized phone numbers.

## New User Flow
New users register with email and then verify phone number.

Each user can have multiple pets (dogs) each has it's own phone number.

Each pet can have a personalized greeting with medical information, demeanor, and whatever else

![New User](https://github.com/dtolb/dogdial/blob/master/readme-images/Dog-Dial-new-user.png?raw=true)

## Call Flow
![Call Flow](https://github.com/dtolb/dogdial/blob/master/readme-images/Call-flow.png?raw=true)

## User Model
Each User has:
* 0+ pets
* 1+ validated phone numbers
* email address
* user name

## Pet Model
Each pet has:
* Phone number
* Name
* Comments
* Personalized greeting
* Medical Issues

## API
### /users
* ```POST``` - create new user
* ```GET``` {username} - get user

### /users/{username}/pets
* ```POST``` - create new pet
* ```GET``` - get all pets
* ```GET``` /pets/{petid} - get a pet


* Date: 2016-07-26
* Creator: shuchengc

##Descritpion:
----
This is a movie reviews restful api by using node.js,express and mongodb.
all the APIs are tested by postman.

###Functionality:

- get all reviews: GET /api/reviews
- get one reviews: GET /api/reviews/id
- create a new review: POST /api/reviews  //body data: username,content
- update a review: PUT /api/reviews/id  //body data: username,content
- delete a review: DELETE /api/reviews/id 
- sign up a user: POST /api/signup	//body data: username,password
- I add the basic auth strategy for the api, hence you should use the user signup api firstly to create authentication user and password for other APIs.

###Data Models:
review
- username:owner of review
- content: review content
- createdAt: the created datetime
- updatedAt: the updated datetime

user
- username: user name
- password: user password

###Folds:
- server.js: index file
- app/models: data model files
- app/controllers: user authentication logic
- fakeReviewsData.js: fake some reviews

###Implementation:
- local mongodb
- $npm install
- $node fakeReviewsData.js  // insert some fake reviews into the mongodb
- $grunt



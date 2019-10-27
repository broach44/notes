# Class Notes - 10/26/2019

By the end of the day we will be calling data and passing it to the page.

## JSON

- What is returned when you access an API.
- Javascript Object with quotes around the keys
- JSON Files will not accept comments
- Check syntax for errors with [Jsonlint](https://jsonlint.com/)
- Use every time you are writing a Json file, upload to check when ready.
- Firebase is an object storage database, you have to upload an object of objects.
- When we pull the code in we have to make it an array of objects.

## ERDs
- Entity relationship diagrams
- used when doing architecture for a new api
- need an agreement on what will be in the database
- Map out the relationships between the different types of tables, what data types and relationships between the tables
- Id's are important because they are unique
- Join tables used to make the relationship between the various different tables in the database
- firebase calls them collections
- backend calls them tables

|Bears   |Equipment  |Hunters         |
|------- |-----------|----------------|
|id      |id         |id              |
|type    |name       |age             |
|color   |description|license         |
|lastMeal|quantity   |numYearsHunting |
|size    |cost       |numKills        |
|weight  |           |location        |
|isHungry|           |                |
|location|           |                |



|Kills      |HunterEquipment|
|-----------|---------------|
|id         |id             |
|bearId     |hunterId       |
|hunterId   |equipmentId    |
|equipmentId|               |

- Above is an ERD once you draw the arrows to connect the relationship between the tables
- they will review the collections because there is a "wrong" way that will not work well
- make decisions on how to arrange your collections dependent on what you are trying to do in your application
- Tool - [Lucid Chart](http://www.lucidchart.com)
- Update chart if you make changes, then update the tickets
- symbols stand for the type of relationship, one or many.
- Emergency room - ERD - create a diagram - what information to collect to keep track of the patient.  Start with paper - then make a lucid chart
- Each collection will get a separate Json file

## Axios

need .then and .catch 
promise based

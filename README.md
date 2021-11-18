JAVAEE Final MINI PROJECT - 18000509

Build And Run

1. Open a terminal and go to the project folder
2. Run "./gradlew build -Dquarkus.package.type=uber-jar" to build the app
# Observe if there is a build folder with a jar file, or else use eclipse (intellij) ide build tool
3. Run "java -jar build/petstore-runner.jar" to run the app

API End points


Note - In the beginning there is no data in the list, therefore first input some data to retreive data.
Use 3rd party application to run and see results on the APIs (Get methods can be viewed in web browser)

*Add a pet
	url : http://localhost:8080/v1/pets
	method : POST
	body : {
		    "petName" : "buula",
		    "petType" : "dog",
		    "petAge" : 3
		}

*Get all pets
	url : http://localhost:8080/v1/pets
	method : GET

*Get a pet by ID
	url : http://localhost:8080/v1/pets/1
	method : GET

*Delete a pet
	url : http://localhost:8080/v1/pets/1
	method : DELETE
	
*Update a pet
	url : http://localhost:8080/v1/pets
	method : PUT
	body : {
		    "petId": 1,
		    "petName" : "brownie",
		    "petType" : "dog",
		    "petAge" : 3
		}
		
*Add a pet type
	url : http://localhost:8080/v1/pets/petTypes
	method : POST
	body : {
		    "petType" : "dog"
		}

*Get all pet types
	url : http://localhost:8080/v1/pets/petTypes
	method : GET

*Get a pet type by ID
	url : http://localhost:8080/v1/pets/petTypes/1
	method : GET
	
*Update a pet type
	url : http://localhost:8080/v1/pets/petTypes
	method : PUT
	body : {
		    "petType" : "black dog",
		    "petTypeId": 1
		}

*Delete a pet type
	url : http://localhost:8080/v1/pets/pettypes/1
	method : DELETE

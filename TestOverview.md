
--Creating pets

-should create a new pet when all required fields are provided: This test case verifies that a new pet can be created when all required fields are provided. It expects a 200 status code and the created pet in the response.

-should return a 200 status code and a pet object with default values when pet data is empty: This test case verifies that a pet can be created with default values when no data is provided. It expects a 200 status code and a pet object with default values in the response.



--Deleting pets

-should return 404 when a non-existing ID is provided: This test case verifies that a 404 status code is returned when trying to delete a pet with a non-existing ID.

-should return an error when an invalid ID is provided: This test case verifies that an error is returned when trying to delete a pet with an invalid ID.



--Finding Pets by status

-should find pets by status: This test case verifies that pets can be found by their status. It expects an array of pets with the specified status in the response.

-should find pets with status {status}: This test case verifies that pets can be found by their status for each status in ['pending', 'sold']. It expects an array of pets with the specified status in the response.

-should return an empty array for invalid status: This test case verifies that an empty array is returned when trying to find pets with an invalid status.



--Finding pets by ID

-should return 404 for non-existing ID: This test case verifies that a 404 status code is returned when trying to find a pet with a non-existing ID.

-should return an error for invalid ID: This test case verifies that an error is returned when trying to find a pet with an invalid ID.

-should return an error when ID is not provided: This test case verifies that an error is returned when trying to find a pet without providing an ID.



--Updating pets

-should return 405 when a valid ID and data are provided: This test case verifies that a 405 status code is returned when trying to update a pet with a valid ID and data.

-should return 405 when a non-existing ID is provided: This test case verifies that a 405 status code is returned when trying to update a pet with a non-existing ID.

-should return 200 and the created pet when ID is not provided: This test case verifies that a new pet is created and returned when trying to update a pet without providing an ID. It expects a 200 status code and the created pet in the response.
# CareersService

Used :  Spring Web flux(Reactive Spring REST API), Cassandra DB, Kafka, Hazelcast, Spring Web client

Implemented a Springboot REST endpoint createJobProfile that will perform the following.
-	Persist job profile information, provided as input, into Cassandra table - “job”.

Implemented a Springboot REST endpoint findEmpForJobID that will perform the following.
-	Finds the years of experience required for the provided JobId, from Cassandra (job table)
-	Makes an HTTP non-blocking call to EmployeeService microservice using the endpoint - findEmpSkillSet
-	Returns all employees that match the information.

Implemented a Springboot REST Endpoint that performs operations on the Hazelcast cache for Job table.
-	Queries Hazelcast cache for Job information (by jobID)

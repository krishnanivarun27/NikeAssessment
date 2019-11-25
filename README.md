# NikeAssessment

This project is meant to access the overall understanding of data transformation and test your skills on Apache Spark and its integration with various other technologies.

Given : 
You have 2 CSV files representing station and bike's trip data. 

Ask : 
The objective is to read the data from both files and transform it to produce an output in JSON format. 
The output should provide the total duration travelled by a bike on each route (start station -> end station) along with a list of the stations landmarks. 
If the landmark for both the start and end stations is same then only one landmark should be recorded in the output.

The output JSON payload must be written to a persistence data store like DynamoDB or S3 or HDFS. 

Below is a sample of the json that needs to be created for each bike per route:

    {
        "bike" : 123,
        "start_station" : "St James Park",
        "end_station" : "Japanton",
        "landmarks" : ["San Jose"],
        "total_duration" : 3000
    }
    

The assessment can be done in Python/Java/Scala.(we prefer python though).The output should contain well written Unit tests with atleast 90% code coverage. 
Also, please ensure all coding standards and best practices are followed.

Following build tools to be used(depending upon the programming language) : 

* Java : Maven
* Scala : sbt
* Python : pybuilder

You can also run this on any cloud environment of your choice.See attached environment file for details.


Once done, please upload your solution to GitLab and grant access to @varun.krishnani for further review process.
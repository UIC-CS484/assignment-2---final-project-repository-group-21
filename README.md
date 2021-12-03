# CHIdata
[![Node.js CI](https://github.com/UIC-CS484/assignment-2---final-project-repository-group-21/actions/workflows/node.js.yml/badge.svg)](https://github.com/UIC-CS484/assignment-2---final-project-repository-group-21/actions/workflows/node.js.yml)
[website](https://chidata.herokuapp.com/)

This application will help end users to be informed about their communities. The application is connected to the Chicago Data Portal to get data about Chicago Police crime data as well as have connections to city employee data.


#### API Connections
- Connected to the Chicago Police Crime database via [Chicago Data Portal](https://data.cityofchicago.org/)
- Connected to the Service Request api to get all the service requests made in the city
- API calls made using ajax
    ```
     $.get("https://data.cityofchicago.org/resource/crimes.json",
            function (e) {
                $.each(e, function (i, v) {
                    //data.addRows([v.case_number]);
                    apiData.push([v.case_number, v.primary_type, v.description, v.ward, v.district, v.arrest, v.year]);

                }); // end of the callback function and parameter list for $.each
            }); //  end of the callback function and parameter list for $.get 
    ```
    
#### Tools
- Google Charts Library
- Google maps api (currently not fully integrated and not working)


#### Team Member
Biruk Yigzaw






#### Assignment 3:
Requirement 1:
- Database for the users to sign in and out. Just logs username, password, and lastlogon time.
![image](https://user-images.githubusercontent.com/54635639/142281737-1d5b0bad-c4e2-4817-abdd-c148c6b2f6b9.png)

Requirement 2:



Requirement 3: RESTFul API
- API connection made to the Chicago Police Crime database.

Requirement 4: Front-end data Manipulation using table, chart, map ...
- From the API connectiong made in requirment 3 and the result from the API connection is sorted and added into
a chart/table using Google Charts library visualiation table. This gives the users raw data dump were user can look up results from the database.



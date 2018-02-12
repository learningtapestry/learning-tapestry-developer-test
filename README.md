# Learning Registry Developer Test

This is a test project to assess a software developer's skills.

## Requirements

- Use .NET Core
- Use an RDBMS
- Use an ORM
- Use git
- Aside from the libraries referenced in the instructions, use whichever libraries
  you prefer

## Test submission

Submit the test using a [git bundle](https://git-scm.com/blog/2010/03/10/bundles.html).

## Instructions

In this project, you will create a backend API as well as a frontend client to the API.

### Backend API

Implement the following endpoints:

- [GET] `/resources?page={page}`: paginate records from the database and return
them as JSON. Each record must be returned with all its associated information.

- [GET] `/resources/reports/domains`: show the total number of resources for
each domain name in the database (use the `resource_locator` property to find
the domain name).

- [POST] `/resources/refresh`: pull data
  from the [LR API](http://node01.public.learningregistry.net/) (3000 records
  are enough). Parse the data and store it in the database. You can design the
  database model however you prefer. Delete old data before storing the new records.
  [Documentation for the LR API.](https://github.com/LearningRegistry/LearningRegistry/wiki/Consuming-Learning-Registry-Records#1--harvesting-records)

### Frontend client

The frontend client must be implemented using
[create-react-app](https://github.com/facebook/create-react-app). Don't worry
about making it look good.

- Show a list of records with basic information. Paginate the list.
- Allow the user to click a record to see the value of its `resource_data`
  property.
- Show a "Refresh data" button that allows the user to trigger a refresh.

### Tests

- Write a test for the `/resources` endpoint verifying that it's returning
  records.

- Write a test for the `/resources/reports/domains` endpoint verifying that
  it's aggregating records.

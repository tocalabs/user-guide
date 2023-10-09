# Making API Calls in Toca

**Purpose:** This section aims to guide you through the process of making API calls to external services, as well as managing the data returned from these calls.  
**Prerequisites:** To get the most out of this guide, you should have access to Toca and possess a foundational understanding of Actions and workflows. Basic knowledge of HTTPS and RESTful services is also recommended.

## Table of Contents

1. [Introduction to API Calls](#making-api-calls-in-toca)
2. [Working Example](#the-working-example)
3. [Utilising the postcodes.io Service](#utilising-the-postcodesio-service)
4. [Making GET and POST Calls](#making-get-and-post-calls)
5. [Managing Data](#managing-data)

## Introduction to API Calls

In today's interconnected digital landscape, API calls serve as the critical links between different systems and services. Whether you're dealing with JSON, XML, or any other bespoke data format, API calls facilitate the transfer of data between servers and services. This section explores how to make GET and POST calls using Toca and how to parse the returned data into a Toca datastore.

## The Working Example

For this working example, we will assume the need to create two services: one that captures the area of a postcode and another that captures the postcode itself. We will be using the open-source [postcodes.io](https://postcodes.io/) service for this purpose.

## Utilising the postcodes.io Service

The [postcodes.io](https://postcodes.io/) service is a free, open-source API that provides postcode and geolocation data specifically for the UK. We'll use this service as a case study to demonstrate how to make API calls within Toca.

### Postcodes.io GET Service

The documentation for the Postcodes.io GET service can be found [here](https://postcodes.io/docs).

The format of the response is as below:

```JSON
{
    "status": 200,
    "result": {
        "postcode": "SW1A 2AA",
        // ... other fields ...
    }
}
```

We will cover how to use Toca to access this service and manage the response into a new format under the section `Creating a GET Request`.

### Postcodes.io POST Service

The Postcodes.io POST service requires an HTTP POST message along with a JSON body. This will be covered in a subsequent section.

The required JSON body format is as follows:

```JSON
{
  "postcodes": ["SW1A 2AA", "M45 6GN", "EX165BL"]
}
```

The response format is quite large, but a truncated version is provided below:

```JSON
{
    "status": 200,
    "result": [
        {
            "query": "SW1A 2AA",
            // ... other fields ...
        }
    ]
}
```

## Managing Data

To manage the captured data, we will use a Toca datastore to create a table that captures both the `postcode` and the `admin_district`. These values will then be available for use in other services. Storing this data in a datastore is key to utilising various types of data later in our automation workflows or apps.

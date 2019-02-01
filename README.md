# Dummy Brief

We understand that being a good developer does not mean being able to recite how specific functions like spaceship operators work, or the Liskov substitution principle in your sleep.

We understand that a good developer is somebody who is not afraid to not know the answer, but are able to use the resource available to them to find suitable solutions to the problems they are faced with, and the ability to adapt their knowledge to different circumstances.

For this test we’ll be providing you with a small brief to potentially put you outside of your comfort zones to produce a few simple components which should solve a small problem, **sometimes you're required to work with platforms you're unfamiliar with outside of your day to day roles, imagine this is one of those moments.**

## The Brief

You have a new client, who can **only runs NodeJS applications** on their server, which means they cannot run anything like PHP, Ruby or Python etc for this dummy project.

Although you're not a Node developer, you understand how javascript works, understand basic design principles, how a REST API works and are self-sufficient. You believe you can cobble something together to suit the client's needs.

The client needs a NodeJS CLI tool which accesses their EPOS API to generate some basic reports.

The task should ideally take **no longer than 1 hour 30 minutes**, depending on your experience.

### Feature One

The first report should generate a .csv file of all the orders with the following headers

OrderID | HasCustomerPaid | CustomerName | CustomerEmail
------- | --------------- | ------------ | ------------- 

The client does not mind if the .csv file is not generated to the file system, however he says he’ll give a large bonus if this is done correctly with timestamped files.

The EPOS API provides an API endpoint to return this information.

It also requires all API requests to authenticate by using a HTTP Request header named `X-AUTHORISATION` - They’ve provided you with an API token of `R4o6rHAvpEhUOmVR`

Method | Endpoint
-------| -------
GET    | https://dummy-api.selesti.agency/orders


### Feature Two

The client also needs a way to generate a .csv of a specific customer’s order.

He expects to be able to pass in the order id, and get the .csv generated based upon that.

The client does not mind if the .csv file is not generated to the file system, however he says he’ll give a large bonus if this is done correctly with timestamped files.

The format for the .csv should be as follows

OrderID | HasCustomerPaid | CustomerName | CustomerEmail | NumberOfItemsPurchased | TotalOrderPriceInPounds |
------- | --------------- | ------------ | ------------- | ---------------------- | ----------------------- |

As before the EPOS API provides an endpoint protected by the previously mentioned API key.

Method | Endpoint
-------| -------
GET    | https://dummy-api.selesti.agency/orders/{OrderID}


The client has also kindly supplied a Postman collection for easy API debugging

https://www.getpostman.com/collections/61722bfa245b4e26a85b

## Project Delivery

As there are such high-security restrictions on the server, the client requires the package to be zipped up and delivered over to his team for testing.

They have left a note to make sure they exclude the `node_modules` from the zip as they have an enterprise mirror which they’ll use.

The client understands that your team are not NodeJS developers and has suggested if they have any questions about the project they can email `dummyapi@selesti.com` for any clarification.

```
  ___   ___    _  _  ___ _____   ___ _   _ ___ _    ___ ___ _  _    ___  _  _ _    ___ _  _ ___ 
 |   \ / _ \  | \| |/ _ \_   _| | _ \ | | | _ ) |  |_ _/ __| || |  / _ \| \| | |  |_ _| \| | __|
 | |) | (_) | | .` | (_) || |   |  _/ |_| | _ \ |__ | |\__ \ __ | | (_) | .` | |__ | || .` | _| 
 |___/ \___/  |_|\_|\___/ |_|   |_|  \___/|___/____|___|___/_||_|  \___/|_|\_|____|___|_|\_|___|                            
```

**Please do not publish your results online via any platform, including Github - failing to follow this instruction could lead to immediate dismissal of applicants.**


## Example

The client has also provided an example prototype video which can be viewed by following the below link `https://asciinema.org/a/123175` for inspiration.

[![asciicast](https://asciinema.org/a/123175.png)](https://asciinema.org/a/123175)

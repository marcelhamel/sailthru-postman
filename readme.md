This Postman collection is designed to demonstrate some of the more common API requests made to Sailthru. Due to the nature of how these API's are built, each request (POST, GET, multi-part form uploads) will be structured differently within Postman. Please see the instructions below on how to import this collection and how to test with each request type.

- For implementations of Sailthru API's, it is highly recommended that users leverage one of Sailthru's [client libraries](https://getstarted.sailthru.com/developers/api-client/libraries-overview/).
- If you are a Sailthru user, most of these requests can be tested with the [API Test Tool](https://my.sailthru.com/api/test) within the Sailthru UI.
- For more information on JSON payloads for each endpoint, check out the [Sailthru API Documentation](https://getstarted.sailthru.com/developers/api-basics/introduction/).

## Installation
1. If you don't already have Postman installed, you'll need to head to [Postman.com](https://www.postman.com) to download and install the program as well as register with them.
2. To import this collection, begin by downloading this code repository by clicking Code > Download ZIP. 
3. Open the ZIP file once downloaded to unpack it's contents.
4. Within Postman, go to File > Import.
5. Select "Upload Files" in the dialogue that appears, and select "Sailthru API.postman_collection.json" from the ZIP file you've just unpacked.
6. Click "Import" to finish importing the collection.

## Setting up your environment
1. This collection references API credentials as environment variables. Before making requests with this collection, you'll first need to [create an environment in Postman](https://learning.postman.com/docs/sending-requests/managing-environments/#creating-environments).
2. Within this environment, you'll want to setup your Sailthru API key with a key "api_key" and your secret with a key of "secret":

![Create A New Environment](https://media.sailthru.com/5p6/1k5/3/8/60462ea0dd264.png)

## Making Requests
Requests to the Sailthru API ended up being structured and sent differently based on the type of request. See the notes below for information on how to use Postman to make requests to the Sailthru API:

### GET Requests
To use any of the GET requests in the collection, simply browse to the "body" tab and enter the request body (JSON payload from the Sailthru documentation) as raw JSON.

![GET request screenshot](https://media.sailthru.com/5p6/1k5/3/8/604630eb3c91b.png)


### POST Requests
To use any of the POST requests in the collection, browse to the "body" tab. You'll see that the request body type is "x-www-form-urlencoded". Here, you'll need add the JSON payload for your request in the form field labeled "JSON".

![POST request screenshot](https://media.sailthru.com/5p6/1k5/3/8/6046324389397.png)

### Multi-part Upload Requests
Several of the "jobs" performed by Sailthru's Job API accept file uploads. For these, you'll want to add your JSON payload in the "json" form field as you would with a regular POST request. You'll also need to select the file you wish to upload under the "file" form field:

![UPLOAD request screenshot](https://media.sailthru.com/5p6/1k5/3/8/6046335d30377.png)

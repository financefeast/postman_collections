# Postman Collections for Financefeast environments

[Postman](https://www.postman.com/downloads/) collections for [Financefeast](https://financefeast.io) stock data API. Each endpoint is pre-configured and all you need to do is
enter your client id and client secret into the "Environments" variables CLIENT_ID and CLIENT_SECRET. Your client id and client secret can be found [here](https://customer.financefeast.io).

## Prerequisites

1. [download Postman](https://www.postman.com/downloads/)
2. Clone this repository to your local PC

## Usage

### Import into Postman
Inside each folder, eg "test" are two json files, named "something_collection.json" and "something_environment.json". These need to be imported into Postman.
[click here](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#importing-data-into-postman) for steps on how to import into Postman.

### Enter your client credentials
Under "Environments", select "Test" and you should see a list of variables. Enter your client id into CLIENT_ID and your client secret into CLIENT_SECRET.

### Authenticate
Under "Collections", run "Login" which will attempt to authenticate your client credentials. If successfull you will see a Bearer token. This will automatically be saved as an
environment variable "TOKEN" and used to authenticate all other requests to end points.

### Call an endpoint
Once you are authenticated, under "Collections", run "EOD". You should see data for the pre-defined ticker. You can change the ticker, and the date by changing the query params.

## Getting help
Raise a [Github issue](https://github.com/issues) and one of the team will respond.
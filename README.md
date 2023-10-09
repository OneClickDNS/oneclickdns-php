# OneClickDNS PHP Client
A PHP client for the OneClickDNS API.

## Documentation
Coming soon.

## Requirements
* PHP ^7.3
* PHP ^8.0

## Usage
This library is a PHP client you can use to interact with the OneClickDNS API. Here are some examples.
```
use OneClickDNS\Client;
$client = new Client("API_TOKEN");

$response = $client->identity->whoami();
$whoami = $response->getData();
$account_id = $whoami->account->id;

$response = $client->domains->listDomains($account_id);
$domains = $response->getData();
```

## Sandbox Environment
Coming soon.

## License
Copyright (c) 2011-2023 Linsday Networks. This is Free Software distributed under the MIT license.

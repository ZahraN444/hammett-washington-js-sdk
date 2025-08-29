
# Getting Started with APIMATIC Calculator

## Introduction

Simple calculator API hosted on APIMATIC

## Install the Package

Run the following command from your project directory to install the package from npm:

```bash
npm install hammett-washington-sdk@1.7.6
```

For additional package details, see the [Npm page for the hammett-washington-sdk@1.7.6 npm](https://www.npmjs.com/package/hammett-washington-sdk/v/1.7.6).

## Test the SDK

To validate the functionality of this SDK, you can execute all tests located in the `test` directory. This SDK utilizes `Jest` as both the testing framework and test runner.

To run the tests, navigate to the root directory of the SDK and execute the following command:

```bash
npm run test
```

Or you can also run tests with coverage report:

```bash
npm run test:coverage
```

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/ZahraN444/hammett-washington-js-sdk/tree/1.7.6/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | `Environment` | The API environment. <br> **Default: `Environment.Production`** |
| timeout | `number` | Timeout for API calls.<br>*Default*: `0` |
| httpClientOptions | [`Partial<HttpClientOptions>`](https://www.github.com/ZahraN444/hammett-washington-js-sdk/tree/1.7.6/doc/http-client-options.md) | Stable configurable http client options. |
| unstableHttpClientOptions | `any` | Unstable configurable http client options. |

The API client can be initialized as follows:

```ts
import { Client, Environment } from 'hammett-washington-sdk';

const client = new Client({
  timeout: 0,
  environment: Environment.Production,
});
```

## List of APIs

* [Simple Calculator](https://www.github.com/ZahraN444/hammett-washington-js-sdk/tree/1.7.6/doc/controllers/simple-calculator.md)

## SDK Infrastructure

### Configuration

* [HttpClientOptions](https://www.github.com/ZahraN444/hammett-washington-js-sdk/tree/1.7.6/doc/http-client-options.md)
* [RetryConfiguration](https://www.github.com/ZahraN444/hammett-washington-js-sdk/tree/1.7.6/doc/retry-configuration.md)
* [ProxySettings](https://www.github.com/ZahraN444/hammett-washington-js-sdk/tree/1.7.6/doc/proxy-settings.md)

### HTTP

* [HttpRequest](https://www.github.com/ZahraN444/hammett-washington-js-sdk/tree/1.7.6/doc/http-request.md)

### Utilities

* [ApiResponse](https://www.github.com/ZahraN444/hammett-washington-js-sdk/tree/1.7.6/doc/api-response.md)
* [ApiError](https://www.github.com/ZahraN444/hammett-washington-js-sdk/tree/1.7.6/doc/api-error.md)



# Getting Started with Sample API

## Introduction

API specification with a long data type field

## Install the Package

Run the following command from your project directory to install the package from npm:

```bash
npm install qa-testing-one-of-sdk@1.1.2
```

For additional package details, see the [Npm page for the qa-testing-one-of-sdk@1.1.2 npm](https://www.npmjs.com/package/qa-testing-one-of-sdk/v/1.1.2).

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

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/tahaali2000/qa-testing-one-of-js-sdk/tree/1.1.2/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| timeout | `number` | Timeout for API calls.<br>*Default*: `0` |
| httpClientOptions | [`Partial<HttpClientOptions>`](https://www.github.com/tahaali2000/qa-testing-one-of-js-sdk/tree/1.1.2/doc/http-client-options.md) | Stable configurable http client options. |
| unstableHttpClientOptions | `any` | Unstable configurable http client options. |

The API client can be initialized as follows:

```ts
const client = new Client({
  timeout: 0,
});
```

## List of APIs

* [API](https://www.github.com/tahaali2000/qa-testing-one-of-js-sdk/tree/1.1.2/doc/controllers/api.md)

## SDK Infrastructure

### Configuration

* [HttpClientOptions](https://www.github.com/tahaali2000/qa-testing-one-of-js-sdk/tree/1.1.2/doc/http-client-options.md)
* [RetryConfiguration](https://www.github.com/tahaali2000/qa-testing-one-of-js-sdk/tree/1.1.2/doc/retry-configuration.md)

### HTTP

* [HttpRequest](https://www.github.com/tahaali2000/qa-testing-one-of-js-sdk/tree/1.1.2/doc/http-request.md)

### Utilities

* [ApiResponse](https://www.github.com/tahaali2000/qa-testing-one-of-js-sdk/tree/1.1.2/doc/api-response.md)
* [ApiError](https://www.github.com/tahaali2000/qa-testing-one-of-js-sdk/tree/1.1.2/doc/api-error.md)


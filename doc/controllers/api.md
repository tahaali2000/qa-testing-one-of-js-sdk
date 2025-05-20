# API

```ts
const apiController = new ApiController(client);
```

## Class Name

`ApiController`

## Methods

* [Get a List of Items](../../doc/controllers/api.md#get-a-list-of-items)
* [Create a New Item](../../doc/controllers/api.md#create-a-new-item)


# Get a List of Items

```ts
async getAListOfItems(
  requestOptions?: RequestOptions
): Promise<ApiResponse<ItemsResponse>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [ItemsResponse](../../doc/models/items-response.md).

## Example Usage

```ts
try {
  const { result, ...httpResponse } = await apiController.getAListOfItems();
  // Get more response info...
  // const { statusCode, headers } = httpResponse;
} catch (error) {
  if (error instanceof ApiError) {
    const errors = error.result;
    // const { statusCode, headers } = error;
  }
}
```


# Create a New Item

```ts
async createANewItem(
  body: ItemsRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`ItemsRequest`](../../doc/models/items-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const body: ItemsRequest = {
};

try {
  const { result, ...httpResponse } = await apiController.createANewItem(body);
  // Get more response info...
  // const { statusCode, headers } = httpResponse;
} catch (error) {
  if (error instanceof ApiError) {
    const errors = error.result;
    // const { statusCode, headers } = error;
  }
}
```


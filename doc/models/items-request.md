
# Items Request

## Structure

`ItemsRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `bigint \| undefined` | Optional | - |
| `name` | `string \| undefined` | Optional | - |
| `value` | `bigint \| undefined` | Optional | - |
| `tags` | `string[] \| undefined` | Optional | - |
| `metadata` | `Record<string, string> \| undefined` | Optional | - |
| `details` | [`Details \| undefined`](../../doc/models/details.md) | Optional | - |
| `status` | [`StatusEnum \| undefined`](../../doc/models/status-enum.md) | Optional | - |
| `pricing` | [`ItemsRequestPricing \| undefined`](../../doc/models/containers/items-request-pricing.md) | Optional | This is a container for any-of cases. |

## Example (as JSON)

```json
{
  "id": 140,
  "name": "name6",
  "value": 92,
  "tags": [
    "tags1",
    "tags2",
    "tags3"
  ],
  "metadata": {
    "key0": "metadata7",
    "key1": "metadata8"
  }
}
```


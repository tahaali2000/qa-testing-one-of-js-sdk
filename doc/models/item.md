
# Item

## Structure

`Item`

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
| `pricing` | [`ItemPricing \| undefined`](../../doc/models/containers/item-pricing.md) | Optional | This is a container for one-of cases. |

## Example (as JSON)

```json
{
  "id": 106,
  "name": "name2",
  "value": 58,
  "tags": [
    "tags7"
  ],
  "metadata": {
    "key0": "metadata9"
  }
}
```


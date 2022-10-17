# Error Code

| Code                          | Description                                                                     |
| ----------------------------- | ------------------------------------------------------------------------------- |
| 'success'                     | General success code                                                            |
| 'error'                       | General fail code                                                               |
| 'no-record'                   | No data in the database                                                         |
| 'duplicated-data'             | Record is duplicated                                                            |
| 'suspect-error'               | Errors are not detected. But, error(s) may happened while processing a request. |
| 'access-denied'               | Do not have permission to access.                                               |
| 'url-not-exist'               | Request url is not exist.                                                       |
| 'service-not-available'       | Service is not available. (Service Registry)                                    |
| 'token-not-exist'             | JWT token is not exist.                                                         |
| 'invalid-token'               | Invalid JWT token.                                                              |
| 'requestor-not-exist'         | Requestor info in request header is not exist.                                  |
| 'too-many-failure'            | Too many failure. (e.g. Sign in)                                                |
| 'not-allowed-for-guest'       | Action from guest is not allowed                                                |
| 'item-not-cancelable'         | Item status, or qty, is not meet cancelable condition.                          |
| 'disabled-value'              | The status of a record(s) is disabled                                           |
| 'no-stock'                    | Out of stock, or stock is not available                                         |
| 'missing-field'               | Some of data field are missing                                                  |
| 'missing-required'            | Required data field is missing                                                  |
| 'invalid-order-state'         | Invalid order state                                                             |
| 'invalid-order-status'        | Invalid order status                                                            |
| 'invalid-dispute-state'       | Invalid dispute state                                                           |
| 'invalid-dispute-status'      | Invalid dispute status                                                          |
| 'cart-key-not-exist'          | Cart key is not exist                                                           |
| 'activation-key-not-exist'    | Account activation key is not exist, or expired                                 |
| 'reset-key-not-exist'         | Password reset is not exist, or expired                                         |
| 'special-price-exceed'        | Special price is higher than regular price                                      |
| 'order-generate-fail'         | Failed to generate order from cart                                              |
| 'customer-generate-fail'      | Failed to generate customer data                                                |
| 'wrong-split-qty'             | Split item qty is equal or greater then item qty                                |
| 'wish-item-exist'             | Same item is already added to wish list                                         |
| 'approve-qty-exceed'          | Approve qty is more than request qty                                            |
| 'wrong-config'                | Configuration is not set, or wrong                                              |
| 'wrong-refund-amount'         | Refund amount is wrong                                                          |
|                               |                                                                                 |
|                               |                                                                                 |
| 'delete-not-allowed'          | Delete action is not allowed                                                    |
| 'account-not-found'           | User name, or email not found                                                   |
| 'password-not-match'          | Password does not match                                                         |
| 'account-not-verified'        | Account does not verified                                                       |
| 'account-not-active'          | Account is in inactive(dormant) state                                           |
|                               |                                                                                 |
|                               |                                                                                 |
|                               |                                                                                 |
|                               |                                                                                 |
| 'product-option-not-selected' | Product option(s) is not selected                                               |
|                               |                                                                                 |

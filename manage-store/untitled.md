# State & Status

## State&#x20;

<table><thead><tr><th width="205.6885928393006">Category</th><th width="200.33333333333331">State Code</th><th>Description</th></tr></thead><tbody><tr><td>Order</td><td>incomplete</td><td></td></tr><tr><td>Order</td><td>pending</td><td></td></tr><tr><td>Order</td><td>processing</td><td></td></tr><tr><td>Order</td><td>complete</td><td></td></tr><tr><td>Order</td><td>on_hold</td><td></td></tr><tr><td>Order</td><td>canceled</td><td></td></tr><tr><td>Dispute</td><td>dispute_review</td><td></td></tr><tr><td>Dispute</td><td>return_processing</td><td></td></tr><tr><td>Dispute</td><td>return_complete</td><td></td></tr><tr><td>Dispute</td><td>replace_processing</td><td></td></tr><tr><td>Dispute</td><td>replace_complete</td><td></td></tr><tr><td>Dispute</td><td>refunded</td><td></td></tr><tr><td>Dispute</td><td>resolved</td><td></td></tr></tbody></table>

## Default Order Status

| State               | Status Code         | Status                 |
| ------------------- | ------------------- | ---------------------- |
| imcomplete          | N/A                 |                        |
| pending             | pending\_payment    | Waiting for payment    |
| processing          | processing          | Preparing for shipping |
| complete            | shipped             | Shipped                |
| on\_hold            | on\_hold            | On Hold                |
| canceled            | canceled            | Canceled               |
| dispute\_review     | dispute\_review     | Dispute in review      |
| return\_processing  | return\_processing  | Return in progress     |
| return\_complete    | return\_complete    | Return finished        |
| replace\_processing | replace\_processing | Replace in progress    |
| replace\_complete   | replace\_complete   | Replace finished       |
| refunded            | refunded            | Refunded               |
| resoled             | resolved            | Dispute Resolved       |

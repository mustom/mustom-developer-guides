# State & Status

## State&#x20;

| Category | State Code          | Description |
| -------- | ------------------- | ----------- |
| Order    | incomplete          |             |
| Order    | pending             |             |
| Order    | processing          |             |
| Order    | complete            |             |
| Order    | on\_hold            |             |
| Order    | canceled            |             |
| Dispute  | dispute\_review     |             |
| Dispute  | return\_processing  |             |
| Dispute  | return\_complete    |             |
| Dispute  | replace\_processing |             |
| Dispute  | replace\_complete   |             |
| Dispute  | refunded            |             |
| Dispute  | resolved            |             |

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

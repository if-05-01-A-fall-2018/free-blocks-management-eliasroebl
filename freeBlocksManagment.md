## 1.

| Block      | 17      | 18     |
|------------|---------|--------|
| Next Block | 18      | -1     |
|            | 4589    | 24353  |
|            | 43536   | 98745  |
|            | 718     | 76345  |
|            | 345     | 9877   |
|            | 23456   | 7345   |
|            | 8345345 | 34535  |
|            | 634534  | 154698 |
|            | 3478    | 967    |
|            | 56      | 8657   |

### a)  Five new blocks are allocated:           

| Block      | 17      | 18     |
|------------|---------|--------|
| Next Block | 18      | -1     |
|            | 4589    | 24353  |
|            | 43536   | 98745  |
|            | 718     | 76345  |
|            | 345     | 9877   |
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 7345   |
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 34535  |
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 154698 |
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 967    |
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 8657   |

### b) The block 22 is freed

| Block      | 17      | 18     |
|------------|---------|--------|
| Next Block | 18      | -1     |
|            | 4589    | 24353  |
|            | 43536   | 98745  |
|            | 718     | 76345  |
|            | 345     | 9877   |
|            |<mark>  22</mark>  | 7345   |
|            || 34535  |
|            || 154698 |
|            || 967    |
|            || 8657   |

### c) Another 5 blocks are allocated

| Block      |17|18|
|------------|---------|--------|
| Next Block |18|-1|
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 24353  |
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 98745  |
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 76345  |
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 9877   |
|            |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>| 7345   |
|            ||34535|
|            ||154698|
|            ||967|
|            ||8657|


### d) Another block is allocated

| Block      |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>|18|
|------------|---------|--------|
| Next Block |<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>|-1|
|            ||24353|
|            ||98745|
|            ||76345|
|            ||9877|
|            ||7345|
|            ||34535|
|            ||154698|
|            ||967|
|            ||8657|

### e) Another three blocks are allocated

| Block      ||18|
|------------|---------|--------|
| Next Block ||-1|
|            ||24353|
|            ||98745|
|            ||76345|
|            ||9877|
|            ||7345|
|            ||34535|
|            ||<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>|
|            ||<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>|
|            ||<mark>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</mark>|

### f) Four blocks(23456,8345345,56 and 634534) are freed

| Block      |<mark>634534</mark>| 18     |
|------------|---------|--------|
| Next Block |<mark>18</mark>| -1     |
|            ||24353|
|            ||98745|
|            ||76345|
|            ||9877|
|            ||7345|
|            ||34535|
|            ||<mark>23456</mark>|
|            ||<mark>8345345</mark>|
|            ||<mark>56</mark>|


## 2.
    Given the two memory footprint scenarios for Free Blocks Managment as presented in class. State the condition under which the linked list approach less space than the bitmap approach.
<br>

    The linked list uses less space then the Bitmap, under the condition that there are less free blocks than the size of the bitmap.
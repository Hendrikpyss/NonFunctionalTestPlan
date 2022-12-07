# Test Case A

### User Story: 
As an end user, I want to be able to cancel my purchase within 1 second so that I am not delayed by the system.

### Critical Problem:
Cancelling a purchase within 1 second

### Test applies to:
GUI system

### Start condition:
Items in the warehouse

| Id | Name | Description| Price | Quantity |
|-----|-----|---------|-----------------|--------|
| 1   | Lays Chips| Potato Chips | 11.0          | 5         |
| 2   | Chupa-chups| Sweets | 8.0          | 8        |
| 3   | Frankfurters| Beer sausages | 15.0          | 12         |
| 4   | Free Beer| Student's delight | 0.0          | 100         |

### Steps to take:
1. Set a timer to 1 second.
2. Press the New Purchase Button
3. Add 5 Lays Chips to the cart (1 in the barcode).
4. Start the timer
5. Press the cancel button
6. Stop the timer
### The test is considered passed
if the order was cancelled within one second, otherwise the test is considered failed
### End condition
The items are not removed from the warehouse, no purchases were made
### Steps to confirm the end condition:
1. Select warehouse tab
2. Check quantity of Lays Chips
3. It must be 5

# Test Case B

### User Story: 
As an end user, I want to be able to remove stock from the warehouse within 1 second so that I am not delayed by the system.

### Critical Problem:
Removing a stock from the warehouse within 1 second

### Test applies to:
GUI system

### Start condition:
Items in the warehouse

| Id | Name | Description| Price | Quantity |
|-----|-----|---------|-----------------|--------|
| 1   | Lays Chips| Potato Chips | 11.0          | 5         |
| 2   | Chupa-chups| Sweets | 8.0          | 8        |
| 3   | Frankfurters| Beer sausages | 15.0          | 12         |
| 4   | Free Beer| Student's delight | 0.0          | 100         |


### Steps to take:
1. Set a timer to 1 second.
2. Go to the warehouse tab
3. Write 4 to the bar code
4. Start the timer
5. Press remove stock button
6. Stop the timer
### The test is considered passed
if the stock was removed within 1 second, otherwise the test is to be considered failed
### End condition
The stock was removed from the warehouse
### Steps to confirm the end condition:
1. Select warehouse tab
2. Check if theres a stock called Free Beer
3. There shouldn't be
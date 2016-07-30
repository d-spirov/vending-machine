## Vending-machine - Entity diagram

The following diagram represents entity-relation for the vending machine.


![Alt text](vending-machine.png?raw=true " Entity diagram")


### Product
- Defines a product which is available in the vending machine. 
- There can be different product types - eg. Snacks, Chocolate, Refreshments etc.

### Coin
- Defines a coin which can be used for payment for the products. Each coin has a certain value.

### VendingMachine
- Defines the vending mahine. 
- Machine state can be Active, Malfunction, Inactive etc.
- Each vending machine contains a bag of coins. For each of the coins amount must be maintained so it is possible to execute transactions requested by the clients. In case is not possible to return amount to the user transaction will be cancelled and coins returned to the user.
- Vending machine contains products. For each product wuantity and price is maintained. Quantity must be up to date in order to know if requested products are available or not.

### Transaction
- Transaction is used to track the payments done by customers in order to buy products. Is good to track the state and changes in the coin bag.
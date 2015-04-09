1. CREATE TABLE receipts (id INTEGER PRIMARY KEY, store TEXT, item TEXT, number_of_items INTEGER, price INTEGER, buy_date TEXT);

2. All the attributes from all the receipts
SELECT * FROM receipts;

3. The store and item names from all the receipts
SELECT store, item FROM receipts;

4. All the attributes from all purchases made at Toys R Us
SELECT * WHERE store = "Toys R Us";

5. The item name of each purchase made at Strand.
SELECT item FROM receipts WHERE store = "Strand";

6. The total number of items Peter purchased
SELECT SUM(number_of_items) FROM receipts;

7. The total number of items purchased at Sears
**answer**

8. All the attributes of receipts where Peter bought multiple items.
**answer**

9. The average number of items purchased on a trip to JC Penny
**answer**

10. Great, now add a new receipt representing the purchase of a single "Heatstreet Maple Bourbon", purchased for $40.99 at "Schnapps Haus" on the most recent fourth of July.
**answer**
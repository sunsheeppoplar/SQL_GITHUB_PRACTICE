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
SELECT SUM(number_of_items) FROM receipts WHERE store = "Sears";

8. All the attributes of receipts where Peter bought multiple items.
SELECT * FROM receipts WHERE number_of_items > 1;

9. The average number of items purchased on a trip to JC Penny
SELECT AVG(number_of_items) FROM receipts WHERE store = "JC Penny";

10. Great, now add a new receipt representing the purchase of a single "Heatstreet Maple Bourbon", purchased for $40.99 at "Schnapps Haus" on the most recent fourth of July.
INSERT INTO receipts (store, item, number_of_items, price, buy_date) VALUES("Schnapps Haus", "Heatstreet Maple Bourbon", 1, 40.99, "July 4 2014");
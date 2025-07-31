### Day 1

**Python Learn:**

* Review `try`/`except` (specific exceptions, `else`/`finally`)
* OOP basics: `class`, `__init__`

**Python Task:**

1. Wrap your billing-input logic in `try`/`except` to catch invalid entries.
2. Define a `Product` class with attributes `name` and `price` and a method `taxed_price()`.

**SQL Learn:**

* INNER JOIN fundamentals (combining two tables)
* Aggregation with `SUM()` and grouping with `GROUP BY`

**SQL Task:**

* Write a query that joins your `orders` and `products` tables to compute **total sales per product**.

---

### Day 2

**Python Learn:**

* Advanced error handling (catching multiple exception types, logging)
* OOP: building a `Customer` class (attributes + methods)

**Python Task:**

1. Refactor billing script so every user action is wrapped in `try`/`except`, logging errors to a file.
2. Instantiate two `Customer` objects and attach `Product` instances via a `Customer.add_order(product, qty)` method.

**SQL Learn:**

* Conditional logic with `CASE WHEN`
* Counting and summing grouped by a conditional bucket

**SQL Task:**

* Add a `category` to each product using `CASE WHEN price > X THEN 'expensive' ELSE 'budget' END`, then **count products per category**.

---

### Day 3

**Python Learn:**

* Input validation in constructors (`raise ValueError`)
* Error handling inside class methods

**Python Task:**

1. In `__init__` of both `Product` and `Customer`, validate inputs (e.g. ensure price > 0) and catch/report invalid data.
2. Refactor billing app to drive entirely through these classes, guarding against invalid operations.

**SQL Learn:**

* Writing **subqueries** in `WHERE` clauses

**SQL Task:**

* Return products whose **total revenue** exceeds the average revenue, by using a subquery that computes the average in the `WHERE` filter.

---

### Day 4

**Python Learn:** Robust file I/O with `with open` and catching `IOError`
**Python Task:** Serialize/deserial­ize your `Customer` list to JSON or pickle, with `try`/`except` around reads/writes

**SQL Learn:** Window functions (`ROW_NUMBER()`, `RANK()`)
**SQL Task:** Rank products by descending revenue using a window function inside a CTE.

---

### Day 5

**Python Learn:** End-to-end exception safety in user I/O, file ops, and logic
**Python Task:** Finalize your class-based billing system, logging **all** exceptions with timestamps

**SQL Learn:** Complex reporting combining JOIN, `CASE`, subquery, and window function
**SQL Task:** Build a comprehensive SQL report that:

1. Joins `orders` & `products`
2. Categorizes with `CASE`
3. Filters via the subquery (above-average revenue)
4. Ranks with a window function
   —document each query’s purpose and sample output.

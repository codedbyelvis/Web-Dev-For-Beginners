# Data Types Practice

## Instructions

Imagine you are building a shopping cart. Write some documentation on the data types that you would need to complete your shopping experience. How did you arrive at your choices?

## Rubric

Criteria | Exemplary | Adequate | Needs Improvement
--- | --- | --- | -- |
||The six data types are listed and explored in detail, documenting their use|Four datatypes are explored|Two data types are explored|

Assuming props gives all of the items data and the checkout button is a reusable component:
1. String - Used to say how many products are in your cart, label all info of the items, and title the different types of calculations(pre-tax, discounts, final total, etc.)
2. Number - Used for all the calculations, especially the final total.
3. Boolean - Used to deselect items from the cart, if a discout is applied to an item, and possibly showing if item is in stock.
4. Undefined - Used for placeholder data for optional fields(check mark for added warranty, empty coupon code section, etc.)
5. Null - Used for placeholder data that is not optional (shipping address info, payment type, etc.)
6. BigInt - This should not be used, as there is no feasible usecase.
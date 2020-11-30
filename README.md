## The problem

Our client is selling the products as shown above:

```
+--------------|--------------|---------+
| Product Code |     Name     |  Price  |
+--------------|--------------|---------+
|     DRINK-1  |   Matcha Tea |  $2.40  |
|     VEGGS-1  |   Carot 1kg  |  $1.80  |
|     DRINK-2  |   Cafe Latte |  $2.50  |
+--------------|--------------|---------+
```

Our client needs to implement these custom promotional rules:
- Buy 2 get 1 free discount: If someone buy 2 Matcha Tea, it will get one free
- Bulk discount: If someone buy 2 kg or more of carots, it will get a 20% discount over the carots pricing.
Our client wants the possibility to create new rules.

Expected business code would be:

```ruby
cart = Cart.new(pricing_rules)
cart.add(item)
cart.add(item)
# ...
price = cart.total
```

Implement a cart and promotional system following these rules.

Test set:

```
Cart content: DRINK-1, DRINK-1, DRINK-1, VEGGS-1
Total price expected:  $6.60

Cart content: VEGGS-1, VEGGS-1, VEGGS-1, DRINK-2
Total price expected:  $6.82

Cart content: DRINK-1, VEGGS-1, DRINK-2
Total price expected: $6.70
```

## Your solution

Please send your solution to yacine@iwa.fi with the subject "Test candidature RoR". 
**please do not put your solution online**

The purpose of this test is to see how you architect an application and write proper code.
Spec must be provided with the solution.

If you have any questions, please proceed as you understand and describe them in the mail with the solutions.

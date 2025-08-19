# 💰 Discount Calculator

A simple Python script that calculates the final price of an item **only if** the discount is **20% or more**. If the discount is less than 20%, the original price is returned.

## 📋 Features

- Prompts user to input:
  - Original price of the item
  - Discount percentage
- Applies the discount **only** if it is 20% or higher
- Displays the final price with or without discount
- Gracefully handles non-numeric input

## 🧠 Logic

```python
def calculate_discount(price, discount_percent):
    """
    Calculates the final price after applying discount.
    If discount is 20% or higher, apply it. Otherwise, return original price.
    """
    if discount_percent >= 20:
        discount_amount = price * (discount_percent / 100)
        return price - discount_amount
    else:
        return price

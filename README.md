# PYTHON-3
def calculate_discount(price, discount_percent):
    
    if discount_percent >= 20:
        discount = price * (discount_percent / 100)
        final_price = price - discount
        return final_price
    else:
        # If the discount is less than 20%, return the original price
        return price


price = float(input("Enter the original price of the item: $"))
discount_percent = float(input("Enter the discount percentage: "))


final_price = calculate_discount(price, discount_percent)


if final_price != price:
    print(f"The final price after applying the discount is: ${final_price:.2f}")
else:
    print(f"No discount applied. The original price is: ${final_price:.2f}")

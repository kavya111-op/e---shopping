# E-shopping
The E-Shopping System simulates a basic shopping experience through a command-line interface. A predefined product catalog is displayed to the user, who can select items and quantities. The system validates inputs, calculates total costs, and generates a final bill during checkout.


---

# 🛒 Shopping Cart Application

A simple and interactive **Python-based Shopping Cart CLI Application** that allows users to browse products, add items to a cart, and manage quantities with validation.

---

## 🚀 Features

* 📦 **Product Catalog Display** – View all available products with names and prices.
* 🛍️ **Add Items to Cart** – Add products by entering product ID and quantity.
* ✔️ **Input Validation** – Prevents invalid IDs, negative quantities, and incorrect inputs.
* 🔄 **Cart Updates** – Automatically updates quantity if the product is already added.
* 🖥️ **Beginner-Friendly Python Script** – Great for learning loops, dictionaries, and functions.

---

## 📁 Project Structure

```
shopping-cart/
├── shopping_cart.py
└── README.md
```

---

## 🧩 Code Overview

The project is built using:

* **Dictionaries** for catalog and cart storage
* **Functions** for modular design
* **Try/Except** blocks for safe user input

### Example Snippet

```python
def add_to_cart():
    show_catalog()
    try:
        pid = int(input("Enter product ID to add: "))
        if pid not in catalog:
            print("❌ Invalid product ID!")
            return

        qty = int(input("Enter quantity: "))
        if qty <= 0:
            print("❌ Invalid quantity!")
            return

        if pid in cart:
            cart[pid] += qty
        else:
            cart[pid] = qty
    except ValueError:
        print("❌ Please enter valid numeric input!")
```

---

## ▶️ Running the Program

### Requirements

* Python **3.x** installed on your system

### Run the Program

```
python shopping_cart.py
```

---

## 🧪 Future Enhancements

Possible improvements you can add:

* ✔️ Cart total and billing system
* ✔️ Remove items from cart
* ✔️ Discount or coupon system
* ✔️ Save cart data to a file
* ✔️ GUI version using Tkinter or PyQt

---

## 📘 License

This project is **open-source** and free to modify or distribute.

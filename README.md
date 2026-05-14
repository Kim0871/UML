# Kiosk Ordering System

## Overview

This project is a console-based **food ordering kiosk system** built in Java.  It simulates an order at a food booth where users can browse a menu, customize drinks and sandwiches and generate a final receipt.
The project is designed to demonstrate multiple **Gang of Four Design Patterns** in a practical way.

---

# Features

## Menu System (Composite Pattern)

The menu is structured as a tree:

- Menu
  - Drinks
  - Sandwiches
  - Snacks

Each category can contain:
- subcategories
- products

## Drink Customization (Strategy Pattern)

Users can customize drinks dynamically:

- Cup size (small / medium / large)
- Ice level (yes / no)
- Sugar level (none / 0% / 50% / 100%)

Each customization affects:
- drink description
- drink price

## Sandwich Customization (Decorator Pattern)

Users can build sandwiches by adding/removing ingredients.

### Base sandwiches:
- Chicken Sandwich
- Veggie Sandwich

### Extras:
- Cheese (+1.0)
- Bacon (+1.5)
- Lettuce (+0.5)
- Tomato (+0.5)
- Patty (+1.5)

### Features:
- Add ingredients
- Remove ingredients

---

# Design Patterns Used

## Composite Pattern
Used to represent the menu hierarchy as a tree structure.

- MenuCategory contains Products and subcategories
- Simplifies menu traversal and display

## Strategy Pattern
Used for drink customization.

- Each strategy modifies the drink step-by-step
- Updates both description and price
  
## Decorator Pattern
Used for sandwich customization.

- Each ingredient wraps the base sandwich
- Adds behavior (description + cost)
- Supports dynamic composition

---

# How to Run

## Compile
```bash
javac Main.java
```

---

# Authors

* YannickHan
* Kim T.
* AntoineCrsr

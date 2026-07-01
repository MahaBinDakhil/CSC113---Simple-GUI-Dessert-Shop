# Simple GUI Dessert Shop

A Java Swing desktop application for managing a dessert shop: creating shop details, adding or removing desserts, and calculating costs, all through an interactive GUI.

![Java](https://img.shields.io/badge/Java-Swing-orange?logo=java)

## Overview

Dessert Shop Management System streamlines running a dessert shop by letting the user set up shop details, manage inventory (cakes and cookies), and view cost calculations. The app is built around an object-oriented class hierarchy and a three-frame Swing GUI.

## How It Works

**Frame 1 — Create Store**
The main screen. Collects the shop name, manager's name, manager's age, and number of items to create the shop. From here, the user can also open Frame 2 (Edit Store) or Frame 3 (Display).

**Frame 2 — Edit Store**
Add or delete desserts. Separate tabs let the user add a **Cake** (ID, flavor, size, number of layers, quantity) or a **Cookie** (ID, flavor, size, quantity, optional chocolate chips). Items can also be deleted by ID.

**Frame 3 — Display**
Reads shop data from file and displays it, including shop info, manager info, and all dessert details with costs. Includes a search feature to filter desserts by flavor.

## Exception Handling

- **NumberFormatException** (unchecked) — validates user input
- **IOException** (checked) — manages file read/write errors
- **NegativeNumberException** (user-defined) — handles negative input for quantities, IDs, or other numeric fields

## Data Storage

Shop data (desserts, quantities, total cost) is stored in a text file, `storeInfo.txt`, and saved automatically whenever changes are made.

## Class Structure

- **ShopItems** — abstract base class for all shop items
- **Desserts** — abstract class extending ShopItems, adds flavor, size, and quantity
- **Cake / Cookie** — concrete dessert types
- **Manager** — handles shop-level operations
- **DessertShop / DemoShop** — main application logic
- **Frame1 / Frame2 / Frame3** — Swing GUI screens

## Tech Stack

- **Language:** Java
- **GUI:** Java Swing
- **Storage:** Text file (`storeInfo.txt`)
- **IDE:** NetBeans (uses `.form` files)

## Setup

1. Clone the repo
   ```bash
   git clone https://github.com/KoroNeko0/Simple-GUI-Dessert-Shop.git
   ```
2. Open the project in NetBeans (or import the `.java` files into your preferred IDE).
3. Run `Frame1.java` to launch the application.

## Team

Built for CSC113 (Java 2).

| Role | Name |
|---|---|
| Leader | Maha bin Dakhil |
| Member | Amjad Almalki |
| Member | Amna Abdulkareem |

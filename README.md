Cafe Management System - WinForms Application

## Overview

The Cafe Management System is a Windows Forms (WinForms) application built using C#. This software simulates a simple cafe billing system where users can select various drinks and cakes, calculate costs, generate receipts, and reset the form for new orders.

The project is ideal for learning the basics of WinForms, user interface components, and simple billing systems. This program allows users to:
- Choose from a variety of drinks and cakes
- Calculate the total cost, including tax and service charge
- Generate and print a receipt
- Reset the form for new customers
- Save and open receipt details from text files

---

## Features

1. **Drink and Cake Selection**: 
   - Users can select from a wide variety of drinks such as Latte, Espresso, Mocha, and more.
   - Different cakes are available to choose from, including Coffee Cake, Red Velvet Cake, and Cheesecake.

2. **Billing System**: 
   - The system calculates the total cost of the selected items.
   - It includes a 1.75 service charge and a tax rate of 0.45% applied to the subtotal.

3. **Receipt Generation**: 
   - A detailed receipt is generated, listing the items ordered, the service charge, tax, subtotal, and total cost.
   - The receipt can be printed, saved as a text file, or loaded from a previously saved receipt.

4. **Form Reset**: 
   - All the selected items can be reset to zero, and the checkboxes can be cleared using the reset button.

5. **Print Receipt**: 
   - The application allows users to print the generated receipt.

6. **Save and Open Receipt**: 
   - The receipt can be saved as a text file for future reference, and previously saved receipts can be opened from the file system.

---

## How to Run the Application

### 1. Prerequisites
   - Install [Visual Studio](https://visualstudio.microsoft.com/downloads/) with the ".NET Desktop Development" workload.
   - .NET Framework version 4.7.2 or later.

### 2. Steps to Run

1. **Clone the Repository**:
   - Open a terminal or Git Bash and run the following command:
     ```
     git clone https://github.com/yourusername/CafeManagement.git
     ```
   - Navigate to the project directory:
     ```
     cd CafeManagement
     ```

2. **Open the Project**:
   - Launch Visual Studio.
   - Go to `File` -> `Open` -> `Project/Solution`.
   - Navigate to the cloned project directory and select the `.sln` file (`CafeManagement.sln`).

3. **Build the Solution**:
   - In Visual Studio, go to `Build` -> `Build Solution` or press `Ctrl + Shift + B`.
   - Ensure there are no build errors before proceeding.

4. **Run the Application**:
   - Press `F5` or click the `Start` button in Visual Studio to run the application.

---

## Usage Instructions

Once the application is running, follow these steps to use it:

1. **Select Items**:
   - Check the boxes next to the drinks or cakes you want to order.
   - Enter the quantity for each item by clicking inside the corresponding text box (the text boxes will only be enabled once the corresponding checkbox is checked).

2. **Calculate Total**:
   - Once you have selected your items, click the `Total` button. This will calculate the cost of the drinks, cakes, service charge, and tax.
   - The costs will be displayed in the designated labels.

3. **Generate Receipt**:
   - After calculating the total, click the `Receipt` button. This will generate a detailed receipt in the text area on the right side of the form, including item prices, tax, service charge, and total.

4. **Print, Save, or Load a Receipt**:
   - To print the receipt, click the `Print` button in the toolbar.
   - To save the receipt as a text file, click the `Save` button in the toolbar.
   - To load a previously saved receipt, click the `Open` button in the toolbar and select the file.

5. **Reset the Form**:
   - If you want to clear the current selection and start a new order, click the `Reset` button. This will reset all fields to their default values.

6. **Exit the Application**:
   - To close the application, click the `Exit` button.

---

## Billing Functionality

### Total Calculation

The `Total` button calculates the total cost by considering:
- The price of each selected item
- A fixed service charge of 1.75 units
- A tax of 0.45% applied to the subtotal (the combined cost of items and service charge)

Here’s how the calculation works:
1. For each drink or cake, the total cost is calculated as:
   ```
   Item Total = Quantity of Item * Item Price
   ```
   Example:
   - If you order 2 Lattes and the price of a Latte is 1.20, the total cost for Lattes is:
     ```
     Latte Total = 2 * 1.20 = 2.40
     ```

2. The subtotal is the sum of the total costs of all selected drinks and cakes:
   ```
   Subtotal = Sum of all item totals + Service Charge
   ```

3. The tax is calculated as 0.45% of the subtotal:
   ```
   Tax = Subtotal * 0.0045
   ```

4. The total cost is the sum of the subtotal and the tax:
   ```
   Total Cost = Subtotal + Tax
   ```

### Receipt Generation

The `Receipt` button generates a detailed receipt that includes:
- A list of all the selected items and their respective quantities
- The service charge, tax, and total cost
- The current date and time when the receipt was generated

Example Receipt:
```
-------------------------------------------------------------
                    Cafe de Italiano
-------------------------------------------------------------
Latte                               2
Espresso                            1
Mocha                               3
...
-------------------------------------------------------------
Service Charge                      1.75
-------------------------------------------------------------
Tax                                 0.45
Sub Total                           12.85
Total Cost                          13.30
-------------------------------------------------------------
```

### Reset Functionality

The `Reset` button resets:
- All text fields to `0`
- All checkboxes to unchecked
- All cost labels (cake, drink, service charge, subtotal, tax, and total) to their default values

---

## Future Improvements

Potential enhancements that could be added to the project:
- Adding customization options for item prices.
- Implementing a discount system for large orders.
- Allowing users to customize the tax rate and service charge percentage.
- Creating an admin panel for item management (add, remove, or modify items).

---

## Contributing

Feel free to fork the repository and submit pull requests if you'd like to contribute to the project. Make sure your code is well-documented and follows standard C# coding conventions.

---

### Contact

For any questions or support, feel free to reach out via techgeeklearner@gmail.com or open an issue on GitHub.

---

This README provides a comprehensive guide on how to use, run, and contribute to the project. Let me know if you'd like any further customization!

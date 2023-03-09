### Sem-1 Individual Project for inverntory stock management 

# Inventory Stock Management Program
This program manages the stock of a store. It is written in C and uses a file to store data about the products..

## Structure

The product structure is defined as follows:

    char id[10];   // product code/no.
    char name[20]; // product name
    int quantity;  // remaining quantity of product. Subtract from the original quantity the quantity purchased
    int numSold;   // initially zero, when no purchase yet.
    float price;   // price of one piece of product
    int discount;  // discount for this product
    float sales;   // accumulated sales, total sales for this product
    float value;   // total value of product (quantity * price)

## Functions
The functions are defined as below:

    int writeFile(): writes product data to the file.
    int readFile(): reads product data from the file.
    void disZeroQuant(): displays all products with zero quantity.
    void dispHsale(): displays the product with the highest sale.
    void purchaseprod(): makes a purchase of a product.
    void deleteprod(): deletes a product.
    void addProd(): adds a new product.
    int IDChecker(int i, int j): checks if the product id already exists.
    void editProd(): edits a product.
    int checkID(char id[]): checks if the product id exists.
    void displayprod(): displays all products.
    void worth(): displays the total value of stock.

## Main Function

The main function implements the user interface for the program. It displays a menu with the following options:

    1.) Input new product record.
    2.) Edit a Product.
    3.) Delete a Product
    4.) Display all existing product.
    5.) Make a purchase.
    6.) Display the product record with highest sale.
    7.) Display all product with zero quantity
    8.) Display the total value of stock
    9.) Exit the program.

The user can select an option by entering a number. The program then calls the appropriate function to perform the selected action. The program runs until the user chooses to exit.


# Initializing the bag store
bag_store = {}

# Function to add a bag to the store
def add_bag(brand, price, quality):
    if brand not in bag_store:
        bag_store[brand] = {'price': price, 'quality': quality}
        print(f"The {brand} bag has been added to the store .")
    else:
        print(f"The {brand} bag already exists in the store .")

# Function to display the bag inventory
def display_inventory():
    print("Bag Inventory:")
    for brand, details in bag_store.items():
        price = details['price']
        quality = details['quality']
        print(f"Brand: {brand}  |  Price: ${price}  |  Quality: {quality}")

# Adding initial bags to the store
add_bag('Lacoste', 1000, 'High')
add_bag('Gucci', 10050, 'Medium')
add_bag('Versace', 8000, 'Low')

# Displaying the initial store
display_inventory()

# Interactive loop to add more bags
while True:
    print("\nWhat would you like to do?")
    print("1. Add a new bag")
    print("2. Display bag store")
    print("3. Exit")
    choice = input("Enter your choice (1-3): ")

    if choice == '1':
        brand = input("Enter the brand of the bag: ")
        price = input("Enter the price of the bag: ")
        quality = input("Enter the quality of the bag: ")

        try:
            price = float(price)
            add_bag(brand, price, quality)
        except ValueError:
            print("Invalid price entered. Please try again.")

    elif choice == '2':
        display_inventory()

    elif choice == '3':
        print("Exiting the Bag store. Thank you!")
        break

    else:
        print("Invalid choice. Please enter a valid option (1-3).")



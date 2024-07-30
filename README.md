# ECommerce Product API
<img width="350" alt="image" src="https://github.com/user-attachments/assets/3f3602eb-5035-471d-be14-ee4b911aa4d8">

This repository contains JSON data for various products including clothing, mobile phones, air conditioners, televisions, and more. The data is structured and ready to be used in different applications for testing, development, or educational purposes.

Getting Started
Clone the Repository
To get a local copy of the repository, you can clone it using the following command:


git clone https://github.com/SaiYenugwar/ECommerce-Product-API.git


Accessing the JSON Data
The JSON data is available at the following URL:
[Product.json]([https://raw.githubusercontent.com/SaiYenugwar/ECommerce-Product-API/main/Products.json])

You can directly access and download the JSON file using this link.

Example Usage
You can fetch and use the JSON data in your projects. 

Below are examples :-

JavaScript :-

Get all products

fetch('https://raw.githubusercontent.com/SaiYenugwar/ECommerce-Product-API/main/Products.json')
            .then(res=>res.json())
            .then(json=>console.log(json))

Get a single product by Id

fetch('https://raw.githubusercontent.com/SaiYenugwar/ECommerce-Product-API/main/Products.json')
  .then(res => res.json())
  .then(json => {
    const productId = '1.1';
    const product = json.find(item => item.id === productId);
    console.log(product);
  })

Get products in a specific category

fetch('https://raw.githubusercontent.com/SaiYenugwar/ECommerce-Product-API/main/Products.json')
  .then(res => res.json())
  .then(json => {
    const product = json.filter(item => item.category === "Mobile");
    console.log(product);
  })

# Data Overview
Total Products: 172

Categories: 10 (Men's, Women, Mobile, Watch, Laptop, TV, AC, Monitor, Headphone, Tab)

Sub-Categories under Men's: Shirt, Tshirt, Hoodie, Jeans, Shoes, Jacket

Contact
If you have any questions or suggestions, please feel free to reach out to me at https://saiyenugwar.bio.link



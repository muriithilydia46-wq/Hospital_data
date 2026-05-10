Overview
This project demonstrates how to extract data from different sources using Python, convert it into structured DataFrames, and save the outputs as CSV files. The assignment is divided into two parts.

## Tools & Libraries Used
- **Python** core programming language
- **Jupyter Notebook** development environment
- **requests** for sending HTTP requests to APIs and GitHub
- **pandas** for data manipulation and DataFrame creation
- **Mockaroo** for generating synthetic data

## Part 2: Working with JSON Data from GitHub

### Process
1. **Created a synthetic dataset** using Mockaroo with the following fields:
   - `hospital_name`, `nato_phonetic`, `gender`, `street_address`, `city`
 
2. **Uploaded the JSON file** to a public GitHub repository

3. **Fetched the data using Python** by sending a GET request to the raw GitHub URL using the `requests` library and confirming a successful response (status code 200)

4. **Parsed the JSON response** and converted it into a structured pandas DataFrame

5. **Saved the output** as `mock_hospital_data.csv`

## Part 3: Working with DummyJSON API Endpoints

### Process

#### Products Endpoint — `https://dummyjson.com/products`
1. Sent a GET request to the products endpoint using the `requests` library
2. Confirmed a successful response (status code 200)
3. Extracted the JSON response and accessed the `products` key
4. Converted the products list into a structured pandas DataFrame
5. Saved the output as `products_data.csv`

#### Carts Endpoint — `https://dummyjson.com/carts`
1. Sent a GET request to the carts endpoint using the `requests` library
2. Confirmed a successful response (status code 200)
3. Extracted the JSON response and accessed the `carts` key
4. Flattened the nested product data within each cart into individual rows
5. Converted the flattened data into a structured pandas DataFrame
6. Saved the output as `carts.csv`

# Eat Safe, Love: MongoDB and Python Data Analysis

This repository contains the code and data for a data analysis project focusing on food establishment hygiene ratings in the UK. The project uses MongoDB as the database, along with Python and Jupyter Notebooks for data manipulation and analysis. 

## Repository Contents

The repository is organized as follows:

- **`Resources/`:**
  - **`establishments.json`:** This file contains the initial data for food establishments, stored in JSON format.

- **`NoSQL_analysis_starter.ipynb`:** The Jupyter Notebook file containing the core data analysis code, including:
    - Data import and basic manipulation with PyMongo and Pandas.
    - Implementation of various queries and aggregation pipelines using MongoDB.
    - Code for converting data types and manipulating the data.
    - Displaying of analysis results.

- **`NoSQL_setup_starter.ipynb`:** The Jupyter Notebook file containing the code for setting up the database, including:
    - Creating a connection to the MongoDB database.
    - Importing the initial data from `establishments.json`
    - Adding a new restaurant, updating restaurant information, and deleting records.
    - Updating and verifying data types.

- **`Explanation for nosql-challenge Repo.pdf`:** A PDF document providing explanations about the structure and process followed in the two Jupyter Notebooks.

## Project Goals

The main objectives of this project are to:

1. **Set Up the Database:**
    - Create a MongoDB database named `uk_food`.
    - Import the food establishment data into a collection named `establishments`.
    - Verify data imports, data cleaning, and type conversions.
2. **Update the Database:**
    - Add a new restaurant, "Penang Flavours" to the collection.
    - Update the new restaurant with the correct BusinessTypeID.
    - Delete any establishments belonging to the "Dover" local authority.
    - Convert the string values for the geocode coordinates and rating values to correct numbers (double or int as appropriate).
3. **Perform Exploratory Analysis:**
    - Find the number of establishments with a hygiene score equal to 20.
    - Identify establishments in London with a RatingValue of 4 or greater.
    - Locate the top 5 establishments with a RatingValue of 5, nearest to the new restaurant "Penang Flavours" and sort by the lowest hygiene scores.
    - Determine the count of establishments with a hygiene score of 0 per local authority.

## Tools and Technologies

- **MongoDB:** A document-oriented NoSQL database.
- **Python:** A general-purpose programming language.
- **PyMongo:** A Python driver for interacting with MongoDB.
- **Jupyter Notebook:** An interactive web-based platform for coding and data exploration.
- **Pandas:** A Python library for data analysis and manipulation.

## How to Use This Repository

1. **Clone the Repository:**
    ```bash
    git clone [repository URL]
    ```
2. **Install Dependencies:** Ensure you have Python, pip, PyMongo, and Pandas installed. The easiest way to do this is via Anaconda: https://www.anaconda.com/
    ```bash
    pip install pymongo pandas notebook
    ```
3. **Start a MongoDB server**
    - Follow the MongoDB documentation to get the server running: https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-windows/
    - Once installed, run the server with the command `mongod`

4. **Open the Notebooks:** Open the Jupyter Notebook files (`NoSQL_analysis_starter.ipynb`, `NoSQL_setup_starter.ipynb`) to review the Python code and data analysis processes.

5. **Execute Code:** Run each cell within the Jupyter Notebook files to execute the code, which include database operations, analysis, and visualizations of results.

## Note

- The `Explanation for nosql-challenge Repo.pdf` document provides detailed explanations for each step of the process in the notebooks.

## Contributing
Feel free to fork this repository and contribute to it by adding additional analysis or making improvements.

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

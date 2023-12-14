### Web Scraping GitHub Topics and Top Repositories
This is a Python web scraping project that collects information on GitHub topics and their top repositories using the Beautiful Soup library. 
The script navigates through the GitHub Topics section, extracts the relevant data for each topic, and generates CSV files containing details such as repository name, title, URL, and stars for all repositories under each topic.

### Requirements
Make sure you have the following dependencies installed before running the script:
- Python 3.x
- Beautiful Soup 4
- Requests library

### Getting Started
1. Clone this repository to your local machine using Git.
```bash
git clone https://github.com/your-username/your-repo-name.git
```
2. Install Dependencies:
Before running the script, ensure you have the required Python libraries installed. You can install them using pip.
```bash
pip install beautifulsoup4 requests
```
3. Open the IPython Notebook:
Navigate to the project directory and open the IPython Notebook file github_topic_scraper.ipynb in Jupyter Notebook or JupyterLab.
4. Run the Notebook:
Within Jupyter Notebook, execute the cells in the notebook one by one to run the web scraping script.
5. View the Output:
The notebook will generate CSV files in the output directory, each named after the corresponding topic.
These CSV files will contain information about the top repositories for each topic, including the repository name, title, URL, and stars.

### How it Works
The github_topic_scraper.py script performs the following steps:

- Sends an HTTP request to the GitHub Topics section (https://github.com/topics).
- Retrieves the HTML content of the page using the Requests library.
- Parses the HTML content using Beautiful Soup and extracts the list of topics.
- For each topic, it follows the link to the corresponding page (e.g., https://github.com/topics/{topic-name}).
- Parses the HTML content of the topic page and extracts information about the top repositories (e.g., repository name, title, URL, and stars).
- Generates CSV files for each topic, storing the extracted information for all repositories under that topic.
- The CSV files are saved in the output directory with filenames like topic_name.csv

### Output
The script generates CSV files for each topic in the output directory. Each CSV file will have the following columns:
Repository Name: The name of the repository.
Title: The title of the repository.
URL: The URL of the repository.
Stars: The number of stars the repository has received.

### Disclaimer
This web scraping project is intended for educational purposes only. Always check the website's terms of service and robots.txt before scraping any data.

Happy web scraping!

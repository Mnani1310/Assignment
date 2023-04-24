Word Frequency Microservice

Description

This microservice takes a URL of a static website as input and identifies all the unique words and how many times they occur on the web page. The output is a list of words in JSON format along with the frequency of occurrence (number of times the word is repeated).

How to Install and Run

Clone the repository:

git clone https://github.com/Mnani1310/Assignment.git

Install the dependencies by running the following command in the project directory:


pip install -r requirements.txt

Start the microservice by running the following command:


python app.py

This will start the microservice on http://localhost:5000.


To use the microservice, make a POST request to 

http://localhost:5000/word_frequency with a JSON payload that contains the URL of the website you want to analyze:

json
{
    "url": "https://www.example.com"
}

The microservice will respond with a JSON object that contains the frequency of each unique word on the webpage:

json
{
    "the": 10,
    "quick": 5,
    "brown": 5,
    ...
}

Examples of Usage
Here is an example of how to use the microservice with Python:

go
import requests

url = 'http://localhost:5000/word_frequency'
payload = {'url': 'https://www.example.com'}

response = requests.post(url, json=payload)

if response.status_code == 200:
    print(response.json())
else:
    print('Error:', response.status_code)
    
List of Dependencies
Flask==2.1.1
beautifulsoup4==4.10.0
requests==2.26.0

License Information
This project is licensed under the MIT License. See the LICENSE file for more information.

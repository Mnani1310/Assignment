Project Title: Word Frequency Microservice

Description: This is a microservice built in Python that takes a URL of a static website as an input and identifies all the unique words and their frequency of occurrence on the web page. The output is a JSON object that lists each unique word and its frequency of occurrence.

How to Install and Run the Project:

Clone the project from the GitHub repository:

bash
Copy code
git clone https://github.com/<username>/<repository>.git
Install the required dependencies by running the following command in the project directory:

Copy code
pip install -r requirements.txt
Run the microservice by executing the following command in the project directory:

Copy code
python app.py
The microservice should be up and running on localhost:5000

Examples of How to Use the Project:

Open a web browser and navigate to http://localhost:5000
Enter a URL of a static website in the input field and submit the form.
The microservice will process the URL and return a JSON object that lists each unique word and its frequency of occurrence on the web page.
List of Dependencies:

Flask==2.0.2
requests==2.26.0
beautifulsoup4==4.10.0
License: This project is licensed under the MIT License.

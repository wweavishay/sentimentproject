#Flask Sentiment Analysis Application

This Flask application performs sentiment analysis on text using the NLTK model. It classifies the text as either positive or negative, providing percentages for each classification.

## Running the Application

To run this Flask project, follow these steps:

1. Ensure you have Python installed on your system.

2. Install the required dependencies by running the following command in your terminal or command prompt:
    ```
    pip install -r requirements.txt
    ```

3. Once the dependencies are installed, navigate to the project directory containing the `app.py` file.

4. Run the Flask application using the command:
    ```
    python app.py
    ```

5. Once the application is running, open a web browser and go to `http://127.0.0.1:5002/` 
## Usage

1. Input Text: Enter the text you want to analyze in the provided text input field.

2. Analyze Button: Click the "submit" button to perform sentiment analysis on the entered text.

3. Results: The application will display the sentiment analysis results, showing the percentage likelihood of the text being positive or negative.

## File Structure

- `app.py`: The main Flask application file containing the routes and logic for sentiment analysis.
- `templates/`: Directory containing HTML templates for the web interface.
- `static/`: Directory for CSS files .

## Libraries and Frameworks Used

- Python
- Flask
- NLTK (Natural Language Toolkit)



#Level Text Processing step by step 

1.Preparing Stopwords: The code gets common words (like "the", "is", "and") that don’t carry strong feelings or context. It sets up a list of these words for English to filter them out later.

2.Getting User Input: When someone submits text, the system catches it. It makes sure all the text is in the same style by making it all lowercase.

3.Breaking Text into Words and Cleaning: The text gets divided into separate words. Then, it removes those common words (stopwords) from this bunch to focus on the important ones that carry more weight.

4.Figuring out Sentiment: It uses a tool called SentimentIntensityAnalyzer to understand the feelings behind the words. This tool gives scores for positivity, negativity, neutrality, and an overall score (ranging from -1 to 1).

5.Adjusting the Sentiment Score: The overall sentiment score is changed to a range that’s easier to understand (from -1 to 1 to a simpler 0 to 1) for better display and comprehension.

6.Showing the Results: The system gives back the final sentiment score along with the original text. This way, users can see how positive or negative the text is while looking at what they typed.
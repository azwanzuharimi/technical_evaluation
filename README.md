### Job Recommendation Model - Question 2a

2 type of files:
- Candidate details (30 separate JSON files)
- Job listing (single CSV file)

Objective:
- To provide a recommendation model to match each candidate with the most suitable job listed

Language/Technology:
- Python on Google Colab

Steps:
1. Read files placed in Google Drive using pandas. Loop each files and append all candidate information into single dataframe
2. Clean, transform, and tokenize text data for candidates and job listings
3. Get contextual similarity percentage for each candidate against all job listings using Spacy
4. Get top 3 most suitable jobs for each candidate
5. Output of a dataframe of each candidate with their most suitable position, and the similarity score


Challenges:
- Reading many deeply nested JSON files containing duplicated columns
- Stopwords (for tokenization) need to be custom made
- Transforming results into desired format output

Future Enhancements:
- Improve tokenization process and how the duplicated columns are transformed
- Try to use different NLP machine learning models to improve contextual similarity score

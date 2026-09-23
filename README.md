# Book Recommendation & Analysis System

This project is a book recommendation system that uses NLP and LLM-based techniques to recommend books based on what the user is looking for.

The main idea is to use the description and other information about books to find books that are similar to a user's query. I used embeddings and a vector database for semantic search, along with Hugging Face models for classification.

## What it does

* Recommends books based on user input
* Finds books using semantic similarity instead of only matching keywords
* Classifies books using zero-shot classification
* Uses embeddings to represent book descriptions
* Uses a vector database to retrieve similar books
* Provides a simple interface using Gradio

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Hugging Face
* LangChain
* [FAISS/Chroma]
* Gradio
* Matplotlib

## How it works

The basic workflow of the project is:

```text
Book Dataset
     ↓
Data Cleaning
     ↓
Book Description Processing
     ↓
Zero-Shot Classification
     ↓
Embeddings
     ↓
Vector Database
     ↓
Semantic Search
     ↓
Book Recommendations
     ↓
Gradio Interface
```

The book data is first cleaned and processed. I then use Hugging Face models for classification and generate embeddings from the book descriptions.

These embeddings are stored in a vector database. When a user enters a query, the system searches for books that are semantically similar to the query and uses the retrieved information to generate recommendations.

## Example

A user can enter something like:

```text
I want a psychological thriller with an unreliable narrator.
```

The system searches the book collection and returns books that are relevant to the query.

## Project Structure

```text
Book-Recommendation/
│
├── data/
├── notebooks/
├── src/
├── app.py
├── requirements.txt
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

## Run the project

```bash
python app.py
```

The Gradio interface will open locally and can be used to search for book recommendations.

## What I learned

Through this project, I worked with:

* NLP and text preprocessing
* Hugging Face models
* Text embeddings
* Semantic search
* Vector databases
* LangChain
* Building a simple interface with Gradio

## Future Improvements

Some things I would like to add in the future:

* Personalized recommendations based on user history
* Better recommendation evaluation
* Conversational recommendations
* Hybrid recommendation using user preferences and book similarity
* Deployment as a web application

## Author

Sandeep Ambarkar
B.Tech Electronics and Computer Engineering
Mahindra University

# Wikipedia Question-Answering Bot

## Overview
This project is a Question-Answering (QA) bot that takes a Wikipedia webpage as input and answers questions based on the content of the page. The bot leverages Natural Language Processing (NLP) models to extract relevant information and provide accurate responses to user queries.

## Features
- Accepts a Wikipedia webpage URL as input.
- Extracts and processes text content from the webpage.
- Uses a pre-trained NLP model (DistilBERT) for question-answering.
- Supports multiple top answers (configurable via `top_k`).
- Returns extracted answers along with the relevant context.

## Technologies Used
- Python
- Hugging Face Transformers (`distilbert/distilbert-base-cased-distilled-squad`)
- Sentence Transformers (`all-MiniLM-L6-v2` for embedding)
- BeautifulSoup (for web scraping Wikipedia content)
- PyTorch (for model inference)
- Jupyter Notebook

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/Wikipedia_QA_Bot.git
   cd Wikipedia_QA_Bot
   ```


## Usage
1. Open the Jupyter Notebook:
   ```sh
   jupyter notebook
   ```
2. Run the `Wikipedia_QA_bot.ipynb` notebook.
3. Provide a Wikipedia webpage URL.
4. Ask questions related to the content of the page.
5. The bot will return relevant answers with supporting context.

## Example
```python
question = "Who founded OpenAI?"
url = "https://en.wikipedia.org/wiki/OpenAI"
```
**Output:**
```
Answer: Sam Altman
Context: OpenAI, Inc. is an American artificial intelligence (AI) research organization founded in December 2015 and headquartered in San Francisco, California. 

It is OpenAI's first partnership with an educational institution.[74] In February, the U.S. 

Throughout 2024, roughly half of then-employed AI safety researchers left OpenAI, citing the company's prominent role in an industry-wide problem.[14][15]
 In December 2015, OpenAI was founded by Sam Altman, Elon Musk, Ilya Sutskever, Greg Brockman, Trevor Blackwell, Vicki Cheung, Andrej Karpathy, Durk Kingma, John Schulman, Pamela Vagata, and Wojciech Zaremba, with Sam Altman and Elon Musk as the co-chairs. 


```

## Configuration
- `top_k`: Adjust the number of top answers returned.
- `max_answer_length`: Set a limit for the maximum length of the answer.

## Future Improvements
- Expand to support multiple Wikipedia pages as context.
- Implement a web-based UI for user interaction.
- Improve answer ranking with advanced RAG techniques.
- Provide stable sentence answers.
- Change to a model that can answer questions more intelligently.
- Correct half answers.

## License
This project is licensed under the MIT License.

## Contributions
Contributions are welcome! Feel free to open issues and submit pull requests.

## Author
Your Name (@TeddyM1975)


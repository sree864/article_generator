# Information Retrieval Software for Article Generation

## Features
- Gathers data related to the topic from multiple sources
- Performs analysis and compilation of results
- Produces an article with proper citations and references

## Workflow
1. Define standard websites as trusted and verified sources
2. Scrape data from more websites
3. Extract information from these sources using an information extraction algorithm
4. Utilize natural language processing for text summarization
5. Generate a Word file with the outputs and references included

## Abstract
This project focuses on developing an information retrieval software that gathers data from multiple sources, performs analysis, and compiles the results into an article with proper citations and references. The software leverages web mining and natural language processing techniques to achieve this. The resulting article provides a concise summary of the topic by extracting relevant information from trusted websites and utilizing text summarization methods. The software also generates a Word file containing the summarized output and references.

## Keywords
Web Mining, Bing, Natural Language Processing

## Methodology
The software follows the following procedure:

### A. Getting Inputs
- User provides the query and the number of websites to process.

### B. Get the Top n Websites
- Bing Search API is used to retrieve the top n websites relevant to the query.

### C. Scraping
- Each website's relevant data is obtained using domain-specific scrapers.

### D. Data Cleaning
- HTML tags, special characters, and new line characters are removed from the data.

### E. Text Summarization
- TF-IDF (Term Frequency - Inverse Document Frequency) approach is used for extractive summarization of the text.
- Cosine similarity is computed within two vectors.
- The top 10 sentences are selected and combined to form a summary.

### F. Generate Document
- The query is added as the title, the generated summary as the content, and the URLs as references.
- The Python `docx` library is used to convert the output into a Word document, which is then saved.

## How to Make It Work
1. Download the `article_generator.py` file from the repository.
2. Open the `article_generator.py` file in a Python editor or IDE.
3. Locate the "Input Section" in the code.
4. Replace the `query` variable with your desired keyword or topic.
5. Adjust the `n` variable to specify the number of websites to process.
6. Save the `article_generator.py` file after making the changes.
7. Run the `article_generator.py` file in the Python environment.
8. After execution, the software will generate the article in a Word document.

## Architecture
![Architecture](architecture.png)

## Results
![Output File](output.png)

## Future Scope
The project can be enhanced by:
- Including better coverage of relevant data
- Implementing more advanced summarization techniques
- Allowing users to choose their preferred language
- Generating documents in both the original language and English translation

## Conclusion
The developed information retrieval software represents a significant advancement in automated content creation. By employing advanced Python language and NLP tools, the software can gather, analyze, and summarize information from multiple sources with accuracy and efficiency. Its customizable options make it a valuable tool for various professionals, while its web scraping and natural language processing techniques ensure comprehensive and reliable summaries. Overall, the software holds great potential for streamlining content creation processes and finding applications in a wide range of fields.

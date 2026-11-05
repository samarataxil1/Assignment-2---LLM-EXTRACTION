This project built a Python workflow that pulled 8-K filings from SEC EDGAR for eight tech companies, converted them to text, 
and used a locally run Llama 3.2 model (through Ollama) to extract newly announced products into a CSV with company, ticker, 
filing date, product name, and a short description. The first results had many false positives, such as stock and debt 
securities, so the prompt and keyword filters were refined, which cut ten candidates down to one that still needs to be checked 
against its source filing. The main limitations are that only 20 filings were analyzed and only the first 12,000 characters of 
each were read, 
so the project shows the value of prompt refinement, filtering, and source validation when using LLMs on financial documents.

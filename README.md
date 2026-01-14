# Bootcamp :- iCOR-Automated-Environmental-Legal-Register-Builder
iCOR is a Legal Tech pipeline that automates the creation of environmental legal registers. It uses BeautifulSoup to scrape data from legislation.gov.uk and Azure OpenAI (GPT-4) to extract structured insights. The system features optimized token management to reduce costs and converts complex legal text into actionable JSON data.

# iCOR: Intelligent Compliance & Obligation Register

iCOR is an automated tool designed to help environmental managers bridge the gap between raw UK legislation and actionable legal registers. By combining web scraping with Large Language Models (LLMs), it reduces the manual effort required to track regulatory changes.

## 🔄 The Pipeline
1. **Extraction:** Scrapes legal text and metadata from `legislation.gov.uk` using BeautifulSoup.
2. **Structure:** Stores raw data in a version-controlled Pandas DataFrame.
3. **Summarization:** Leverages GPT-4 to extract key changes, mandatory obligations, and dates.
4. **Integration:** Outputs structured JSON for easy integration into compliance dashboards.



## 🛠 Features & Optimizations
- **Token-Efficient Prompting:** Custom system prompts designed to minimize Azure OpenAI costs while maximizing extraction accuracy.
- **JSON Formatting:** Forced schema output for automated downstream processing.
- **Selective Scraping:** Uses `find_all()` logic to isolate legal bodies and remove website "noise" (headers/footers), saving ~30% on token usage.

## 📂 Project Structure
- **01_Technical_Report:** Documentation on the legal register building process and iCOR logic.
- **02_Source_Codes:** Jupyter Notebooks for web scraping and OpenAI integration.
- **03_System_Images:** Visual representations of the data flow and resulting register.
- **04_Schematic_Diagrams:** Logical flowcharts of the scraping-to-summarization process.



## 🚀 Future Improvements
- [ ] Integration with a vector database (RAG) for multi-document querying.
- [ ] Automated email alerts for new legislation matching specific keywords.
- [ ] Comparison tool to highlight line-by-line changes between original and updated acts.

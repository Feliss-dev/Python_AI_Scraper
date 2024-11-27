🌐 AI Web Scraper with Parsing Capabilities
This project is an AI-powered web scraper built with Streamlit, Selenium, BeautifulSoup, and LangChain. It extracts content from web pages and leverages AI to retrieve specific information based on your custom descriptions.

✨ Features
🕸️ Web Scraping: Extract HTML content from any given website.
🧹 Content Cleaning: Automatically clean the content by removing unnecessary scripts, styles, and blank lines.
🤖 AI Parsing: Use AI to extract specific data based on user-provided instructions.
🖥️ Interactive UI: Streamlit offers a modern and easy-to-use interface.
📋 Prerequisites
Python (>= 3.8) installed on your system.

Install the required libraries:


pip install streamlit selenium beautifulsoup4 lxml html5lib langchain python-dotenv
Chrome WebDriver:

Download the correct version for your Chrome browser here.
Add the WebDriver to your PATH.
Superproxy Credentials:

Update the AUTH constant in the scrape_website function with your Superproxy credentials.
AI Model:

Configure the Ollama LLM for LangChain usage. Refer to Ollama's official documentation.
🚀 Setup Guide
1️⃣ Clone the Repository

git clone <repository-url>
cd <repository-folder>
2️⃣ Configure Environment Variables
Create a .env file to securely store sensitive credentials:


SUPERPROXY_AUTH=brd-customer-hl_527308d8-zone-ai_scraper:i0ny949pw63x
3️⃣ Install Dependencies

pip install -r requirements.txt
4️⃣ Run the Application

streamlit run app.py
💻 How to Use
Launch the App:

Open your browser at http://localhost:8501.
Scrape a Website:

🔗 Enter the URL of the website in the input field.
🖱️ Click the Scrape Site button.
🛠️ View and inspect the cleaned DOM content in the View DOM Element section.
Parse Content:

📝 Enter a description of what you want to extract in the input field.
💡 Click Parse DOM to process and extract the desired information.
📄 Results will appear below the input box.
📁 Project Structure

├── app.py                     # Main Streamlit application
├── scrape.py                  # Web scraping utilities (Selenium, BeautifulSoup)
├── parse.py                   # AI-based parsing (LangChain, Ollama)
├── requirements.txt           # Python dependencies
└── .env                       # Environment variables (not included in the repo)
🛠️ Troubleshooting
❌ Connection Issues:
Ensure your Superproxy credentials are correct and the proxy server is reachable.
⚠️ Model Invocation Errors:
Verify that the Ollama LLM is configured properly and accessible.
🛑 WebDriver Errors:
Ensure your Chrome WebDriver matches your Chrome browser version.
📖 Example Use Case
Input URL: https://example.com
Parsing Instruction: "Extract all headings and paragraphs related to technology."
Output:

Heading: The Future of Technology
Paragraph: Technology is rapidly evolving, with AI leading the charge...
🤝 Contributing
🌟 Fork this repository.
✏️ Create a feature branch.
📬 Submit a pull request.
🛡️ License
This project is open-source and licensed under the MIT License.

🎉 Happy Scraping! Let us know if you need help extending or customizing this project. 😊

Made with ❤️ by AI and Open-Source Tools

Azure Text Analytics – Review Analysis Project

This project demonstrates how to use Microsoft Azure AI Text Analytics to automatically analyze text-based customer reviews.
It performs:

🔤 Language Detection

😊 Sentiment Analysis

🏷️ Key Phrase Extraction

🧩 Entity Recognition

🔗 Linked Entity Recognition

All review text files stored in the reviews/ folder are processed automatically

project-folder/
│-- reviews/                  # Folder containing text files for analysis
│-- text-analysis.py          # Main Python script
│-- .env                      # Your secrets (NOT uploaded to GitHub)
│-- .env.example              # Example env variables (uploaded to GitHub)
│-- requirements.txt
│-- README.md
🔧 Tech Stack

Python

Azure Text Analytics (Azure Cognitive Services)

python-dotenv

✅ Prerequisites

Python 3.8+

Azure AI (Cognitive Services) Resource

Endpoint

Key

Create a reviews/ folder and add .txt files inside.

⚙️ Installation
1. Clone the repository:
git clone <your-repo-url>
cd <your-project-folder>

2. Install dependencies:
pip install -r requirements.txt

🔐 Setup Environment Variables

Create a .env file in the project root:

AI_SERVICE_ENDPOINT=your_endpoint_here
AI_SERVICE_KEY=your_key_here


Also create .env.example and upload that to GitHub:

AI_SERVICE_ENDPOINT=
AI_SERVICE_KEY=


⚠️ Never upload your .env file.

▶️ Run the Project

Simply run:

python text-analysis.py


The script will:

Loop through all files inside reviews/

Print language

Print sentiment

Extract key phrases

Extract entities

Extract linked entities

📌 Example Output
-------------
review1.txt
The product is amazing and delivery was fast!

Language: English
Sentiment: positive

Key Phrases:
    product
    delivery

Entities:
    product (Product)

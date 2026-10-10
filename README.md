# LinkedIn-Post-Caption-Generator
A GenAI-powered LinkedIn post generator that analyzes past posts and uses few-shot prompting to generate new content based on topic, language, length, and writing style.
# GenAI LinkedIn Post Generator 🚀

A Generative AI application that generates LinkedIn posts using examples from previously written posts. Users can select a topic, language, and post length to generate content inspired by the writing style of the available examples.

## ✨ Features

* **Topic Selection:** Choose from topics extracted from existing posts.
* **Custom Length:** Generate short, medium, or long posts.
* **Language Options:** Select English or Hinglish.
* **Few-Shot Prompting:** Use relevant examples to guide the language model's output.
* **Interactive Interface:** Generate posts through a Streamlit web application.

## 🛠️ Tech Stack

* Python
* Pandas
* LangChain
* Groq API
* Large Language Models (LLMs)
* Streamlit

## ⚙️ How It Works

1. **Data Processing:** Load historical LinkedIn posts and extract metadata, including topic tags, language, and line count.
2. **Post Filtering:** Retrieve relevant examples based on the selected topic, language, and length.
3. **Prompt Construction:** Add the retrieved examples to a prompt using few-shot prompting.
4. **Content Generation:** Send the prompt to an LLM through the Groq API.
5. **Display Results:** Show the generated LinkedIn post in the Streamlit interface.

## 📁 Project Structure

```text
genai-linkedin-post-generator/
├── data/
│   ├── raw_posts.json
│   └── processed_posts.json
├── app.py
├── few_shot.py
├── llm_helper.py
├── post_generator.py
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd genai-linkedin-post-generator
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure your API key

Create a `.env` file in the project root:

```text
GROQ_API_KEY=your_groq_api_key
```

Get an API key from [Groq Console](https://console.groq.com/keys).

Never commit your API key to GitHub.

### 5. Prepare the dataset

Ensure the required post datasets are available in the `data/` directory and that `processed_posts.json` contains the fields expected by the application.

### 6. Run the application

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal.

## 📚 Key Concepts

* Generative AI
* Large Language Models
* Prompt Engineering
* Few-Shot Prompting
* Data Preprocessing
* API Integration
* Interactive AI Applications



## 🔮 Future Improvements

* Add more language options.
* Improve topic classification and example retrieval.
* Allow users to provide their own post history.
* Add controls for tone, audience, and writing preferences.
* Evaluate generated posts for relevance and writing-style consistency.



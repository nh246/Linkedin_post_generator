# LinkedIn Post Generator AI

An intelligent AI-powered tool that generates engaging, professional LinkedIn posts on any topic in any language using Google's Gemini 2.0 Flash model and LangChain.

## 📋 Features

- **AI-Powered Content Generation**: Uses Google's Gemini 2.0 Flash model for high-quality post creation
- **Multi-Language Support**: Generate LinkedIn posts in any language
- **Professional Structure**: Automatically creates well-structured posts with:
  - Attention-grabbing hooks
  - Key insights and tips
  - Strong calls-to-action
  - Relevant emojis and hashtags
- **Fallback Mechanism**: Includes error handling with direct Google API fallback
- **Interactive Loop**: Continuously generate posts without restarting the program
- **LangChain Integration**: Leverages LangChain for prompt management and chain orchestration

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- Google API Key (for Gemini model access)
- pip (Python package manager)

### Installation

1. **Clone or download this repository**

2. **Install required packages**:
```bash
pip install langchain langchain-google-genai google-generativeai
```

3. **Set up your Google API Key**:
   - Get your API key from [Google AI Studio](https://ai.google.dev/)
   - Update the `GOOGLE_API_KEY` in the notebook or set it as an environment variable

### Configuration

In the notebook, locate the API Key section and update:

```python
os.environ["GOOGLE_API_KEY"] = "YOUR_API_KEY_HERE"
```

## 💻 Usage

1. **Run the Jupyter Notebook**:
   - Open `linkedinpost_ai_nazmul_hossain.ipynb` in Jupyter Notebook or JupyterLab
   - Install the required packages (first cell)
   - Execute all cells sequentially

2. **Generate Posts**:
   - When prompted, enter a topic (e.g., "Artificial Intelligence in Business")
   - Enter the desired language (e.g., "English", "French", "Spanish")
   - The AI will generate a professional LinkedIn post

3. **Continuous Generation**:
   - The script runs in a loop for continuous post generation
   - Type `exit` or `quit` to exit the program
   - Generate unlimited posts without restarting

### Example

```
Enter topic (or type 'exit' to quit): Digital Transformation
Enter language (or type 'exit' to quit): English

⚙️ Running... please wait...

========================================================================
        GENERATED LINKEDIN POST (AI Agent Output)
========================================================================
[Generated post content here]
========================================================================
✓ Success! Topic: Digital Transformation | Language: English
```

## 🏗️ Project Structure

```
Linkedin_post_generator/
├── linkedinpost_ai_nazmul_hossain.ipynb  # Main Jupyter notebook
└── README.md                               # This file
```

## 🔧 Technical Details

### Libraries Used

- **LangChain**: Prompt management and LLM chain orchestration
- **Google Generative AI**: Access to Gemini 2.0 Flash model
- **LangChain Google GenAI**: LangChain integration for Google's generative models

### Model Configuration

- **Model**: Gemini 2.0 Flash
- **Temperature**: 0.7 (balanced creativity)
- **Max Output Tokens**: 600 (sufficient for LinkedIn posts)

### Prompt Structure

The AI follows a structured prompt that ensures:
- Attention-grabbing opening
- 1-2 key insights or actionable tips
- Professional tone with 1-2 emojis
- 3-4 relevant hashtags
- Effective call-to-action
- Output is 2-4 paragraphs

## ⚠️ Error Handling

The application includes robust error handling:
- **Primary Method**: Uses LangChain for reliable output handling
- **Fallback Mechanism**: Automatically switches to direct Google API if LangChain encounters issues
- **Validation**: Checks for empty or insufficient responses

## 📝 Notes

- Keep your API key secure and never commit it to version control
- Each generation uses API credits; monitor your usage on Google AI Studio
- The temperature setting (0.7) provides a good balance between creativity and consistency
- Posts are optimized for LinkedIn's character limits and engagement algorithms

## 🎬 Demo

A demonstration video of this project is available on [Google Drive](https://drive.google.com/file/d/1BoK2WneCtpMgaMMC4vCp-CEP_0qr5Ar8/view?usp=sharing)

## 👨‍💻 Author

**Nazmul Hossain**

## 📄 License

This project is open-source. Feel free to use and modify it for your needs.

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest improvements
- Submit pull requests

## 🙋 FAQ

**Q: Can I generate posts in languages other than English?**
- A: Yes! The tool supports any language. Simply specify your desired language when prompted.

**Q: What happens if the API fails?**
- A: The application has a fallback mechanism that uses the direct Google API if LangChain encounters issues.

**Q: Can I modify the post structure?**
- A: Yes! You can edit the `PromptTemplate` in the notebook to customize the output format.

**Q: Is there a limit to how many posts I can generate?**
- A: There's no limit in the tool itself, but your Google API usage limits may apply based on your plan.

## 🔗 Useful Resources

- [Google Generative AI Documentation](https://ai.google.dev/docs)
- [LangChain Documentation](https://docs.langchain.com)
- [Jupyter Notebook Documentation](https://jupyter.org/documentation)

---

**Happy Generating!** 🚀

# 📚 Semantic Book Recommender

An AI-powered book recommendation system that uses semantic search and emotion analysis to help users discover their next favorite book.

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-Hugging_Face-yellow?style=for-the-badge)](https://huggingface.co/spaces/EdwardConstantine/book-recommender)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)](https://github.com/EmonKarmaker/book_reccomender-2.0)
[![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python)](https://www.python.org/)
[![Gradio](https://img.shields.io/badge/Gradio-3.43-FF6B35?style=for-the-badge&logo=gradio)](https://gradio.app/)

---

## 🎯 Key Features

- **🔍 Semantic Search:** Uses sentence transformers and vector embeddings to understand book descriptions beyond keyword matching
- **🎭 Emotion-Based Filtering:** Filter recommendations by emotional tone (Happy, Sad, Suspenseful, Angry, Surprising)
- **📂 Category-Based Search:** Browse books across multiple genres and categories
- **🖼️ Visual Gallery:** Beautiful book cover displays with detailed descriptions
- **⚡ Real-Time Recommendations:** Instant results powered by ChromaDB vector database

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **LangChain** | Framework for building LLM applications |
| **ChromaDB** | Vector database for semantic similarity search |
| **Sentence Transformers** | Embedding model (`all-MiniLM-L6-v2`) |
| **Gradio** | Interactive web interface |
| **Pandas & NumPy** | Data manipulation and processing |
| **HuggingFace** | Model hosting and embeddings |

---

## 🚀 Live Demo

Try it out here: **[Book Recommender App](https://huggingface.co/spaces/EdwardConstantine/book-recommender)**

---

## 📸 Screenshots

![Book Recommender Interface](assets/Screenshot%202025-11-23%20212935.png)

---

## 🧠 How It Works

1. **Document Processing:** Book descriptions are loaded and split into chunks
2. **Embedding Generation:** Text is converted to 384-dimensional vectors using sentence transformers
3. **Vector Storage:** Embeddings are stored in ChromaDB for fast similarity search
4. **Semantic Matching:** User queries are embedded and matched against the book database
5. **Emotion Filtering:** Results are sorted by emotion scores (joy, fear, anger, sadness, surprise)
6. **Visual Display:** Top recommendations are displayed with cover images and descriptions

---

## 📦 Installation & Setup

### Prerequisites
- Python 3.11+
- pip package manager

### Local Setup

```bash
# Clone the repository
git clone https://github.com/EmonKarmaker/book_reccomender-2.0.git
cd book_reccomender-2.0

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Create .env file with your API keys
echo "GROQ_API_KEY=your_groq_key" >> .env
echo "HUGGINGFACEHUB_API_TOKEN=your_hf_token" >> .env

# Run the application
python app.py
```

The app will be available at `http://localhost:7860`

---

## 📂 Project Structure

```
book_reccomender-2.0/
├── app.py                      # Main Gradio application
├── requirements.txt            # Python dependencies
├── books_with_emotions.csv     # Book dataset with emotion scores
├── tagged_description.txt      # Preprocessed book descriptions
├── cover-not-found.jpg         # Fallback cover image
├── chroma_db/                  # Vector database storage
├── README.md                   # Project documentation
└── assets/                     # Screenshots and images
```

---

## 🎨 Dataset

The book dataset includes:
- **Book metadata:** Title, authors, ISBN, categories
- **Descriptions:** Detailed book summaries
- **Emotion scores:** Joy, surprise, anger, fear, sadness
- **Cover images:** High-resolution thumbnails

---

## 🔮 Future Enhancements

- [ ] Add user authentication and reading history
- [ ] Implement collaborative filtering
- [ ] Support for multilingual book recommendations
- [ ] Integration with Goodreads API
- [ ] Reading list management
- [ ] Book ratings and reviews

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Emon Karmaker**

- GitHub: [@EmonKarmaker](https://github.com/EmonKarmaker)
- LinkedIn: [Your LinkedIn Profile]
- Portfolio: [Your Portfolio Website]

---

## 🙏 Acknowledgments

- Sentence Transformers for the embedding model
- LangChain for the RAG framework
- Gradio for the beautiful UI
- HuggingFace for hosting and model infrastructure

---

## 📧 Contact

For questions or feedback, please open an issue or reach out via [LinkedIn](your-linkedin-url).

---

<div align="center">
  Made with ❤️ and 🤖 AI
</div>

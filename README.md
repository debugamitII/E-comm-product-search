# E-comm-product-search
E-commerce Product search using AgenticAI
Here's a well-structured **README.md** for your Streamlit-based E-commerce Product Search Assistant project:

---

# 🛒 E-commerce Product Search Assistant

This is a **Streamlit web application** that uses **LangChain**, **Pydantic**, and **Groq LLM** to return structured JSON data about a product, such as its name, brand, specifications, price, and purchase link. It acts as a smart ecommerce assistant capable of answering natural language product queries.

---

## 🚀 Features

* 🌐 Natural language product queries
* 🤖 Powered by `Groq` LLM with `LangChain`
* ✅ Structured JSON response using `Pydantic`
* 🎨 Responsive UI with dark mode support
* 🔗 Direct product link and basic details display

---

## 🧰 Tech Stack

| Tool/Library                | Purpose                           |
| --------------------------- | --------------------------------- |
| Python                      | Core programming language         |
| Streamlit                   | Frontend UI                       |
| LangChain                   | Prompt and model chaining         |
| Groq (via `langchain_groq`) | LLM for product generation        |
| Pydantic                    | Enforces structured output (JSON) |
| dotenv                      | Environment variable management   |

---

## 📦 Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/ecommerce-assistant.git
cd ecommerce-assistant

# 2. Create and activate a virtual environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the root directory with the following content:

```env
OPENAI_API_KEY=your-openai-api-key
GROQ_API_KEY=your-groq-api-key
LANGCHAIN_API_KEY=your-langchain-api-key
LANGCHAIN_PROJECT=your-project-name
```

---

## 🖥️ How to Run

```bash
streamlit run app.py
```

This will launch the app in your browser at `http://localhost:8501`.

---

## ✨ Example Output

**Query:**

```
Find best mobile phone deal
```

**Output (Structured):**

```json
{
  "product_name": "iPhone 15 Pro Max",
  "brand": "Apple",
  "model": "A3104",
  "specs": "6.7-inch display, A17 Pro chip, 256GB storage",
  "price": "$1199",
  "link": "https://example.com/iphone15"
}
```

---

## 📁 Project Structure

```
.
├── app.py              # Streamlit app code
├── .env                # Environment variables (not committed)
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

---

## ✅ TODO / Improvements

* 🔍 Add multi-product comparison
* 🗃️ Add caching or memory for previous searches
* 🌐 Integrate real-time ecommerce API (Amazon, Flipkart, etc.)
* 📱 Make mobile-friendly layout

---

## 📄 License

This project is licensed under the MIT License.

---

Let me know if you want to auto-generate `requirements.txt` or deploy this to Streamlit Cloud / HuggingFace Spaces.


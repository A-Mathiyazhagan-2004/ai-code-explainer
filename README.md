
# AI Code Explainer with Complexity Analysis and Optimization Suggestions

This project demonstrates the use of Generative AI (via Google Gemini) to explain code, analyze its time and space complexity, suggest optimizations, and even compare two code snippets. It features a colorful console UI and supports saving explanations to downloadable files.

---

## 💻 Features
✅ Explain code in **simple English** (line-by-line or summary).  
✅ **Analyze time and space complexity** of the code.  
✅ **Suggest optimizations** and point out potential bad practices.  
✅ **Compare two code snippets** and explain which is better.  
✅ Colorful, user-friendly console interface.  
✅ Save explanations as `.txt` or `.md` files and download them.

---

## 🚀 How to Run

1️⃣ Clone the repository:
```bash
git clone https://github.com/A-Mathiyazhagan-2004/ai-code-explainer
cd ai-code-explainer
```

2️⃣ Open the notebook in Google Colab.

3️⃣ **Install dependencies** (already included in the notebook):
```python
!pip install -q google-generativeai
```

4️⃣ **Provide your Gemini API key**:
In the notebook, replace:
```python
genai.configure(api_key="YOUR_API_KEY")
```
with:
```python
genai.configure(api_key="PASTE_YOUR_ACTUAL_API_KEY_HERE")
```

⚠️ **Recommended:**  
Instead of hardcoding the API key, you can store it securely like this in Colab:
```python
import os
api_key = os.getenv("GEMINI_API_KEY")
genai.configure(api_key=api_key)
```
And set your environment variable in Colab (in a hidden cell):
```python
os.environ["GEMINI_API_KEY"] = "PASTE_YOUR_ACTUAL_API_KEY_HERE"
```

5️⃣ Run the notebook cells and follow the on-screen instructions to input code, choose options, and generate explanations!

---

## 📝 Example Input Flow
```
👉 Please enter your main code (type END on a new line to finish):
def add(a, b):
    return a + b
END

Do you want to input another code to compare? (yes/no): no
Enter programming language (default Python): Python
Choose explanation type (line-by-line / summary, default line-by-line): summary
Save as txt or md? (default txt): txt
Do you want to explain another code snippet? (yes/no): no
```

---

## 📂 Outputs
- Explanation files will be saved and downloadable directly from Colab (e.g., `ai_code_explanation_1.txt`).

---

## ⚠ Important Notes
- Never commit your API key to GitHub.
- This project uses the **Gemini 1.5 Flash model**. You may switch to `gemini-1.5-pro` or others depending on your quota.
- The project runs best in Google Colab due to interactive input handling.

---

## 🔮 Future Improvements
- Add Streamlit or Flask web interface
- Visualize complexity (graphs, charts)
- Support for more languages beyond Python/C/Java/C++

---

## ✨ Credits
Made with Google Gemini + Python + Colab.

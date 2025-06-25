# 🕵️‍♂️ Fake Review Detector with BERT + LIME

This is a web-based Fake Review Detector built using **Streamlit**. It uses a fine-tuned **BERT** model to classify whether a review is **Original** or **Computer-Generated**. For interpretability, it integrates **LIME (Local Interpretable Model-agnostic Explanations)** to visualize what parts of the text influenced the prediction.

---

## 🚀 Features

- 🔍 **Real-Time Review Classification**: Detect whether a single review is genuine or generated.
- 🧠 **BERT-based Model**: Uses `lol3445/bert-email-cap-classifier` for high-accuracy classification.
- 💬 **Confidence Score & Prediction Label**: Outputs prediction along with model confidence.
- ✅ **Feedback Collection**: Users can mark predictions as correct/incorrect for improvement tracking.
- 🔍 **LIME Explanation**: See which words most influenced the model's decision (with a color-coded breakdown).
- 📁 **CSV Upload Support**: Bulk detection from `.csv` files with a `text` column.
- ⬇️ **Downloadable Results**: Export results in CSV format for analysis.

---

## 🧠 Model

- **Model**: BERT fine-tuned on email/review classification.
- **Source**: [`lol3445/bert-email-cap-classifier`](https://huggingface.co/lol3445/bert-email-cap-classifier)
- **Classes**:
  - `Original` — Human-written text
  - `Computer-Generated` — AI/Script-written text

---

## 📦 Installation

1. **Clone this repo** (if using locally):

```bash
git clone https://github.com/yourusername/fake-review-detector.git
cd fake-review-detector
````

2. **Install dependencies**:

```bash
pip install -r requirements.txt
```

3. **Run the app**:

```bash
streamlit run app.py
```

> Or run it directly in Google Colab (you'll need to convert it to `.ipynb`).

---

## 📁 File Structure

```
.
├── app.py                 # Main Streamlit app
├── feedback_log.txt       # Stores user feedback (optional)
├── requirements.txt       # Required Python packages
└── README.md
```

---

## 🔍 How to Use

### 🔹 Single Text Prediction

1. Enter any review text in the input box.
2. Click **Classify**.
3. View the prediction label and confidence.
4. Optionally, provide feedback on correctness.

### 🔹 Explanation (LIME)

* Check **"Show Explanation (LIME)"** to visualize how words influence prediction.
* Requires a minimum number of words (default: 3).

### 🔹 Bulk Detection

1. Upload a `.csv` file containing a column named `text`.
2. View classification results instantly.
3. Download processed results in `.csv` format.

---

## 📈 Roadmap

* ✅ Model loading and classification
* ✅ LIME interpretability
* ✅ CSV upload and batch classification
* 🔜 Training on custom datasets
* 🔜 User login + feedback tracking via database
* 🔜 Deploy to Hugging Face or Streamlit Cloud

---

## 📌 Notes

* Feedback is saved in `feedback_log.txt`. You can modify it to log in a database for production.
* Confidence is visualized via progress bar for better UX.

---

## 🙋‍♂️ Author

**Rahul Kodunga**
🎓 B.Tech (CSE), Dehradun
📫 [rahulkodunga@gmail.com](mailto:rahulkodunga@gmail.com)
💡 Interested in AI, NLP, and building useful ML tools

---

## 📃 License

MIT License. See `LICENSE` file for details.

---

> “Detecting fake content with real intelligence.”

```

---

Would you like me to also generate the `requirements.txt` for this project?
```

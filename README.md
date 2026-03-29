# 💄 Cosmetics Ingredient Analysis & Recommendation System

A content-based recommendation system that analyzes chemical ingredients of 1,472 Sephora cosmetic products using t-SNE dimensionality reduction and interactive Bokeh visualization.

---

## 📁 Folder Structure

Make sure your project folder looks exactly like this before running:

```
project/
│
├── datasets/
│   └── cosmetics.csv
│
└── notebook.ipynb
```

> ⚠️ The `datasets/` folder **must be inside the same directory** as `notebook.ipynb`. If the CSV is in a different location, the file path in the code will not work.

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install Required Libraries

```bash
pip install pandas numpy scikit-learn bokeh
```

### 3. Verify Folder Structure

Make sure `cosmetics.csv` is inside a folder named `datasets/`:

```bash
# On Windows
mkdir datasets
move cosmetics.csv datasets\

# On Mac/Linux
mkdir datasets
mv cosmetics.csv datasets/
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Then open `notebook.ipynb` in your browser.

---

## ▶️ Running the Project

Run each cell in order from top to bottom — **do not skip cells** as each task builds on the previous one.

| Task | Description |
|------|-------------|
| Task 1 | Import libraries and load dataset |
| Task 2 | Filter for moisturizers and dry skin |
| Task 3 | Tokenize ingredients |
| Task 4 | Initialize Document-Term Matrix |
| Task 5 | Create one-hot encoder function |
| Task 6 | Fill the matrix |
| Task 7 | Dimension reduction with t-SNE |
| Task 8 | Create Bokeh scatter plot |
| Task 9 | Add hover tooltips |
| Task 10 | Display the plot |
| Task 11 | Compare two similar products |

---

## 🛠️ Tech Stack

- **Python** — core language
- **pandas & NumPy** — data manipulation
- **scikit-learn** — t-SNE dimensionality reduction
- **Bokeh** — interactive visualization

---

## 🚀 Expected Output

An interactive scatter plot where:
- Each dot represents a cosmetic product
- Products with **similar ingredients cluster together**
- Hovering over a dot shows **Name, Brand, Price, and Rank**

---

## ⚠️ Common Issues

**Plot not showing?**
Make sure `output_notebook()` is called before `show(plot)`.

**File not found error?**
Check that `cosmetics.csv` is inside the `datasets/` folder, not in the root directory.

**Bokeh deprecation warning?**
Use `plot.scatter()` instead of `plot.circle()` if you're on Bokeh 3.4.0+.

**Suppress all warnings:**
```python
import warnings
warnings.filterwarnings('ignore')
```

---

## 📊 Dataset

- **Source:** Sephora product listings
- **Size:** 1,472 products × 11 columns
- **Key columns:** `Label`, `Brand`, `Name`, `Price`, `Rank`, `Ingredients`, skin type flags

---

## 👤 Author

**Kushagra Singh**  
Data Science Intern | Portfolio Project

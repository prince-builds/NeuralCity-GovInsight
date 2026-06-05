# NeuralCity-GovInsight

AI-powered natural language analytics system for Government Crop Production Data.

Users can ask questions in plain English and receive data-driven answers with visualizations.

---

## Live Demo

🚀 Gradio App:

https://a7f495650d637f3aa6.gradio.live/

> Note: Gradio public links may expire after a limited time. If the link is inactive, follow the setup instructions below to run the project locally.

---

## Important: Groq API Setup

This project requires a Groq API key.

Create a free API key:

https://console.groq.com/keys

Replace:

```python
client = Groq(
    api_key="YOUR_GROQ_API_KEY"
)
```

with your own API key.

OR

Use an environment variable:

```python
import os
from groq import Groq

client = Groq(
    api_key=os.getenv("GROQ_API_KEY")
)
```

---

## Quick Start

### 1. Install Dependencies

```bash
pip install groq gradio pandas matplotlib requests
```

### 2. Open Notebook

```bash
NeuralCity_GovInsight.ipynb
```

### 3. Add Your Groq API Key

Follow the instructions above.

### 4. Run All Cells

Run all notebook cells from top to bottom.

### 5. Launch Gradio App

A public Gradio URL will be generated.

---

## Features

* Natural language question understanding using Groq LLM
* Query-to-JSON conversion
* Crop production analytics
* Interactive charts
* Government crop dataset exploration
* Out-of-scope question detection

---

## Supported Queries

### Top State

Examples:

* Which state produced the most rice in 2010?
* Which state produced the most wheat in 2012?

---

### Top N States

Examples:

* Top 5 rice producing states in 2010
* Top 10 wheat producing states in 2013

---

### Production Trend

Examples:

* Show rice production trend in Punjab
* Show wheat production trend in Haryana

---

### Compare States

Examples:

* Compare rice production in Punjab and Haryana in 2010
* Compare wheat production in Uttar Pradesh and Punjab in 2012

---

### Summary

Examples:

* Give summary of rice production in Punjab in 2010
* Give summary of wheat production in Haryana in 2012

---

### Out of Scope Detection

Examples:

* What is India's GDP?
* Who is the Prime Minister of India?
* Tell me about IPL

The system correctly identifies these questions as outside the crop production dataset.

---

## Dataset

Dataset used:

`crop_production.csv`

Columns:

* State_Name
* District_Name
* Crop_Year
* Season
* Crop
* Area
* Production

---

## Tech Stack

* Python
* Pandas
* Matplotlib
* Groq API
* Llama 3.3 70B Versatile
* Gradio

---

## Example Test Questions

```text
Which state produced the most rice in 2010?

Which state produced the most wheat in 2012?

Top 5 rice producing states in 2010

Top 5 wheat producing states in 2012

Show rice production trend in Punjab

Show wheat production trend in Punjab

Compare rice production in Punjab and Haryana in 2010

Compare wheat production in Punjab and Haryana in 2012

Give summary of rice production in Punjab in 2010

Give summary of wheat production in Haryana in 2012

What is India's GDP?

Who is the Prime Minister of India?
```

---

## Screenshots

### Application Demo

See the screenshots inside the `screenshots` folder for sample outputs and visualizations.

---

## Future Improvements

* Additional agricultural datasets
* Multi-crop comparison
* District-level analytics
* Export reports to PDF
* Advanced dashboards
* Multi-year crop forecasting

---

## Author

Prince

B.Tech AI

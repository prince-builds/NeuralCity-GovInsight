# NeuralCity-GovInsight


AI-powered natural language analytics system for Government Crop Production Data.

Users can ask questions in plain English and receive data-driven answers with visualizations.

---

## Features

- Natural language question understanding using Groq LLM
- Query-to-JSON conversion
- Crop production analytics
- Interactive charts
- Government crop dataset exploration
- Out-of-scope question detection

---

## Supported Queries

### Top State

Examples:

- Which state produced the most rice in 2010?
- Which state produced the most wheat in 2012?

---

### Top N States

Examples:

- Top 5 rice producing states in 2010
- Top 10 wheat producing states in 2013

---

### Production Trend

Examples:

- Show rice production trend in Punjab
- Show wheat production trend in Haryana

---

### Compare States

Examples:

- Compare rice production in Punjab and Haryana in 2010
- Compare wheat production in Uttar Pradesh and Punjab in 2012

---

### Summary

Examples:

- Give summary of rice production in Punjab in 2010
- Give summary of wheat production in Haryana in 2012

---

### Out of Scope Detection

Examples:

- What is India's GDP?
- Who is the Prime Minister of India?
- Tell me about IPL

The system correctly identifies these questions as outside the crop production dataset.

---

## Dataset

Dataset used:

`crop_production.csv`

Columns:

- State_Name
- District_Name
- Crop_Year
- Season
- Crop
- Area
- Production

---

## Tech Stack

- Python
- Pandas
- Matplotlib
- Groq API
- Llama 3.3 70B Versatile
- Gradio

---

## Installation

Install dependencies:

```bash
pip install groq gradio pandas matplotlib requests
```

---

## Groq API Setup

Create a Groq API key:

https://console.groq.com/keys

Replace:

```python
client = Groq(
    api_key="YOUR_GROQ_API_KEY"
)
```

with your own key.

OR

Set an environment variable:

```python
import os

client = Groq(
    api_key=os.getenv("GROQ_API_KEY")
)
```

---

## Run

Open the notebook:

```bash
NeuralCity_GovInsight.ipynb
```

Run all cells.

Launch the Gradio application and open the generated public URL.

---

## Example Test Questions

```text
Which state produced the most rice in 2010?

Which state produced the most wheat in 2012?

Top 5 rice producing states in 2010

Show rice production trend in Punjab

Show wheat production trend in Punjab

Compare rice production in Punjab and Haryana in 2010

Give summary of rice production in Punjab in 2010

What is India's GDP?
```

---

## Future Improvements

- Additional agricultural datasets
- Multi-crop comparison
- District-level analytics
- Export reports to PDF
- Advanced dashboards

---

## Author

Prince
B.Tech AI

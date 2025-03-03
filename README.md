# Data Analysis Agent

## Overview
This Streamlit application leverages **LangChain**, **OpenAI**, and **Matplotlib** to create an interactive data analysis agent. Users can query a dataset using natural language and visualize insights through dynamically generated graphs.

## Features
- **Chat Interface**: Ask questions about the dataset and receive responses.
- **Data Visualization**: Automatically generates graphs for relevant queries.
- **Chat History Preservation**: Stores and displays previous messages and visualizations.
- **Supports OpenAI API**: Uses OpenAI's language model for intelligent data analysis.

## Installation
```bash
pip install streamlit pandas matplotlib langchain openai python-dotenv
```

## Setup
1. **Add OpenAI API Key**:
   - Create a `.env` file and add your OpenAI API key:
     ```
     OPENAI_API_KEY=your_api_key_here
     ```
   - Alternatively, store it in `st.secrets` if using Streamlit Cloud.

2. **Prepare Your Dataset**:
   - Place your dataset (e.g., `customers.csv`) in the project directory.

## Usage
Run the Streamlit app:
```bash
streamlit run app.py
```

## Functionality
- **Chat-Based Queries**:
  - Example: *"Show the first few rows of the dataset."*
  - Example: *"Group customers by country and plot a graph for the top 5 countries."*

- **Graph Generation**:
  - Supports automatic graph plotting based on keywords.
  - Example graphs:
    - Top 5 countries with most customers
    - Customer age distribution

## Future Enhancements
- Add more visualization types.
- Improve NLP query handling.
- Integrate additional AI models for enhanced analysis.

---
Made with Streamlit, LangChain, and OpenAI.


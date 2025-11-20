# AI-ML-Assignment-6-Prompt-Engineering
# AI/ML Assignment 6: Prompt Engineering for Performance Improvement

**Student Name:** Ermiyas H. 
**Task:** Structured Data Extraction from Purchase Records  
**LLM Used:** Google Gemini 1.5 Flash  
**Date:**  2025

## Task Description

Extract structured purchase information from unstructured e-commerce transaction text and output in valid JSON format with specific fields: customer_name, product, price, purchase_date, warranty_expiration, and address.

**Challenge:** The model must correctly identify the main product price ($2,499) and exclude the add-on AppleCare price ($379), demonstrating nuanced understanding.

## Results Comparison Table

| Test | Techniques Used | Score | Key Achievement |
|------|----------------|-------|-----------------|
| **Baseline** | None (vague instruction) | 2/10 | Baseline (poor) |
| **Technique 1** | Role Prompting | 5/10 | Professional tone, more complete |
| **Technique 2** | Role + Output Formatting | 7/10 | Structured JSON output |
| **Technique 3** | Role + Format + Chain-of-Thought | 8/10 | Accurate extraction with reasoning |
| **Final Optimized** | Role + Format + CoT + Explicit Rules | 9/10 | Clean, accurate, production-ready |

## Performance Gain

**Baseline → Final:** 350% improvement (2/10 → 9/10)

## Key Lessons Learned

1. **Specificity Matters:** Vague instructions fail completely. Explicit output format requirements dramatically improve structure.

2. **Role Prompting Sets Context:** Defining the model as an "expert Data Analyst" shifts its internal knowledge distribution toward more professional responses.

3. **Chain-of-Thought Enhances Accuracy:** Breaking tasks into explicit steps reduces field extraction errors, especially for nuanced requirements like "exclude add-ons from price."

4. **Combination is Key:** No single technique achieved 9/10 performance. The final prompt combines all techniques successfully.

5. **Practical Insight:** For structured extraction tasks, prompt engineering can eliminate the need for fine-tuning entirely - directly relevant to our coursework on RAG vs fine-tuning approaches.

## Repository Structure
```
AI-ML-Assignment-6-Prompt-Engineering/
├── prompt_engineering_assignment.ipynb
├── README.md
└── constant_input.txt
```

## How to Run

### Prerequisites
- Anaconda Python 3.10+
- Free Gemini API key from https://aistudio.google.com/app/apikey

### Setup
```bash
conda create -n prompt_engineering python=3.10 -y
conda activate prompt_engineering
pip install google-generativeai jupyter pandas
jupyter notebook
```

### Execution
1. Open `prompt_engineering_assignment.ipynb`
2. Add your Gemini API key in Cell 1
3. Run all cells sequentially

## Video Demonstration

[YouTube Link - to be added after recording]
```

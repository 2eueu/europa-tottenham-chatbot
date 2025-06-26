# Europa Match Chatbot

## Project Overview

**Europa Match Chatbot** is an interactive system that allows users to search for highlight moments from Tottenham’s UEFA Europa League knockout stage matches.  
By analyzing live match commentaries from 5 matches (Quarterfinals, Semifinals, and Final), the chatbot provides keyword-based scene retrieval with emojis and natural-language outputs.

---

## 🔍 Key Features

1. **Match-Based Search**
   - Users can enter queries like `"goal Son"` or `"penalty VAR"`  
   - The chatbot searches through real-time match commentary data (`comments_*.json`)

2. **Highlight Retrieval**
   - Relevant match scenes are retrieved and formatted with emojis (⚽ Goal, 📕 Card, 🟨 VAR)
   - Each response includes the match name and a brief context

3. **Natural Language Processing (NLP)**
   - Basic keyword matching and context-aware filtering
   - Capable of identifying multiple events per match

4. **Data Source**
   - 5 UEFA Europa League matches from Tottenham Hotspur (2024–2025)
     - Quarterfinal 1st & 2nd legs  
     - Semifinal 1st & 2nd legs  
     - Final  
   - JSON-format comment logs scraped from SofaScore and Opta Match Summaries

---

## 🧠 How It Works

1. User types a keyword →  
2. System scans all match comment JSON files →  
3. Matches found → highlight snippets generated →  
4. Output presented in Markdown-like structured response

---

##  Technologies Used

###  Language & Tools  
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)  
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

### Data Format  
[![JSON](https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=json&logoColor=white)](https://www.json.org/)

###  Libraries  
`pandas`, `re`, `emoji`, `IPython.display`

---

## Sample Output

```
🆚 Tottenham vs Eintracht Frankfurt  
⚽ 34' GOAL by Son Heung-min — brilliant finish from the edge of the box!

🟨 56' VAR check for handball — no penalty awarded
```

---

##  File Structure

```
 data/
  ├─ comments_qf1.json
  ├─ comments_qf2.json
  ├─ comments_sf1.json
  ├─ comments_sf2.json
  └─ comments_final.json

 uefa_comment_bot.ipynb
```

---

## Author

- **GaEun Lee**  
- Department of AI Engineering, Sookmyung Women’s University  
- GitHub: [2eueu](https://github.com/2eueu)

---

##  License

MIT License © 2025 GaEun Lee (2eueu_)

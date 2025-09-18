# Generate-Nutrition-MCQ-from-PDF
This repository contains code of Langflow which generates MCQ from the PDF Uploaded in Astra DB https://astra.datastax.com/

# Quiz Generator with LangFlow
Create auto-generated multiple-choice quizzes (MCQs) for any topic using a no-code/low-code GenAI flow in LangFlow.
________________________________________
# Project Goal
Build a GenAI pipeline that takes a topic (e.g., "Diet and Nutrition") and question count, and returns a validated multiple-choice quiz with answer key and rationales.
________________________________________
Key Features
•	Topic-driven quiz generation for MCQs only
•	Difficulty levels (easy / medium / hard)
•	Configurable number of questions
________________________________________
# Architecture (Flow Overview)
Input → Astra DB → Parser → Prompt Template → LLM → Output
Components you’ll use in LangFlow
•	Input: topic, number of questions
•	Astra DB: store and retrieve context
•	Parser: enforce schema and structure
•	Template: PromptTemplate composing system + user instructions
•	LLM: Groq
•	Output: Display
________________________________________
# Tech Stack
•	LangFlow (visual orchestration UI)
•	Astra DB (database for context & storage)
•	LLM provider: Groq
•	Python 3.12.1
########################Sample Output#########################

 
# User
Create the 10 mcq questions of quiz on the Diet and Nutrition

Answer Key
D – The guidelines do not advise eating three servings of red meat daily.
C – Cashews have the highest caloric value among the listed nuts.
B – Approximately 55 g of protein is recommended for a sedentary adult man.
C – Cucumber falls under the low‑calorie (< 100 kcal) category.
B – GI measures how quickly a food raises blood glucose levels.
A – Flaxseed oil is the richest source of ALA per 100 g.
B – Normal adult BMI is 18.5–24.9 kg/m².
A – Guideline 4 specifically addresses regular physical activity.
B – Soaking in water with a small amount of sodium bicarbonate helps remove residues.
B – Whole‑grain wheat chapati is the main complex‑carbohydrate source in the plan.




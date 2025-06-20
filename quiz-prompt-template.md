### Prompt Template: Generate a Multiple-Choice Quiz

**Instructions:**  
Create a multiple-choice quiz with the following criteria:
- Include **between 5 and 15 questions**
- Each question must have **4 answer options**
- Only one correct answer per question
- Clearly indicate the correct answer using the **index** of the correct option
- Include a brief **explanation** for each correct answer
- Use structured **JSON** format with these fields:
  - `question`: The text of the question
  - `options`: Array of 4 answer choices
  - `answer`: Array with the index (0-based) of the correct option
  - `explanation`: Clarifies why that answer is correct
  - `type`: Always set as `"singleSelect"`
- Add a root `title` field and set `type` to `"quiz"`

**Topic:** *[Insert your quiz topic here]*  
Examples:  
- Power BI DAX Functions  
- JavaScript Array Methods  
- Python for Data Science  
- Cybersecurity Fundamentals  
- Beginner Spanish Vocabulary

---

### Example Prompt Usage

> Create a multiple-choice quiz with 10 questions about **Power BI DAX functions**, each with 4 options and one correct answer. Use JSON format with the fields: `question`, `options`, `answer`, `explanation`, and `type` set as `"singleSelect"`. Also add a `title` for the quiz and a top-level `type` set to `"quiz"`.

### Simplified version
```markdown
> Create a multiple-choice quiz with the following structure: > - Between 5 and 15 questions. > - Each question should include 4 answer options. > - Only one correct answer per question. > - Clearly indicate the correct option(s) using the index. > - Include a clear and concise explanation for each correct answer. > - Organize the output as structured JSON with the following fields: > question, options (array), answer (array with index of correct option), explanation, type ("singleSelect"). > - Add a title field and set type to "quiz".

> Topic: [Insert quiz topic here] 
# Example topics: Power BI DAX functions, React.js basics, Python data structures, European history, beginner Spanish vocabulary, cybersecurity fundamentals, etc.
```

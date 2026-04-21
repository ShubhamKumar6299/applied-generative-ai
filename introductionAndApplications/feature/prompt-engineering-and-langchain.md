IN-CONTEXT LEARNING
______________________
ADVANTAGES
* no fine tuning needed
* reduces time and resource consumption
* improves performance

DISADVANTAGES
* limited to what can fit in-context
* complex tasks need gradient steps
* involves adjustments based on error gradients
________________________________
 ## PROMPT ENGINEERING
 - instructions => what needs to be done
 - context => help llm understand the scenario
 - Input Data
 - Output indicator

_____________________________________
## INTRO TO LANGCHAIN (python framework)
- chaining => retrieval, extraction, processing, generation
# advantages
- modularity
- extensibility
- decomposition capabilities
- vector database compatability
# practical applications
- content summarization
- data extraction
- question aswering
- automated content generation
__________________________________________

##advanced method of prompt engineering


*******                 NOTES       ******

# Prompt Engineering Recap Notes

## 1. Advanced Prompting Techniques

### Zero-shot Prompting
- No examples are provided
- Model relies entirely on pre-trained knowledge

### Few-shot Prompting
- A few examples are given in the prompt
- Helps guide the model toward better outputs

### Chain-of-Thought (CoT) Prompting
- Encourages the model to explain reasoning step-by-step
- Improves performance on complex problems (logic, math)

### Self-Consistency
- Generate multiple reasoning paths
- Select the most consistent/majority answer
- Improves reliability

---

## 2. Prompt Engineering Tools

- Tools help facilitate interactions with LLMs
- Enable better structuring and reuse of prompts
- Improve efficiency and consistency

---

## 3. LangChain and Prompt Templates

- LangChain uses **prompt templates**
- Prompt templates are:
  - Predefined structures for prompts
  - Reusable and dynamic (support variables)
  - Useful for generating consistent outputs

### Example
- Answer the following question: {question}

---

## 4. Agents in Prompt Applications

- Agents are systems that:
  - Use multiple prompts
  - Make decisions dynamically
  - Perform complex, multi-step tasks

### Key Idea
- Agents orchestrate multiple prompts instead of relying on a single input
- Useful for handling workflows across different domains

---

## 5. Key Takeaways

- Advanced prompting techniques improve output quality
- Prompt tools and templates enable scalable applications
- LangChain simplifies LLM-based development
- Agents allow automation of complex tasks



# LangChain LCEL Chaining Method

## 1. Introduction to LCEL

- LCEL (LangChain Expression Language) is used to structure workflows
- It simplifies chaining of components using a clean syntax
- Uses the **pipe (`|`) operator** to connect components

---

## 2. Creating an LCEL Pattern

### Steps to Build a Chain

1. Define a template with variables in curly braces `{}`  
2. Create a prompt template instance  
3. Build a chain using the pipe (`|`) operator  
4. Invoke the chain with input values  

---

## 3. Prompt Templates

- Prompts use templates with variables:

"What is the capital of {country}?"


- Variables are dynamically replaced during execution

---

## 4. Runnable (Core Concept)

- Fundamental building block in LCEL
- Acts as a pipeline component

### Structure

Input → Runnable → Output


### Can Connect:
- LLMs
- Retrievers
- Tools

---

## 5. RunnableSequence

- Executes components **sequentially**
- Output of one component → Input of next

### Flow

Input → Step1 → Step2 → Step3 → Output


---

## 6. RunnableParallel

- Runs multiple components **concurrently**
- All components receive the **same input**

### Use Case
- When you want multiple outputs at the same time

---

## 7. LCEL Simplification

- Replaces `RunnableSequence` with pipe operator (`|`)
- Makes code more readable and concise

### Example Concept

prompt | model | parser


---

## 8. Type Coercion in LCEL

- Automatically converts objects into runnable components

### Conversions:
- Functions → `RunnableLambda`
- Dictionaries → `RunnableParallel`

- Reduces manual effort and boilerplate code

---

## 9. Key Features of LCEL

- Clean and readable syntax
- Supports both sequential and parallel workflows
- Automatic type conversion
- Easy integration with LLMs and tools
- Scalable for complex pipelines

---

## 10. LCEL Strengths

- Simplifies workflow creation
- Reduces complexity compared to traditional chaining
- Enables modular and reusable pipelines
- Supports advanced orchestration of components

---

## 11. Recap

- LCEL uses pipe (`|`) operator for chaining
- Prompt templates use `{}` for dynamic variables
- Runnable connects components into pipelines
- RunnableSequence → sequential execution
- RunnableParallel → concurrent execution
- LCEL simplifies chaining and handles type conversion automatically


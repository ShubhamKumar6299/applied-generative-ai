***            RAW NOTES, STRUCTURED NOTES BEGINS FROM LINE 57 ***

****       What are generative AI models?  ***
________________________________________________________
* LLMs are part of foundation models which is part of generative AI
=> nlp task? (we can tune our model to perform very natural nlp task)

advantage of these models
* performance
* productivity

disadvantages
* compute cost
* trust

__________________________________________________________
***    WHAT IS NLP(natural language processing)
__________________________________________________________
* UNSTRUCTURED should be structured for machine or llm to understand

NLP translate betweeen unstructured to structerd, it sits between them and called (NLU = > natural language understand and NLG=> natural language generation)

* we need to understand the context for translating between unstructured to structured and vice versa
* MACHINE TRANSLATION
* VIRTUAL ASSISTANT CHATBOTS
* SENTIMENT ANALYSIS
* SPAM DETECTION

* first stage of NLP is "TOKENIZATION"
*  we work one token a time and first stage is "STEMMING"
* LEMMATIZATION
* PART OF SPEECH TAGGING
               __________________________________________
               |                                         |
               |           TOKENIZATION                  |
               |________________________________________
                     /                \
                    /                  \

            ____________________        __________________________
            |  STEMINGS         |       |  LEMMATIZATION          |
            ____________________         _________________________
                   \                           /
                   ______________________________________________
                  |            PART OF SPEECH TAGGING           |
                  _______________________________________________
                                     |
                  ________________________________________________
                 |  NAME ENTITY RECOGNITION(N.E.R)              |
                 ________________________________________________

//DETAILED LINK FOR REFERENCE OF ALL THE REQUIRED MATERIAL

https://www.coursera.org/learn/develop-generative-ai-applications-get-started/supplement/09NTh/reading-comprehensive-guide-to-generative-ai


***     STRUCTURED NOTES    ***


# Generative AI and NLP Notes

## 1. Generative AI Models

Generative AI models are systems capable of generating new content such as text, images, code, and audio based on learned patterns from data.

### Hierarchy
Generative AI → Foundation Models → LLMs → NLP Tasks

- LLMs (Large Language Models) are a subset of foundation models.
- They are primarily used for natural language processing tasks.
- Models can be fine-tuned for specific use cases.

### Advantages
- High performance
- Increased productivity

### Disadvantages
- High computational cost
- Trust issues (e.g., hallucinations, incorrect outputs)

---

## 2. Natural Language Processing (NLP)

NLP is a field of AI that enables machines to understand, interpret, and generate human language.

### Core Concept
- Human language is unstructured.
- Machines require structured data.
- NLP acts as a bridge between unstructured and structured data.

### Components
- NLU (Natural Language Understanding)
- NLG (Natural Language Generation)

---

## 3. Applications of NLP

- Machine Translation
- Chatbots / Virtual Assistants
- Sentiment Analysis
- Spam Detection

---

## 4. NLP Processing Pipeline

### 4.1 Tokenization
- Splitting text into smaller units (tokens)
- First step in NLP

### 4.2 Stemming
- Reduces words to root form
- Example: "running" → "run"

### 4.3 Lemmatization
- Converts words to their meaningful base form
- More accurate than stemming

### 4.4 Part of Speech Tagging
- Identifies grammatical roles (noun, verb, adjective, etc.)

### 4.5 Named Entity Recognition (NER)
- Extracts entities such as:
  - Person names
  - Locations
  - Organizations
  - Dates

---

## 5. NLP Workflow

Tokenization  
→ Stemming / Lemmatization  
→ Part of Speech Tagging  
→ Named Entity Recognition  

---

## 6. Additional Generative AI Concepts

- Prompting: Designing inputs to guide model output
- Prompt Templates: Reusable structured prompts
- RAG (Retrieval-Augmented Generation): Combines retrieval with generation
- Agents: Autonomous systems capable of reasoning and task execution
- Vector Databases: Store embeddings for similarity search
- Fine-tuning: Customizing models with domain-specific data

---

## 7. Summary

- Generative AI enables content creation
- LLMs power most NLP applications
- NLP converts unstructured language into structured data
- Processing involves multiple stages from tokenization to entity recognition
- Challenges include computational cost and reliability



## NLP FLOW DIAGRAM 

                 TOKENIZATION
                      |
        -------------------------------
        |                             |
     STEMMING                  LEMMATIZATION
        |                             |
        ----------- MERGED ------------
                      |
          PART OF SPEECH TAGGING
                      |
      NAMED ENTITY RECOGNITION (NER)



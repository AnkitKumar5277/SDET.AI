# RAG

RAG = Retrieval-Augmented Generation

AI pehle aapke documents mein search karta hai, phir usi information ke basis par answer deta hai.

Matlab AI guess nahi karta, balki document se answer nikalta hai.

RAG is a technique that allows an AI model to answer questions using your own documents instead of relying only on its training.
---

## Q: Company mein kitni Casual Leaves hain?

Without RAG - AI guess karega.

With RAG:

```text
User Question
      │
      ▼
Company PDF Search
      │
      ▼
Relevant Information
      │
      ▼
AI Answer
```

---

## RAG Ki Need Kyu Hai?

Suppose company ke paas:

- HR Policy PDF
- Test Cases
- Requirement Documents
- API Documentation
- User Manual

AI ko ye sab pata nahi hota.

RAG:

- ✅ Documents read karta hai
- ✅ Relevant information search karta hai
- ✅ Sirf wahi information AI ko bhejta hai
- ✅ Accurate answer deta hai

---

## Real Life Example

Suppose ek PDF hai.

**Company Policy**

- Casual Leave = 12
- Sick Leave = 10
- Work From Home = 2 Days

User poochta hai:

> How many casual leaves?

RAG:

```text
Search PDF
     ↓
Find "Casual Leave =12"
     ↓
AI
     ↓
Answer:
Employees get 12 casual leaves.
```

---

# RAG Architecture

```text
PDF

↓

Loader

↓

Text Split

↓

Embeddings

↓

Vector Database

↓

Retriever

↓

LLM

↓

Answer
```

---

## Loader

Loader ka kaam hota hai document read karna.

Example:

```text
Company.pdf

↓

Loader

↓

Text
```

Python:

```python
loader = PyPDFLoader("company.pdf")
docs = loader.load()
```

---

## Text Splitter

LLM ek baar mein bahut bada PDF nahi padh sakta.

Isliye document ko chote pieces (chunks) mein todte hain.

Example:

```text
100 Pages

↓

Chunk 1

Chunk 2

Chunk 3

Chunk 4
```

Example:

- Chunk Size = 500 characters
- Overlap =100

---

## Chunk Overlap

Suppose text:

```text
Python is a programming language.

It is easy to learn.
```

Without overlap:

```text
Chunk1

Python is a programming

Chunk2

language. It is easy...
```

Sentence toot gaya.

With overlap:

```text
Chunk1

Python is a programming language.

Chunk2

programming language.

It is easy...
```

Context maintain rehta hai.

---

## Embeddings

Ye sabse important concept hai.

Computer text ko directly understand nahi karta.

Isliye text ko numbers mein convert kiya jata hai.

Example

```text
Python

↓

[0.12, 0.56, 0.98, ....]
```

Ye numbers hi Embeddings kehlate hain.

---

## Vector Database

Ab embeddings ko store karna hota hai.

Ye kaam Vector Database karta hai.

Popular databases:

- FAISS
- ChromaDB
- Pinecone
- Qdrant
- Milvus

Example

```text
Embeddings

↓

Vector Database

↓

Saved
```

---

## Similarity Search

User poochta hai:

```text
Leave Policy
```

Vector DB compare karta hai:

```text
Question

↓

Document 1

95%

Document 2

20%

Document 3

70%
```

Highest similarity wala document return hota hai.

---

## LLM

Ab relevant text AI ko diya jata hai.

Example:

```text
Context

Casual Leave =12

Question

How many leaves?

↓

GPT

↓

12 Casual Leaves
```

AI sirf context ke basis par answer deta hai.

---

## Complete RAG Flow

```text
User Question

↓

Vector Search

↓

Top 3 Chunks

↓

GPT

↓

Final Answer
```

---

# QA Engineers ke Liye RAG Projects

Agar aap QA ya SDET ho, to ye projects resume mein strong lagenge:

## 1. Test Case Search Bot

Test cases upload karo.

AI se poochho:

> "Login test case dikhao."

---

## 2. Bug Report Chatbot

Purane bug reports search karo.

Duplicate bugs identify karo.

---

## 3. Requirement Document Assistant

BRD/SRS upload karo.

AI se requirements poochho.

---

## 4. API Documentation Chatbot

API docs upload karo.

Endpoint, request, response ke answers lo.

---

## 5. Company Policy Chatbot

HR documents upload karo.

Leave policy, holidays, WFH policy poochho.

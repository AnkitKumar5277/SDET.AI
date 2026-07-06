# RAG  
RAG = Retrieval-Augmented Generation  
AI pehle aapke documents mein search karta hai, phir usi information ke basis par answer deta hai.  
Matlab AI guess nahi karta, balki document se answer nikalta hai.  

### Q: Company mein kitni Casual Leaves hain?
Without RAG - AI guess karega.
With RAG:
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

### RAG Ki Need Kyu Hai? 
Suppose company ke paas:  
HR Policy PDF  
Test Cases  
Requirement Documents  
API Documentation
User Manual

AI ko ye sab pata nahi hota.

RAG:
✅ Documents read karta hai
✅ Relevant information search karta hai
✅ Sirf wahi information AI ko bhejta hai
✅ Accurate answer deta hai

### Real Life Example
Suppose ek PDF hai.
Company Policy
Casual Leave = 12
Sick Leave = 10
Work From Home = 2 Days

User poochta hai:
How many casual leaves?

RAG:
Search PDF
↓
Find "Casual Leave =12"
↓
AI
↓
Answer:
Employees get 12 casual leaves.

### RAG Architecture
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


### Loader
Loader ka kaam hota hai document read karna.

Example:

Company.pdf

↓

Loader

↓

Text

Python:

loader = PyPDFLoader("company.pdf")
docs = loader.load()

### Text Splitter

LLM ek baar mein bahut bada PDF nahi padh sakta.

Isliye document ko chote pieces (chunks) mein todte hain.

Example:

100 Pages

↓

Chunk 1

Chunk 2

Chunk 3

Chunk 4

Example:

Chunk Size = 500 characters

Overlap =100

### Chunk Overlap
Suppose text:

Python is a programming language.

It is easy to learn.

Without overlap:

Chunk1

Python is a programming

Chunk2

language. It is easy...

Sentence toot gaya.

With overlap:

Chunk1

Python is a programming language.

Chunk2

programming language.

It is easy...

Context maintain rehta hai.



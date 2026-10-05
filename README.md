# C# 14 &amp; .NET 10 — From Fundamentals to AI Engineering

A single Python script that generates a complete, bookmarked PDF textbook:
**C# 14 & .NET 10 — From Fundamentals to AI Engineering** (301 pages, A4).

The book is a practical, project-driven route through modern C# and real AI
engineering — from your first line of C# 14, through object-oriented design,
collections, and algorithms, to shipping production AI (RAG, Semantic Kernel,
local ONNX models, agents, and Native AOT microservices).

## Contents of this repo

| File | Description |
|------|-------------|
| `build_csharp_book.py` | The complete book generator (layout, styling, chapters, appendices, cover, TOC). |
| `requirements.txt` | Python dependencies. |
| `.gitignore` | Excludes caches, scratch, and the generated PDF. |

> The PDF itself is a build artifact and is **not** committed. Run the build
> below to generate `CSharp_14_and_NET_10_From_Fundamentals_to_AI_Engineering.pdf`.

## Requirements

- **Python 3.10+**
- **ReportLab** (`pip install -r requirements.txt`)
- **Fonts (optional, recommended):** the premium look uses Windows system fonts
  — Georgia (serif body), Segoe UI (sans headings), and Consolas (code). On
  Windows these are already present. If any are missing, the script
  automatically falls back to the built-in core fonts (Times/Helvetica/Courier),
  so it still builds everywhere — just with plainer typography.

## Build

```powershell
pip install -r requirements.txt
python build_csharp_book.py
```

This writes `CSharp_14_and_NET_10_From_Fundamentals_to_AI_Engineering.pdf` next
to the script.

## Design notes

- **Typography:** Georgia serif body (~10.5/15), Consolas code (~8.6/11.4),
  Segoe UI Bold headings — tuned to match a premium publisher layout.
- **Cover:** white page with a light content panel, a full-width gradient bar,
  a serif two-tone title, a centered isometric diamond cluster, and author /
  edition blocks pinned above the footer.
- **Contents:** colored left-pipe markers on chapters, indented plain
  sub-sections, a gradient underline rule, and no page-number dot leaders.
- **Section headings:** every section carries a colored left pipe bar; callouts
  use a left accent bar (note / try-it / pitfall / learn).
- **Bookmarks:** a full PDF outline is generated from the chapter and section
  structure; the on-page Contents is generated from the same entries.

## Book structure

The book is organized into nine parts (68 chapters) with full-page part
dividers, a worked capstone per phase, and eleven appendices.

### Part I — Modern C# Language Foundations
1. Install, Create, Compile, Run
2. Variables, Constants, and the Type System
3. Operators and Control Flow
4. Strings and Text
5. Arrays, Ranges, and Indices
6. Methods and Parameters

### Part II — Object-Oriented C#
7. Classes and Object Construction
8. Properties and Indexers
9. Access Levels, Static Members, and Namespaces
10. Inheritance and Redefining Members
11. Composition, Encapsulation, and Polymorphism
12. Interfaces and Abstract Classes
13. Structs, Enums, and Records

### Part III — Advanced C# Features
14. Exception Handling and Resource Lifetime
15. Delegates, Lambdas, and Events
16. Generics and Constraints
17. Operator Overloading and Custom Conversions
18. Preprocessor and Compilation Controls
19. Asynchronous Methods and Streams

### Part IV — Data Structures and Algorithms
20. Lists and Linked Structures
21. Sorting Algorithms
22. Stacks, Queues, and Priority Queues
23. Dictionaries and Sets
24. Basic and Binary Trees
25. Binary Search Trees
26. AVL and Red-Black Trees
27. Heaps: Binary, Binomial, and Fibonacci
28. Graph Concepts and Representation
29. Graph Traversal
30. MST, Coloring, and Shortest Paths

### Part V — Robust, Testable Applications
31. Robust, Extensible, Testable Applications
32. Capstone: Support Dispatch System

### Part VI — AI Engineering with C#
33. Modern C# for AI Engineers
34. How AI Actually Works for Developers
35. Your First AI Call
36. Classical ML with ML.NET
37. Orchestration with Semantic Kernel
38. Embeddings and Vector Databases
39. Retrieval-Augmented Generation (RAG)
40. Performance Tuning and Native AOT
41. Local Inference with ONNX Runtime
42. AI Observability with OpenTelemetry
43. Responsible AI and Guardrails
44. Capstone I — ComplianceBot Architecture and Ingestion
45. Capstone II — Pipeline, Performance, and Guardrails

### Part VII — Deeper Dives and Practice
46. LINQ and Functional Data Pipelines
47. Spans, Memory, and High-Performance C#
48. Dependency Injection and Configuration
49. Unit Testing and TDD with xUnit
50. Minimal APIs and Web Services
51. Prompt Engineering Patterns in C#
52. Evaluating and Testing AI Systems
53. Deploying AI Services

### Part VIII — Agentic AI and LLM Internals
54. Building an LLM Agent in C#
55. Multi-Agent Systems in C#
56. How LLMs Work Inside

### Part IX — Applied AI: Projects, Frameworks, and the Future
57. AI Tools and Function Calling
58. Memory Systems for Agents
59. Fine-Tuning and Model Customization
60. AI Frameworks and the Model Context Protocol
61. Project — An End-to-End RAG Pipeline
62. Project — A Real-World ML.NET Application
63. Project — An Autonomous Research Agent
64. Working with Local and Open-Source Models
65. Full-Stack AI Apps with Blazor and .NET
66. Advanced Topics and Future Trends
67. Document Intelligence and Multimodal Inputs
68. Speech and Real-Time AI

### Appendices
- **A** — The Companion Monorepo
- **B** — C# 14 Quick Update
- **C** — Complexity Cheat Sheet
- **D** — Exercises and Worked Solutions
- **E** — C# 14 & 15 Feature Tour
- **F** — Patterns and Idioms
- **G** — Glossary
- **H** — Resources and Further Reading
- **I** — Project Briefs
- **J** — Answers to Conceptual Questions
- **K** — AI Engineering Production Checklist

### Chapter anatomy

Each chapter follows a consistent, teach-by-example rhythm:

- A **chapter banner** and a short lead that frames why the topic matters.
- A **"You will learn"** box listing the chapter's objectives.
- **Sections** that each open with a short, runnable snippet, then explain what
  it is, why it matters, how the syntax works, and what can go wrong.
- **Try-it** prompts that turn reading into deliberate practice.
- A **Common pitfalls** box, a **Chapter summary**, and a **Knowledge check**
  (answers in Appendix J).

## License

Content and code © Michael Muruthi. Add your preferred license here before
publishing (e.g., MIT for the code, and a separate notice for the book text).

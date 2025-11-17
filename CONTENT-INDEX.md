# 📚 Complete LangChain4j Content Index

Quick reference to find exactly what you need!

---

## 🗺️ Navigation Guide

```
Spring-AI/
│
├── 📄 START-HERE.md                          ⭐ BEGIN HERE
│   └── Your entry point and roadmap
│
├── 📘 Main Guides/
│   ├── LANGCHAIN4J-LEARNING-PATH.md          21-day structured course
│   ├── LANGCHAIN4J-COMPLETE-GUIDE.md         Comprehensive reference
│   ├── LANGCHAIN4J-QUICKSTART.md             5-minute setup
│   └── ENHANCED-CONTENT-GUIDE.md             What's new & how to use
│
└── 📚 Learning Modules/
    │
    ├── Module 1: Foundations/ ⭐⭐⭐⭐⭐
    │   ├── README.md                         Theory & concepts
    │   └── examples/
    │       ├── Example01_HelloWorld.java     🟢 EASY | 100 lines
    │       ├── Example02_PromptTemplates.java 🟢 EASY | 150 lines
    │       ├── Example03_SystemMessages.java  🟡 MEDIUM | 200 lines
    │       └── Example04_Streaming.java       🟡 MEDIUM | 150 lines
    │
    ├── Module 2: Structured Interactions/ ⭐⭐⭐⭐
    │   ├── README.md
    │   └── examples/
    │       ├── Example01_BasicAIService.java  🟢 EASY | 250 lines
    │       └── Example02_StructuredExtraction.java 🟡 MEDIUM | 300 lines
    │
    ├── Module 3: Memory/ ⭐⭐⭐⭐⭐ [NEW!]
    │   ├── README.md
    │   └── examples/
    │       ├── Example01_BasicChatMemory.java 🟡 MEDIUM | 350 lines
    │       └── Example02_AIServiceWithMemory.java 🟡 MEDIUM | 450 lines
    │
    ├── Module 4: Tools/ ⭐⭐⭐⭐⭐ [ENHANCED!]
    │   ├── README.md
    │   └── examples/
    │       ├── Example01_SimpleCalculatorTool.java 🟡 MEDIUM | 244 lines
    │       └── Example02_MultipleTools.java   🔴 ADVANCED | 600 lines
    │
    └── Module 5: RAG/ ⭐⭐⭐⭐⭐ [NEW!]
        ├── README.md
        └── examples/
            └── Example01_SimpleRAG.java       🔴 ADVANCED | 550 lines
```

---

## 📊 Content Matrix

| Module | Examples | Lines | Theory % | Difficulty | Time |
|--------|----------|-------|----------|------------|------|
| **Module 1** | 4 | ~600 | 50% | 🟢 Beginner | 2-3 days |
| **Module 2** | 2 | ~550 | 55% | 🟢 Beginner | 2-3 days |
| **Module 3** | 2 | ~800 | 60% | 🟡 Intermediate | 2-3 days |
| **Module 4** | 2 | ~850 | 60% | 🟡 Intermediate | 3-4 days |
| **Module 5** | 1 | ~550 | 65% | 🔴 Advanced | 3-4 days |
| **TOTAL** | **11** | **~3,350** | **58%** | Progressive | **12-17 days** |

---

## 🎯 Quick Find: What You Need

### "I Want to Learn..."

#### Basic LLM Interaction
→ **Module 1, Example 1**: `Example01_HelloWorld.java`
- First LLM call
- Model configuration
- Simple prompts

#### Prompt Engineering
→ **Module 1, Example 2**: `Example02_PromptTemplates.java`
- Template variables
- Reusable prompts
- Dynamic content

#### AI Personalities
→ **Module 1, Example 3**: `Example03_SystemMessages.java`
- System messages
- Persona definition
- Behavior control

#### Type-Safe AI Services
→ **Module 2, Example 1**: `Example01_BasicAIService.java`
- Interface-based AI
- @UserMessage annotation
- Automatic implementation

#### Extract Structured Data
→ **Module 2, Example 2**: `Example02_StructuredExtraction.java`
- POJOs from text
- JSON parsing
- Complex objects

#### Conversation Memory
→ **Module 3, Example 1**: `Example01_BasicChatMemory.java`
- Chat history
- Message window
- Memory management

#### Multi-User Memory
→ **Module 3, Example 2**: `Example02_AIServiceWithMemory.java`
- @MemoryId annotation
- Separate conversations
- Memory stores

#### Function Calling
→ **Module 4, Example 1**: `Example01_SimpleCalculatorTool.java`
- @Tool annotation
- Basic tool creation
- Tool execution

#### Multi-Tool Agents
→ **Module 4, Example 2**: `Example02_MultipleTools.java`
- Multiple tools
- Tool coordination
- Sequential calling

#### RAG (Document Q&A)
→ **Module 5, Example 1**: `Example01_SimpleRAG.java`
- Complete RAG pipeline
- Embeddings
- Semantic search

---

## 📖 Content by Topic

### 🎨 Prompting
| Location | Topic | Lines |
|----------|-------|-------|
| M1-E2 | Templates & Variables | 150 |
| M1-E3 | System Messages & Personas | 200 |
| M2-E1 | Annotations (@UserMessage) | 250 |

### 🧠 Memory & Context
| Location | Topic | Lines |
|----------|-------|-------|
| M3-E1 | Basic Chat Memory | 350 |
| M3-E2 | AI Service Memory | 450 |
| M3-E2 | Multi-User (@MemoryId) | 450 |

### 🛠️ Tools & Actions
| Location | Topic | Lines |
|----------|-------|-------|
| M4-E1 | Simple Tools | 244 |
| M4-E2 | Multiple Tools | 600 |
| M4-E2 | Stateful Tools | 600 |

### 📄 RAG & Documents
| Location | Topic | Lines |
|----------|-------|-------|
| M5-E1 | Complete RAG Pipeline | 550 |
| M5-E1 | Embeddings | 550 |
| M5-E1 | Semantic Search | 550 |

### 🏗️ Patterns & Architecture
| Location | Topic | Lines |
|----------|-------|-------|
| M2-E1 | AI Service Pattern | 250 |
| M2-E2 | Structured Extraction | 300 |
| M3-E2 | Memory Provider Pattern | 450 |
| M4-E2 | Tool Composition | 600 |

---

## 🎓 Learning Paths

### Path 1: Quick Start (1 Week)
**Goal**: Build a simple chatbot

Day 1-2: Module 1 (all 4 examples)
Day 3-4: Module 2 (both examples)
Day 5-6: Module 3, Example 1
Day 7: Build simple chatbot project

### Path 2: Complete Course (3 Weeks)
**Goal**: Master all basics

Week 1: Modules 1-2 (6 examples)
Week 2: Module 3-4 (4 examples)
Week 3: Module 5 + Final project

### Path 3: Specific Skills

**Need Memory?**
1. Module 1, Example 1 (basics)
2. Module 3, Example 1 (memory)
3. Module 3, Example 2 (AI Service + memory)

**Need Tools?**
1. Module 1, Example 1 (basics)
2. Module 4, Example 1 (simple tool)
3. Module 4, Example 2 (multiple tools)

**Need RAG?**
1. Module 1, Example 1 (basics)
2. Module 2, Example 2 (structured extraction)
3. Module 5, Example 1 (RAG)

---

## 🔍 Find by Feature

### Annotations Used
| Annotation | Module | Example |
|------------|--------|---------|
| `@Tool` | M4 | E1, E2 |
| `@UserMessage` | M2 | E1 |
| `@SystemMessage` | M1, M2, M3 | Multiple |
| `@MemoryId` | M3 | E2 |
| `@V` | M2 | E1 |

### Classes & Interfaces
| Class | Module | Purpose |
|-------|--------|---------|
| `ChatLanguageModel` | All | LLM interaction |
| `ChatMemory` | M3 | Conversation history |
| `EmbeddingModel` | M5 | Text to vectors |
| `EmbeddingStore` | M5 | Vector database |
| `AiServices` | M2, M3, M4 | Interface-based AI |

### Patterns Demonstrated
| Pattern | Module | Example |
|---------|--------|---------|
| Builder Pattern | All | Model creation |
| Strategy Pattern | M3 | Memory strategies |
| Decorator Pattern | M4 | Tool composition |
| Factory Pattern | M2 | AI Service creation |

---

## 💻 Code Complexity

### Beginner-Friendly (🟢)
- M1-E1: Hello World (simplest!)
- M1-E2: Prompt Templates
- M2-E1: Basic AI Service

### Intermediate (🟡)
- M1-E3: System Messages
- M1-E4: Streaming
- M2-E2: Structured Extraction
- M3-E1: Basic Memory
- M3-E2: AI Service Memory
- M4-E1: Simple Tools

### Advanced (🔴)
- M4-E2: Multiple Tools (most complex logic!)
- M5-E1: RAG (most components)

---

## 📈 Theory Density

### High Theory (>60% comments)
Best for learning concepts:
- M5-E1: RAG (65%)
- M3-E1: Memory (60%)
- M3-E2: Memory (60%)
- M4-E2: Tools (60%)

### Balanced (50-60%)
Good mix of theory and code:
- M1-E2: Templates (55%)
- M2-E2: Extraction (55%)
- M1-E1: Hello World (50%)

### Code-Heavy (<50%)
Focus on implementation:
- M1-E4: Streaming (45%)
- M2-E1: Services (45%)

---

## 🎯 By Use Case

### "I Want to Build..."

#### Chatbot
1. M1-E1 (basics)
2. M3-E1 (add memory)
3. M3-E2 (multi-user)

#### Q&A System
1. M1-E1 (basics)
2. M5-E1 (RAG)
3. M2-E2 (structured answers)

#### Task Automation Agent
1. M1-E1 (basics)
2. M4-E1 (simple tools)
3. M4-E2 (multiple tools)

#### Data Extraction Tool
1. M1-E1 (basics)
2. M2-E1 (AI Services)
3. M2-E2 (structured extraction)

#### Personal Assistant
1. M1-E3 (personality)
2. M3-E2 (memory + persona)
3. M4-E2 (tools)

---

## 🚀 Quick Access Commands

```bash
# Navigate to project
cd /Users/biyadav/IdeaProjects/Spring-AI/langchain4j-learning

# Module 1
cd module-01-foundations/examples
ls -la

# Module 2
cd ../module-02-structured/examples
ls -la

# Module 3 (NEW!)
cd ../module-03-memory/examples
ls -la

# Module 4
cd ../module-04-tools/examples
ls -la

# Module 5 (NEW!)
cd ../module-05-rag-basics/examples
ls -la
```

---

## 📚 Documentation Files

### Getting Started
- `START-HERE.md` - Start here!
- `LANGCHAIN4J-QUICKSTART.md` - 5-min setup

### Learning Guides
- `LANGCHAIN4J-LEARNING-PATH.md` - 21-day course
- `LANGCHAIN4J-COMPLETE-GUIDE.md` - Full reference
- `ENHANCED-CONTENT-GUIDE.md` - New content overview

### Technical
- `langchain4j-pom.xml` - Maven dependencies
- Each `module-XX/README.md` - Module theory

---

## 🎓 Recommended Reading Order

1. **START-HERE.md** (5 min)
2. **LANGCHAIN4J-LEARNING-PATH.md** (10 min)
3. **Module 1 README** (15 min)
4. **Module 1 Examples** (1-2 days)
5. **Continue sequentially...**

---

## 💡 Pro Tips

### For Maximum Learning:
1. Read theory BEFORE code
2. Run example WHILE reading
3. Modify AFTER understanding
4. Build project AFTER module

### For Quick Reference:
1. Use this index to find topics
2. Jump to specific examples
3. Read comments in code
4. Check module READMEs

### For Projects:
1. Start with similar example
2. Copy pattern, not code
3. Adapt to your use case
4. Refer back when stuck

---

**Total Content**: 11 examples, 3,350+ lines, 58% theory, 8 comprehensive guides!

**You have everything you need to master LangChain4j!** 🎉


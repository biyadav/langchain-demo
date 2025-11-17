# LangChain4j Quick Start Guide

## 🚀 Get Started in 5 Minutes!

### Step 1: Set Up Your API Key

```bash
# Option 1: Export in terminal
export OPENAI_API_KEY=sk-your-key-here

# Option 2: Add to your shell profile (~/.zshrc or ~/.bashrc)
echo 'export OPENAI_API_KEY=sk-your-key-here' >> ~/.zshrc
source ~/.zshrc
```

Get your key from: https://platform.openai.com/api-keys

### Step 2: Copy the POM File

Use the `langchain4j-pom.xml` for your Maven project:

```bash
cd /Users/biyadav/IdeaProjects/Spring-AI
cp langchain4j-pom.xml my-langchain4j-project/pom.xml
```

Or create a new project and copy the dependencies section.

### Step 3: Run Your First Example

```bash
# Navigate to module 1
cd langchain4j-learning/module-01-foundations/examples

# Run the hello world example
java Example01_HelloWorld.java
```

## 📚 Learning Path

### Beginner (Days 1-7)
1. **Module 1**: Foundations
   - Hello World
   - Prompt Templates
   - System Messages
   - Streaming

2. **Module 2**: Structured Interactions
   - AI Services
   - Data Extraction
   - Type-safe interfaces

### Intermediate (Days 8-14)
3. **Module 3**: Memory
   - Chat Memory
   - Message Window
   - Token Window
   - Persistent Storage

4. **Module 4**: Tools
   - Function Calling
   - Multiple Tools
   - External APIs

### Advanced (Days 15-21)
5. **Module 5**: RAG Basics
   - Document Loading
   - Embeddings
   - Vector Stores

6. **Module 6**: Advanced RAG
   - Re-ranking
   - Metadata Filtering

7. **Module 7**: Agents
   - ReAct Pattern
   - Multi-Agent Systems

8. **Module 8**: Production
   - Error Handling
   - Observability
   - Best Practices

## 🎯 Quick Examples

### Hello World
```java
ChatLanguageModel model = OpenAiChatModel.builder()
    .apiKey(System.getenv("OPENAI_API_KEY"))
    .modelName("gpt-4o-mini")
    .build();

String response = model.generate("Hello!");
System.out.println(response);
```

### AI Service
```java
interface Assistant {
    @UserMessage("Translate '{{text}}' to {{language}}")
    String translate(@V("text") String text, @V("language") String lang);
}

Assistant assistant = AiServices.create(Assistant.class, model);
String result = assistant.translate("Hello", "Spanish");
```

### With Memory
```java
ChatMemory memory = MessageWindowChatMemory.withMaxMessages(10);

Assistant assistant = AiServices.builder(Assistant.class)
    .chatLanguageModel(model)
    .chatMemory(memory)
    .build();
```

### With Tools
```java
class MyTools {
    @Tool("Get current time")
    String getCurrentTime() {
        return LocalDateTime.now().toString();
    }
}

Assistant assistant = AiServices.builder(Assistant.class)
    .chatLanguageModel(model)
    .tools(new MyTools())
    .build();
```

## 📖 Project Structure

```
langchain4j-learning/
├── module-01-foundations/
│   ├── README.md              # Theory and concepts
│   └── examples/
│       ├── Example01_HelloWorld.java
│       ├── Example02_PromptTemplates.java
│       ├── Example03_SystemMessages.java
│       └── Example04_Streaming.java
├── module-02-structured/
│   ├── README.md
│   └── examples/
│       ├── Example01_BasicAIService.java
│       └── Example02_StructuredExtraction.java
├── module-03-memory/
│   ├── README.md
│   └── examples/
├── module-04-tools/
│   ├── README.md
│   └── examples/
│       └── Example01_SimpleCalculatorTool.java
└── [more modules...]
```

## 🔧 Development Tips

### Use IntelliJ IDEA
- Best IDE for Java development
- Excellent Maven support
- Great autocomplete

### Enable Annotations Processing
For Lombok support:
```
Settings → Build → Compiler → Annotation Processors
✅ Enable annotation processing
```

### Maven Commands
```bash
# Compile
mvn compile

# Run a specific class
mvn exec:java -Dexec.mainClass="com.example.Main"

# Clean and rebuild
mvn clean install
```

## 🐛 Troubleshooting

### API Key Issues
```bash
# Check if set
echo $OPENAI_API_KEY

# Should see: sk-...
# If empty, export it again
```

### Dependency Issues
```bash
# Force update
mvn clean install -U

# Clear local cache
rm -rf ~/.m2/repository/dev/langchain4j
mvn install
```

### SSL Certificate Errors (Enterprise)
Add to JVM options:
```bash
-Djavax.net.ssl.trustStore=/path/to/truststore
-Djavax.net.ssl.trustStorePassword=changeit
```

## 💡 Pro Tips

1. **Start Simple**: Run examples before modifying
2. **Read READMEs**: Each module has detailed theory
3. **Experiment**: Modify examples to learn
4. **Use Debugger**: Step through AI Service calls
5. **Check Logs**: Enable DEBUG logging to see prompts

## 🎓 Next Steps

1. ✅ Complete Module 1 exercises
2. ✅ Build a simple chatbot
3. ✅ Add tools to your bot
4. ✅ Implement memory
5. ✅ Build a complete application

## 📚 Resources

- **Official Docs**: https://docs.langchain4j.dev/
- **GitHub**: https://github.com/langchain4j/langchain4j
- **Examples**: https://github.com/langchain4j/langchain4j-examples
- **Discord**: Join the community

## 🆘 Getting Help

1. **Check README**: Most questions answered in module READMEs
2. **Read Examples**: Heavily commented code
3. **GitHub Issues**: Search existing issues
4. **Discord**: Ask the community
5. **Documentation**: Official docs are excellent

## 🎉 Ready to Start!

Open `module-01-foundations/README.md` and begin your LangChain4j journey!

```bash
cd langchain4j-learning/module-01-foundations
cat README.md
```

Happy coding! 🚀


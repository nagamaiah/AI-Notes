# AI Tools and Notes

---


## Python & Machine Learning
Python is the most popular language for AI and ML due to its simplicity and rich ecosystem.

### Key Libraries
- **NumPy:** Numerical computing
- **pandas:** Data manipulation
- **scikit-learn:** Classical ML algorithms
- **TensorFlow & PyTorch:** Deep learning frameworks
- **matplotlib & seaborn:** Data visualization


### Machine Learning Workflow
1. Data Collection
2. Data Cleaning
3. Feature Engineering
4. Model Training
5. Evaluation
6. Deployment

### Types of Machine Learning
- **Supervised Learning:** Labeled data (classification, regression)
- **Unsupervised Learning:** Unlabeled data (clustering, dimensionality reduction)
- **Reinforcement Learning:** Agents learn by interacting with environment

### Deep Learning
- Neural networks with multiple layers
- Used for image, text, and speech tasks


### LLM (Large Language Models)
- Models like GPT-3, BERT, and T5
- LLMs are trained with large datasets to understand and generate human-like text
- Most of chatbots and AI assistants built on LLMs
- LLMs can be used for tasks like translation, summarization, and question answering
- Fine-tuning LLMs for specific tasks
- LLM Examples: 
   - Using OpenAI's GPT-3 for text generation
   - Using Hugging Face's Transformers library for NLP tasks
   - Using Google's BERT for sentiment analysis
   - Using T5 for text summarization
   - Using RAG (Retrieval-Augmented Generation) for question answering



---

## AI Tools

### Jupyter Notebooks
- Interactive coding and visualization
- Widely used for prototyping and sharing research

### VS Code Extensions
- Python, Jupyter, Pylance, Copilot
- Linting, debugging, and code completion

### Data Visualization
- **matplotlib:** Basic plotting
- **seaborn:** Statistical plots
- **plotly:** Interactive charts

### Example: Plotting with matplotlib
```python
import matplotlib.pyplot as plt
plt.plot([1,2,3,4], [1,4,9,16])
plt.xlabel('x')
plt.ylabel('y')
plt.title('Sample Plot')
plt.show()
```

---

## AI Agents
See [../ai-agents/README.md](../ai-agents/README.md) for a deep dive into AI agents, their types, architectures, and use cases.

---

## Github Copilot & Microsoft Copilot Studio

### Github Copilot
- AI-powered code completion
- Supports multiple languages
- Trained on public code
- Integrates with VS Code, JetBrains, and more

### Example: Using Copilot
Type a comment describing a function, and Copilot suggests code.

### Microsoft Copilot Studio
- Build, test, and deploy Copilot extensions
- Integrate Copilot with enterprise workflows

---

## n8n Workflow Automation
n8n is an open-source tool for automating workflows and integrating services.

### Features
- Drag-and-drop workflow builder
- 350+ integrations (APIs, databases, cloud services)
- Self-hostable and scalable

### Example Workflow
1. Trigger: New email received
2. Action: Extract attachment
3. Action: Upload to Google Drive
4. Action: Send Slack notification

### Example: n8n Workflow JSON
```json
{
  "nodes": [
    {"name": "Start", "type": "n8n-nodes-base.start"},
    {"name": "HTTP Request", "type": "n8n-nodes-base.httpRequest"}
  ]
}
```

### Resources
- [n8n Docs](https://docs.n8n.io/)
- [n8n Workflows](https://n8n.io/workflows/)
- [Pulling data from services without pre-built integrations](https://n8n.io/workflows/1748-pulling-data-from-services-that-n8n-doesnt-have-a-pre-built-integration-for/)

---

## Further Reading
- [Python Official Docs](https://docs.python.org/3/)
- [scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html)
- [TensorFlow Tutorials](https://www.tensorflow.org/tutorials)
- [PyTorch Tutorials](https://pytorch.org/tutorials/)
- [VS Code AI Extensions](https://marketplace.visualstudio.com/)
- [Github Copilot](https://github.com/features/copilot)

---

## FAQ
**Q: What is the best way to learn AI/ML?**
A: Start with Python, learn basic ML concepts, and practice with real datasets.

**Q: Can I use AI tools for free?**
A: Many tools have free tiers (Jupyter, n8n, Copilot trial, etc.).

**Q: How do I automate tasks with n8n?**
A: Use the visual builder to connect triggers and actions, then deploy your workflow.

---

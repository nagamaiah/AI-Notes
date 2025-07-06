github codespaces
# chatgpt-apis

## ChatGPT APIs
OpenAI provides APIs to access ChatGPT and other models for text, code, and image generation.

### Usage
- Obtain API key from OpenAI
- Use endpoints for chat, completions, embeddings, etc.
- Libraries: openai (Python), openai-node (Node.js)

### Example
```python
import openai
openai.api_key = 'YOUR_API_KEY'
response = openai.ChatCompletion.create(model="gpt-4", messages=[{"role": "user", "content": "Hello!"}])
print(response.choices[0].message['content'])
```

### Docs
- [OpenAI API Docs](https://platform.openai.com/docs)

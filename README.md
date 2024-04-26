# example-app
This repository if for a free agent applications available on the yapp store, used to showcase how one might register the application using the developer SDK 

An example using Llava on Ollama and autogen

## Setting up model:

`litellm --model ollama/mistral`
`litellm --model ollama/llava`

Run ollama server locally:
- `OLLAMA_HOST=127.0.0.1:5050 ollama serve`

```bash
curl http://localhost:5050/api/chat -d '{
   "model": "llava:34b",
   "messages": [
     {
       "role": "user",
       "content": "why is the sky blue?"
     }
   ],
   "stream": false
}'
```
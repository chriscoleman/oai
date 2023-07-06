# oai

A minimalist OpenAI API client.

## Installation

```bash
pip install oai
```

## Usage
```python
import oai

oai.Api().post('chat/completions', json={
    'model': 'gpt-3.5-turbo',
    'messages': [
        {
            'role': 'system',
            'content': "You will introduce yourself as Batman. Then I will ask you a question which you will answer as Batman."
        },
        {
            'role': 'assistant',
            'content': "Hello, I'm Batman."
        },
        {
            'role': 'user',
            'content': 'Tell me exactly who you are and what you do using only four words.'
        }
    ]
})
```

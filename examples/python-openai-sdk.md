# Python OpenAI SDK Example

Install the SDK:

```bash
pip install openai
```

Use your APIMaster.ai API key and endpoint:

```python
from openai import OpenAI

client = OpenAI(
    api_key="YOUR_APIMASTER_API_KEY",
    base_url="YOUR_APIMASTER_BASE_URL"
)

response = client.chat.completions.create(
    model="gpt-5.4",
    messages=[
        {"role": "user", "content": "Write a short hello world message."}
    ]
)

print(response.choices[0].message.content)
```

Replace `YOUR_APIMASTER_API_KEY` and `YOUR_APIMASTER_BASE_URL` with the values from your APIMaster.ai console.

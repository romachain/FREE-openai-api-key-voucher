# Node.js OpenAI SDK Example

Install the SDK:

```bash
npm install openai
```

Use your APIMaster.ai API key and endpoint:

```js
import OpenAI from "openai";

const client = new OpenAI({
  apiKey: "YOUR_APIMASTER_API_KEY",
  baseURL: "YOUR_APIMASTER_BASE_URL"
});

const response = await client.chat.completions.create({
  model: "gpt-5.4",
  messages: [
    { role: "user", content: "Write a short hello world message." }
  ]
});

console.log(response.choices[0].message.content);
```

Replace `YOUR_APIMASTER_API_KEY` and `YOUR_APIMASTER_BASE_URL` with the values from your APIMaster.ai console.

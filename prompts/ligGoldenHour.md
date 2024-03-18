---
promptId: 'ligGoldenHour'
name: '🖼️ Generate a Golden Hour Sunlight photo'
description: 'The hour just after sunrise or just before sunset when the natural light is soft and warm. Increases the temperature of generations.'
author: 'Prompt Engineering Guide'
tags: 'photo, dalle-2,lighting'
version: '0.0.1'
output: '\n![]({{requestResults.data.0.url}})'
provider: 'custom'
endpoint: 'https://api.openai.com/v1/images/generations'
body: '{"n": 1, "size": "1024x1024", "prompt": "{{escp prompt}}"}'
headers: "{\r      \"Content-Type\": \"application/json\",\r      \"authorization\": \"Bearer {{keys.openAIChat}}\"\r}"
stream: false
---
{{selection}}, Golden Hour Sunlight
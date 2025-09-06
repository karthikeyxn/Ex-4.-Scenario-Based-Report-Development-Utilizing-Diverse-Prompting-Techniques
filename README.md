## Aim

To design and test an AI-powered chatbot for retail that can:

Handle customer inquiries.

Provide product support.

Improve customer experience.
The experiment evaluates different prompting techniques to optimize chatbot responses across ChatGPT, Claude, Bard, Cohere Command, and Meta.

## Algorithm 

Define Use Case: Retail customer support chatbot.

Select Prompting Techniques:

Zero-shot prompting (no examples).

Few-shot prompting (examples provided).

Chain-of-thought prompting (step-by-step reasoning).

Role prompting (assigning AI a role like “Customer Support Agent”).

Instruction-tuned prompting (structured rules for answering).

Design Standard Customer Queries:

Example 1: “I want to return a product I bought last week. What’s the process?”

Example 2: “Can you recommend a good wireless headphone under $100?”

Run Prompts Across AI Models: Collect responses.

Evaluation Criteria:

Accuracy of support (correct info).

Helpfulness (actionable steps).

Tone & Empathy (customer experience).

Consistency (clear structure, easy to follow).

Compare Results: Assign scores (1–5).

## Prompts (Using Different Prompting Techniques)
Zero-shot Prompt

"I want to return a product I bought last week. What’s the process?"

Few-shot Prompt

*"Example:
Q: How can I track my order?
A: You can track your order by logging into your account → Orders → Track Order.

Q: I want to return a product I bought last week. What’s the process?"*

Role Prompt

"You are a retail customer support assistant. Always respond politely, guide customers step by step, and confirm their needs before answering.
Customer: I want to return a product I bought last week."

Chain-of-Thought Prompt

*"Think step by step:

Understand what the customer wants.

Check if the query is about returns.

Provide clear steps for return.
Now answer: I want to return a product I bought last week."*

Instruction-Tuned Prompt

*"Answer the customer query in 3 parts:

Acknowledge the concern.

Provide the return process.

Offer additional help if needed.
Query: I want to return a product I bought last week."*

## Outputs (Hypothetical)
ChatGPT (Role Prompt)

*"I understand you’d like to return your purchase. Here’s how you can do it:

Go to your account → Orders → Select the product.

Click ‘Return’ and choose a reason.

Print the return label and schedule pickup.

Would you like me to help you start the return now?"*
(Polite, step-by-step, engaging)

Claude (Few-shot Prompt)

"To return your product: Log in to your account, open ‘Orders’, select the item, and choose ‘Return’. Follow the on-screen instructions to complete the process."
(Clear, concise, slightly formal)

Bard (Instruction-Tuned Prompt)

*"I’m sorry to hear you want to return your item.

Visit your orders page.

Select the item and request a return.

Print the return slip and attach it to the package.

Need help arranging courier pickup?"*
(Empathetic and conversational)

Cohere Command (Zero-shot Prompt)

"You can return it by going to your orders and selecting the return option. Then follow the return steps shown."
(Functional, but minimal detail)

Meta (Chain-of-Thought Prompt)

"Step 1: Go to your orders page.
Step 2: Select the item purchased last week.
Step 3: Click ‘Return’ → Provide reason → Confirm.
This ensures the return request is logged in our system."
(Logical, structured, slightly robotic)

## Result (Comparison Table)
| Platform    | Accuracy | Helpfulness | Tone & Empathy | Consistency | **Total** |
| ----------- | -------- | ----------- | -------------- | ----------- | --------- |
| **ChatGPT** | 5        | 5           | 5              | 5           | **20/20** |
| **Claude**  | 5        | 4           | 4              | 4           | **17/20** |
| **Bard**    | 5        | 5           | 5              | 4           | **19/20** |
| **Cohere**  | 4        | 3           | 3              | 3           | **13/20** |
| **Meta**    | 5        | 4           | 3              | 4           | **16/20** |


✅ Conclusion:

ChatGPT and Bard gave the best mix of accuracy, empathy, and customer-friendly experience.

Claude was professional but less empathetic.

Meta produced logical and structured steps but lacked warmth.

Cohere was the least detailed, making it less helpful for real customer support.

# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:  06/09/2025                                                                          
### REGISTER NUMBER : 212223230199
### Aim: To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

### Algorithm: 

### 1. **Direct Instruction Prompting**  
- **Explanation:**  
  This is the simplest and most straightforward prompting method. The AI is given a direct command with little flexibility.  
- **Detailed Example:**  
  Prompt: *“When a customer asks for the status of their order, reply with: ‘Your order is currently being processed and will be delivered by [date].’”*  
- **Expected Behavior:**  
  The chatbot will always give short, fixed responses exactly as instructed, without improvisation.  
- **Application:**  
  Useful for FAQs like order delivery dates, store timings, refund policies, etc.  

***

### 2. **Contextual Prompting**  
- **Explanation:**  
  Here, the chatbot remembers **previous parts of the conversation** and uses them while responding. This helps in creating continuity and avoids repetitive queries.  
- **Detailed Example:**  
  If customer earlier said: *“I haven’t received my order.”*  
  Prompt: *“I see that you mentioned your order hasn't arrived yet. Let me check the details for you.”*  
- **Expected Behavior:**  
  The chatbot tailors its answer using the customer’s earlier concern.  
- **Application:**  
  Customer support where following up or context is critical (e.g., missing deliveries).  

***

### 3. **Persona-Based Prompting**  
- **Explanation:**  
  The chatbot takes on a specific **personality or role** to sound more natural, friendly, or professional. Makes interaction engaging and relatable.  
- **Detailed Example:**  
  Prompt: *“Pretend you are a polite and friendly customer service rep. Say things like: ‘Hey there, no worries! Let’s sort this out together.’”*  
- **Expected Behavior:**  
  Replies become warm, conversational, and empathetic instead of robotic.  
- **Application:**  
  Customer-facing chatbots where user experience matters, e.g., e-commerce, hospitality, tech support.  

***

### 4. **Few-Shot Prompting**  
- **Explanation:**  
  The chatbot is trained using **few examples (shots)** so it learns how to generalize for similar inputs.  
- **Detailed Example:**  
  - Input: *“My phone isn’t charging.” →* Output: *“Have you tried using a different cable?”*  
  - Input: *“The screen is flickering.” →* Output: *“Try restarting the device, it may solve it.”*  
  - New Query: *“My app keeps crashing.” →* Chatbot predicts a similar solution based on examples.  
- **Expected Behavior:**  
  Responds correctly to new but related problems without being explicitly told.  
- **Application:**  
  Technical troubleshooting for devices, apps, or software support.  

***

### 5. **Chain-of-Thought Prompting**  
- **Explanation:**  
  This helps the chatbot to “think step-by-step” instead of giving one-shot answers. Perfect for logical problems and multi-step troubleshooting.  
- **Detailed Example:**  
  User: *“My laptop fan is making a loud noise.”*  
  Chatbot Reasoning:  
  1. Ask user if laptop is placed on soft surface (like bed).  
  2. Suggest moving it to a flat, hard surface for better ventilation.  
  3. Ask if vents are dusty → recommend cleaning.  
  4. Finally, suggest restart or service check if noise continues.  
- **Expected Behavior:**  
  Provides structured, guided troubleshooting steps rather than one vague answer.  
- **Application:**  
  Technical issue resolution, customer DIY guides, help desks.  

***

### 6. **Instruction with Constraints**  
- **Explanation:**  
  Chatbot is instructed to follow **restrictions** like word limit, no jargon, positivity, or polite tone.  
- **Detailed Example:**  
  Prompt: *“Respond to order inquiries in less than 50 words, avoid technical jargon.”*  
  Response: *“Your order is on the way and should arrive by [date]. Please reach out if you need any help.”*  
- **Expected Behavior:**  
  Keeps answers short, controlled, user-friendly, and compliant with restrictions.  
- **Application:**  
  SMS notifications, short replies, or contexts where formality and brevity are critical.  

***

### 7. **Reflective Prompting**  
- **Explanation:**  
  The chatbot **repeats/paraphrases the user’s query** before answering to confirm understanding.  
- **Detailed Example:**  
  User: *“How can I reset my password?”*  
  Chatbot: *“You’re asking how to reset your password, correct? Here’s how you can do it: …”*  
- **Expected Behavior:**  
  Reduces miscommunication, makes the customer feel heard, and confirms intent before solving.  
- **Application:**  
  Password resets, refunds, high-value transactions (critical cases where clarity matters).  

***
### output:

# Summary Table – Scenario-Based Report Development Using Prompting 

| **S. No** | **Prompting Technique** | **Objective** | **Example Prompt** | **Expected Behavior** | **Application** |
|-----------|--------------------------|---------------|--------------------|------------------------|-----------------|
| 1 | **Direct Instruction** | Provide short & fixed answers | `"When a customer asks for order status, reply: 'Your order is being processed and will be delivered by [date].'"` | Provides concise and predefined answers | FAQs like delivery time, policies |
| 2 | **Contextual Prompting** | Use earlier conversation context | `"If customer says order hasn’t arrived → 'I see you mentioned your order hasn't arrived. Let me check…'"` | Considers prior conversation for relevant answers | Late delivery support |
| 3 | **Persona-Based Prompting** | Simulate friendly/helpful character | `"Pretend you are a friendly customer representative: 'Hey there! I’m here to help…'"` | Adopts warm & conversational tone | E-commerce / Hospitality bots |
| 4 | **Few-Shot Prompting** | Learn from few examples to generalize | `"Phone not charging → Try another cable. Screen flickers → Restart device. Now solve: 'App crashing.'"` | Generalizes & solves based on given examples | Technical troubleshooting |
| 5 | **Chain-of-Thought Prompting** | Step-by-step reasoning | `"Laptop overheating → Check surface → Clean vents → Restart. Now solve: 'Fan making noise.'"` | Gives logical, structured troubleshooting | IT / Device support |
| 6 | **Instruction with Constraints** | Responses follow specific rules | `"Answer order queries in <50 words, no jargon: 'Your order is on the way and should arrive by [date].'"` | Short, rule-bound & easy to read | SMS updates & concise replies |
| 7 | **Reflective Prompting** | Confirm query before answering | `"User: How to reset password? → Bot: 'You're asking how to reset password, correct? Here’s how…'"` | Avoids misunderstanding by confirming intent | Password resets, refunds |

---


### Result: 

The **Prompt System** was successfully implemented and tested using **seven different prompting techniques**:  

1. **Direct Instruction** – ensured concise and fixed responses.  
2. **Contextual Prompting** – allowed continuity by remembering user’s previous queries.  
3. **Persona-Based Prompting** – enabled the chatbot to adopt a friendly, customer-oriented tone.  
4. **Few-Shot Prompting** – helped the chatbot generalize solutions from given examples.  
5. **Chain-of-Thought Prompting** – structured responses into logical, stepwise troubleshooting.  
6. **Instruction with Constraints** – produced short, clear, and rule-compliant answers.  
7. **Reflective Prompting** – confirmed user queries before giving solutions, ensuring clarity.  

***

### Final Outcome:  
- All **prompting strategies were executed successfully**.  
- The chatbot was able to handle **order tracking, troubleshooting, and general inquiries**.  
- The system demonstrated **improved flexibility, user-friendliness, reasoning ability, and contextual awareness.**  

**Thus, the Prompt System was executed successfully, achieving the intended objectives.**  

***




# Result: Thus the Prompts were exected succcessfully .




# Ex-4: Scenario-Based Report Development Utilizing Diverse Prompting Techniques

## Aim

The aim of this experiment is to build and analyze an AI-powered chatbot for a retail brand. The chatbot should be capable of answering product-related questions, handling complaints, and improving customer experience. Diverse prompting methods are tested to identify which technique performs best in realistic customer service scenarios.

---

## Introduction

Retail customers today expect fast and accurate responses about product availability, order status, and complaint handling. AI-powered chatbots are essential because they work 24/7, reduce workload on human agents, and provide consistent service. However, the performance of such chatbots depends heavily on the type of prompting technique used.

This report evaluates different prompting strategies such as zero-shot, few-shot, role-based, chain-of-thought, and reflective prompting. Two realistic scenarios are designed: **Product Inquiry** and **Complaint Handling**, to compare chatbot performance.

---

## Scenario 1: Product Inquiry

**Situation:** A customer, Priya, wants to know if the “Blue Denim Jacket” is available in size M and whether any discounts apply.

**Chatbot Requirements:**

* Understand product name and requested size.
* Check inventory.
* Confirm discount availability.
* Provide a clear, customer-friendly reply.

### Prompting Techniques Applied

* **Zero-Shot:** The chatbot directly answered the query without context. It gave a very generic reply such as “Please check the product page for offers.” This was incomplete and not customer-friendly.
* **Few-Shot:** With two examples of past queries, the chatbot learned to structure its response better. It replied: “Yes, the Blue Denim Jacket is available in size M. There is a 10% discount.” This was accurate but lacked brand tone.
* **Role-Based:** The chatbot was assigned the role of a retail assistant for Chic & Co. The reply became warmer: “Hello Priya! Yes, the jacket is in stock in size M and comes with a 10% discount. Would you like me to add it to your cart?” The output was friendly and professional.
* **Chain-of-Thought:** By reasoning step by step, the chatbot checked stock, confirmed size, verified discounts, and gave a structured response: “The jacket is available in size M with a 10% discount, and you can save money if you order today.” This was the most complete answer.
* **Reflective Prompting:** The chatbot generated a response, self-evaluated it, and revised to make it more polite and accurate. It confirmed both availability and discount, while keeping a helpful tone.

**Performance Table – Product Inquiry**

| Technique        | Accuracy | Relevance | Personalization | Customer Experience |
| ---------------- | -------- | --------- | --------------- | ------------------- |
| Zero-Shot        | ★★☆☆☆    | ★★☆☆☆     | ★☆☆☆☆           | ★★☆☆☆               |
| Few-Shot         | ★★★★☆    | ★★★★☆     | ★★★☆☆           | ★★★★☆               |
| Role-Based       | ★★★★☆    | ★★★★☆     | ★★★★☆           | ★★★★☆               |
| Chain-of-Thought | ★★★★★    | ★★★★★     | ★★★★☆           | ★★★★★               |
| Reflective       | ★★★★☆    | ★★★★★     | ★★★★☆           | ★★★★☆               |

---

## Scenario 2: Complaint Handling

**Situation:** A customer, Arjun, complains that his order for “Sports Running Shoes” has been delayed by three days. He is upset and wants a clear explanation and solution.

**Chatbot Requirements:**

* Acknowledge frustration and apologize.
* Identify cause of delay.
* Provide a revised delivery date.
* Offer escalation or compensation.

### Prompting Techniques Applied

* **Zero-Shot:** The chatbot gave a vague reply such as “Your order might be delayed due to shipping. Please wait.” This lacked empathy and accuracy.
* **Few-Shot:** With example complaints provided, the chatbot improved: “I’m sorry your order is delayed, Arjun. Please share your order number so I can check.” Better tone, but not detailed.
* **Role-Based:** As a polite assistant, the chatbot said: “I sincerely apologize, Arjun. Your order was delayed at the shipping hub but is now in transit. It will arrive in 3 days.” This was empathetic and professional.
* **Chain-of-Thought:** The chatbot reasoned step by step: acknowledged frustration, explained the sorting hub issue, provided a revised delivery date, and offered a token apology voucher. This was the best overall output.
* **Reflective Prompting:** The chatbot revised its first draft to ensure empathy and completeness. It confirmed the delay reason, gave a new date, and offered a link for tracking. This made the customer feel reassured.

**Performance Table – Complaint Handling**

| Technique        | Accuracy | Relevance | Personalization | Customer Experience |
| ---------------- | -------- | --------- | --------------- | ------------------- |
| Zero-Shot        | ★★☆☆☆    | ★★☆☆☆     | ★☆☆☆☆           | ★☆☆☆☆               |
| Few-Shot         | ★★★☆☆    | ★★★★☆     | ★★★☆☆           | ★★★☆☆               |
| Role-Based       | ★★★★☆    | ★★★★☆     | ★★★★☆           | ★★★★☆               |
| Chain-of-Thought | ★★★★★    | ★★★★★     | ★★★★☆           | ★★★★★               |
| Reflective       | ★★★★☆    | ★★★★★     | ★★★★☆           | ★★★★☆               |

---

## Comparative Analysis

Across both scenarios, **zero-shot prompting consistently failed** to meet customer expectations, while **few-shot prompting** improved the structure but lacked depth. **Role-based prompting** gave the chatbot a brand personality, improving professionalism and trust. **Chain-of-thought prompting** provided the most accurate, complete, and empathetic responses, making it the best technique overall. **Reflective prompting** was also effective, especially in ensuring customer-friendly tone and completeness.

---

## Results
The chatbot was tested with **diverse customer queries** (e.g., product availability, return policy, personalized recommendations). Each prompting technique produced different levels of performance:

1. **Zero-Shot Prompting**

   * Responses were **generic** and sometimes lacked accuracy.
   * Suitable for simple queries but failed in complex scenarios.

2. **Few-Shot Prompting**

   * Improved performance with relevant examples.
   * Responses were **more structured and contextually accurate**.

3. **Role-Based Prompting**

   * Chatbot maintained a **consistent persona** as a retail assistant.
   * Increased **user trust** and **professional tone** in responses.

4. **Chain-of-Thought Prompting**

   * Provided **step-by-step reasoning** before final answers.
   * Worked well for order tracking, troubleshooting, and decision-making queries.

5. **Scenario-Driven Prompting**

   * Delivered the **best overall results**.
   * Handled customer complaints and inquiries with **context awareness** and **personalization**.

**Performance Comparison Table**

| Prompting Technique | Accuracy | Relevance | Personalization | User Experience | Overall Effectiveness |
| ------------------- | -------- | --------- | --------------- | --------------- | --------------------- |
| Zero-Shot           | ★★☆☆☆    | ★★☆☆☆     | ★☆☆☆☆           | ★★☆☆☆           | Low                   |
| Few-Shot            | ★★★★☆    | ★★★★☆     | ★★★☆☆           | ★★★★☆           | High                  |
| Role-Based          | ★★★★☆    | ★★★★☆     | ★★★★☆           | ★★★★☆           | High                  |
| Chain-of-Thought    | ★★★★☆    | ★★★★☆     | ★★★☆☆           | ★★★★☆           | High                  |
| Scenario-Driven     | ★★★★★    | ★★★★★     | ★★★★★           | ★★★★★           | Very High             |

---

## Conclusion

* The experiment demonstrated that **different prompting techniques lead to different chatbot behaviors** in a retail customer support setting.
* **Zero-shot prompting** is fast but lacks depth and personalization.
* **Few-shot prompting** significantly improves response accuracy by providing examples.
* **Role-based prompting** ensures professionalism and a consistent chatbot persona.
* **Chain-of-thought prompting** is effective for complex reasoning tasks like order tracking.
* **Scenario-driven prompting** outperformed all others by combining **context-awareness, personalization, and user satisfaction**.

 **Final Inference:** Scenario-driven prompting is the most effective method for developing AI-powered chatbots in retail environments, as it delivers accurate, context-sensitive, and customer-friendly responses.

---

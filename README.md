Here's a comprehensive `README.md` for your **O-Range Customer Support Bot**:

---

**O-Range Customer Support Bot**

O-Range's Customer Support Bot is an intelligent chatbot designed to assist customers with troubleshooting, billing inquiries, and product information. It leverages the Hugging Face API for advanced intent classification and provides step-by-step guidance for resolving issues effectively.

---

**Features**
1. **Dynamic Intent Recognition**:
   - Classifies user input into intents like troubleshooting, billing, or product inquiry using Hugging Face's `facebook/bart-large-mnli` model.

2. **Step-by-Step Guidance**:
   - Troubleshoots product issues with a multi-step process, including diagnostics, inspections, and escalation protocols.
   - Resolves billing discrepancies with detailed bill reviews and escalation if necessary.

3. **Comprehensive Product Information**:
   - Provides detailed descriptions, pricing, and customization options for juices, cakes, and smart devices.

4. **Context-Aware Conversations**:
   - Retains context to manage multi-step interactions without reclassification.

5. **Fallback Handling**:
   - Handles unclear queries gracefully with rephrasing prompts or escalation.

---

**Prerequisites**
1. **Python 3.7+**
2. **Required Libraries**:
   - Install dependencies with:
     ```bash
     pip install requests
     ```

3. **Hugging Face API Token**:
   - Create an account on [Hugging Face](https://huggingface.co/).
   - Generate an API token from your account settings.
   - Replace `YOUR_HUGGING_FACE_API_TOKEN` in the code with your token.

---

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/orange-customer-support-bot.git
   cd orange-customer-support-bot
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up the Hugging Face API token:
   - Open `bot_logic.py` and replace with your API token.

**Usage**
1. Run the chatbot script:
   ```bash
   python bot_logic.py
   ```

2. Start interacting with the bot:
   - Type your queries, and the bot will classify your intent and respond appropriately.
   - Type `exit` or `quit` to end the session.

**Example Interaction**
**Scenario 1: Troubleshooting a Smart Thermostat**
**User**: "I need help with my thermostat."  
**Bot**: "Thank you for contacting O-Range. Could you please provide your order number or registered phone number for verification?"

**User**: "12345"  
**Bot**: "Are you facing specific issues, such as connectivity problems with your O-Range smart thermostat?"

**User**: "Yes, it won't connect to Wi-Fi."  
**Bot**: "If possible, test the device in another room or with a different Wi-Fi network to rule out network-related issues."

**Scenario 2: Billing Inquiry**
**User**: "I have an issue with my bill."  
**Bot**: "Thank you for contacting O-Range. Could you please provide your account number for verification?"

**User**: "98765"  
**Bot**: "Could you specify which charges on your bill you find incorrect or wish to dispute?"

**User**: "The last charge seems too high."  
**Bot**: "Please log in to your account portal to review the detailed bill. This will help us identify any discrepancies."

**Scenario 3: Product Inquiry**
**User**: "Tell me about your cakes."  
**Bot**:
Our cakes include:
- Classic Orange Pound Cake: Small ($12.99), Medium ($18.99), Large ($24.99).
- Chocolate-Orange Fusion Cake: Medium ($22.99), Large ($29.99).
- Orange Cheesecake: Slice ($4.99), Whole ($29.99).
Customizations are available!

**Customization**
- Add or modify intents and their responses in the `response_mapping` or the product details sections.
- Extend functionality by integrating additional APIs or databases for live updates.


**Future Improvements**
1. **Add Voice Interaction**:
   - Integrate speech-to-text and text-to-speech capabilities for enhanced usability.
2. **Database Integration**:
   - Store and retrieve user data for personalized recommendations.
3. **Frontend Deployment**:
   - Build a web or mobile interface for the chatbot.

**License**
This project is licensed under the MIT License. Feel free to modify and distribute.

**Contact**
For queries or support, contact us at:
- Email: support@orange.com
- Phone: 1-800-ORANGE
- Website: [www.orange.com](https://www.orange.com)

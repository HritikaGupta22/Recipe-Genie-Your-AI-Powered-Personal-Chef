# Recipe-Genie-Your-AI-Powered-Personal-Chef
Recipe Genie is an AI-powered recipe advisor designed to provide personalized dish recommendations and detailed cooking instructions. Whether you're craving something spicy, healthy, or quick, Recipe Genie tailors recipes based on your cuisine preferences, dietary needs, and cooking experience.

### 🛠️ Model 
- **Base Model:** `llama3.2:latest`  
- **Platform:** [OpenWebUI](https://openwebui.com/m/hritika/recipe-genie)
![image](https://github.com/user-attachments/assets/9cb1ed83-ba6c-40d8-a233-eea62bf88cbd)

- **Model Type:** Large Language Model (LLM) optimized for natural language processing and conversational AI.


### Features
✅ **Personalized Dish Recommendations** – Get suggestions based on your taste, cuisine, and dietary preferences.
✅ **Full Recipe Details** – Ingredients, cooking time, and step-by-step instructions.  
✅ **Smart Adaptation** – Suggests ingredient swaps for allergies and dietary needs.  
✅ **Quick & Easy Meals** – Get fast meal ideas for busy schedules.  
✅ **Beginner-Friendly** – Easy-to-follow instructions for all skill levels.  

### About the Model (Llama 3.2: Latest)  
Recipe Genie is built using **Llama 3.2**, a state-of-the-art LLM designed for efficient and context-aware interactions. Llama 3.2 offers:  
- **Improved NLP capabilities** for generating human-like text.  
- **Fast and efficient processing** for real-time recipe recommendations.  
- **Better contextual understanding** to refine user requests and personalize results.

### System Prompt
```
You are Recipe Genie, an AI-powered recipe advisor designed to provide personalized dish suggestions and detailed recipes. Your goal is to engage users by understanding their food preferences and recommending the best dishes accordingly.

Behavior & Flow:

    Country Selection:
        - Before anything else, ask the user which country they are from or which cuisine they prefer.
        - Adjust all suggestions and recommendations based on the selected country.

    Food Preferences Inquiry:
        - When a user asks for a dish suggestion, first ask:
            - What type of food they are in the mood for (e.g., spicy, sweet, healthy, comfort food, high-protein, etc.).
            - Which cuisine or locality they prefer (if different from the selected country).
        - If the user is unsure, suggest some categories to help them decide.

    Dish Recommendation:
        - Based on their input, suggest a few dishes that match their preference.
        - Provide a short description of each dish, including key ingredients and why it fits their request.
        - If needed, ask follow-up questions to refine the recommendation (e.g., vegetarian/non-vegetarian, dietary restrictions).

    Direct Recipe Response:
        - If the user directly asks for a specific dish recipe, provide the full recipe immediately without asking additional questions.
        - The response should include:
            - Ingredients (with quantities).
            - Cooking time.
            - Preparation and cooking steps.
            - Special tips or variations for different tastes.

    Interactive & Smart:
        - If the user has dietary restrictions or allergies, suggest alternatives.
        - If the user asks for a quick meal, prioritize fast and easy recipes.
        - If the user is a beginner, suggest simple recipes with detailed explanations.
```

## How to Install & Run Recipe Genie

**1️ Install OpenWebUI**
Ensure you have Docker and Docker Compose installed.

🔹 Install Docker & Docker Compose (if not installed)
```
sudo apt update && sudo apt install -y docker.io docker-compose
```

Then, clone and run OpenWebUI:
```
git clone https://github.com/openwebui/openwebui.git
cd openwebui
docker-compose up -d
```
This starts OpenWebUI in the background.


**2 Place the Downloaded JSON Model in the Correct Directory**
- Locate your downloaded JSON model file (e.g., recipe_genie.json).
- Move the file to the correct OpenWebUI models directory.
```
mv /path/to/downloaded_model.json ~/openwebui/models/
```
Replace /path/to/downloaded_model.json with the actual path of the file.


**3. Load the Model in OpenWebUI**


🔹 Open OpenWebUI in a Browser
- Open http://localhost:3000 in your browser.
- Go to Settings → Models.
- Click "Import Model" and upload the JSON file.

**4: Activate and Use the Model**
🔹 Select the Model in OpenWebUI
- Navigate to Chat Interface or API Playground.
- Select the uploaded model from the dropdown.
- Start chatting with your AI model! 

## Conversation


## Learnings:  
**1 Understanding LLaMA 3.2 Capabilities**: LLaMA 3.2 is a powerful language model with strong contextual understanding. Temperature tuning helps balance accuracy and creativity in responses.

**2️ System Prompt Engineering**: A well-structured system prompt ensures the AI follows a clear interaction flow, improves response quality, and adapts to user preferences effectively.

**3️ Model Deployment in OpenWebUI**: OpenWebUI simplifies AI model hosting, allowing easy customization of prompts and configurations without modifying the core model.

**4️ Fine-Tuning for Better Results**: Experimenting with temperature settings and structured prompts enhances response relevance, creativity, and engagement.

**5️ Handling Edge Cases & User Inputs**: Asking clarifying questions improves recommendation accuracy, ensuring responses are tailored to user preferences and dietary needs.

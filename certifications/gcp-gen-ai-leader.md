# GCP Generative AI Leader Certification Notes

This is my personal notes that I have created as a part doing [Google Cloud Generative AI Leader Certification](https://cloud.google.com/learn/certification/generative-ai-leader), taken during following the Cloud Skills Boost Generative AI Leader path.

**Overview:**

- Fundamentals of Generative AI (~30%): Understanding basic concepts and definitions related to AI and ML.
- Google Cloud's Generative AI Offerings (~35%): Familiarity with Google Cloud tools and services that support generative AI.
- Techniques to Improve Model Output (~20%): Knowledge of methods to enhance the performance of generative AI models.
- Business Strategies for Successful Gen AI Solutions (~15%): Strategies for implementing generative AI in business settings.


**Resources:**

-   [Exam Guide](https://services.google.com/fh/files/misc/generative_ai_leader_exam_guide_english.pdf)
-   [Study Guide](https://services.google.com/fh/files/misc/generative_ai_leader_study_guide_english.pdf)
-   [Google Cloud Skills Boost](https://www.cloudskillsboost.google/paths/1951)


## Fundamentals of Generative AI (Additional Notes other than mentioned in Resources)
-   Gen AI often involves Advanced machine learning techniques:
    -   GANs: Generative Adversarial Networks
    -   VAEs: Variational Autoencoders
    -   Transformer Models Eg: GPT (Generative Pre-Trained Transformer)
-   Gen AI has multiple modalities
    -   Vision: realistic images and videos
    -   Text: generating human-like text
    -   Audio: composing music
    -   Molecular: Drug discovery via genomic data


## 1. Generative AI Leader Path

### [Gen AI: Beyond the ChatBot](https://www.skills.google/paths/1951/course_templates/1268/documents/606734)

-   Responsible AI:
    -   Secure AI Framework (SAIF): A comprehensive suite of tools and best practices for building secure AI systems.
    -   Mandiant: Leverage Mandiant's threat intelligence and expertise to protect your AI systems from cyberattacks.
    -   AI Principles: Google's published AI Principles guide the development and deployment of AI technologies.
    -   Responsible AI Toolkit: Resources and tools to help developers and organizations build AI systems that are fair, unbiased, and socially beneficial.


-   Building a successful gen AI strategy:
    Successful gen AI implementation requires a combination of top-down and bottom-up approaches. For both approaches, you want to be strategizing on:
    -   Strategic focus
    -   Exploration
    -   Responsible AI
    -   Resourcing
    -   Impact
    -   Continuous improvement

-   Brainstorm gen AI use cases
    -   Creative Matrix method

-   Augmentation versus Automation (Keeping humans at the forefront of genai implementation)
    Augmentation:
    -   Critical thinking and problem solving
    -   Creativity and Innovation
    -   Relationship building and collaboration
    -   Stategic planning and vision:

    Automation:
    -   Repetitive and rule-based: data entry, information retrieval, content formatting, and basic code generation.
    -   Time consuming and resource-intensive: research, data analysis, content summarization, and initial draft creation



### [GENAI: Unlock Foundational Concepts](https://www.skills.google/paths/1951/course_templates/1265/documents/607925)
-   Data:
    -   Data Quality
        -   Accuracy
        -   Completeness
        -   Representative
        -   Consistency
        -   Relevance

-   Deep Learning:
    -   Neural networks can leverage both labeled and unlabeled data, a strategy known as semi-supervised learning.

-   Large language models (LLMs)​​​
    -   One particularly exciting type of foundation model is the LLM. These models are specifically designed to understand and generate human language. 

-   Diffusion models
    -   Diffusion models are another type of foundational model. They excel in generating high-quality images, audio, and even video by iteratively refining noise (or unstructured/random data and patterns) into structured data.

-   Steps involved in turning data into learning using google cloud
    -   Gather your data
    -   Prepare your data
    -   Train your model
    -   Deploy and predict
    -   Manage your model


-   Factors when choosing a model for your use case
    -   Modality
    -   Context Window
    -   Security
    -   Availability and Reliability

    -   Cost
    -   Performance: Accuracy, Speed, Efficiency
    -   Fine tuning and Customization
    -   Ease of Integration

-   Techniques to improve foundation model limitations
    -   Grounding
    -   Human in the Loop (HITL)

-   Secure AI
    -   Apply Secure AI Framework (SAIF)

-   Responsible AI
    -   Ensuring AI applications avoid intentional and unintentional harm
    -   Important to consider ethical development and positive outcomes for the software you develop


### [GENAI: Navigate the Landscape](https://www.skills.google/paths/1951/course_templates/1261/documents/608406)
-   Building blocks of generative AI
    -   GEN AI Applications (User facing layer)
    -   Agents (Layer that interacts with the environment, gathers info and makes decision)
    -   Platform (Helps with tools and services that help building and deploying AI models.Includes model training platforms like Vertex AI and data management tools)
    -   Models (Brain of AI system reside, comprises of algorithms and learn patterns from data and generate new content, Like LLMs like Gemini, Image recognition models)
    -   Infrastructure (Comprising of Hardware, like Physical servers, TPUs and GPUs that provide computational power.)

-   What can agents do ..?
    -   Understanding and responding to natural language
    -   Automating complex tasks
    -   Personlization

-   How agents work:
    > Broadly there are two categories of agents
    -   Conversatational
        > Conversational agents are designed to understand what you mean, not just what you say, and respond in a way that makes sense.
    -   Workflow Agents
        > Workflow agents are designed to streamline your work and make sure things get done efficiently and correctly by automating tasks or going through complex processes.

-   Agents
    -   Reasoning Loop
        > Continous iterative process of consisting of Observes, Interprets, Plans and Acts
        > Reasoning loop often utilizes advances prompt engineering frameworks
        -   Simple rule-based calculations
        -   Complex thought chains
        -   Machine learning algorithms
        -   Probabilistic reasoning techniques
        > Examples: ReAct, Chain of Thought (CoT) Prompting
    -   Tools
        > Ex: Access and update company inventory

-   Platform Layer
    > Features and Benefits of Vertex AI
        -   Open and Flexible
        -   Powerful Infrastructure
        -   Pre-Trained Models
        -   Comprehensive Tooling
        -   Customization
        -   Easy Integration
    > Vertex AI also includes ML operations (MLOps) tools built in to help you orchestrate end-to-end ML workflows, perform feature engineering, run experiments, manage and iterate your models, track ML metadata, and monitor and evaluate model quality. 
    -   Feature Store
    -   Model Registry
    -   Model Evaluation
    -   Workflow Orchestration
    -   Model Monitoring

-   Model Layer
    > Vertex AI:A model hub (Use models with Model Garden)

-   Infrastructure Layer

-   AI on the Edge
    > Eg: Google Nano (miniature model)
    > Convert your models to Lite Runtime (LiteRT) for optimal performance on edge devices.

-   People, Cost and Time
    -   Cost
    >   You pay for three primary activities
        -   Training
        -   Deploying
        -   Using
    - Pricing
        -   Usage-based
        >   You pay for the amount you use, often measured in tokens or characters processed. This is common for APIs like Google’s PaLM & Gemini APIs.
        -   Subscription-based
        >   You pay a recurring fee for access to the model, often with tiers based on usage limits or features.
        -   Licensing fees
        >   One-time or recurring fees for using a model, especially for commercial purposes or embedding in products.

    - Pricing metrics
        -   Tokens: A token represents a piece of text, like a word or part of a word.
        -   Characters: Some providers, like Google, charge based on the number of characters processed.
        -   Requests: Sometimes you can be charged per request, regardless of the complexity or volume of the task.
    -   Factors affecting cost
        -   Model, size and complexity
        -   Context Window
        -   Features
        -   Deployment

-   GEN AI Solution Needs
    -   Scale
    -   Customization
        -   Start with existing models
        -   Identify your unique needs
        -   Consider data specifity
        -   Consider task complexity
    -   User Interaction 
        -   UI and UX
    -   Privacy
        -   Data Security
        -   Compliance
    -   Other Considerations
        -   Latency
        -   Connectivity
        -   Accuracy
        -   Explainability

-   Choosing and Maintaining your GEN AI Solution
    -   Model monitoring and retraining
    -   Data updates
    -   Software updates and bug fixes
    -   Hardware and Infrastructure
    -   Security and Compliance



### [GENAI APPs: Transform your work](https://www.skills.google/paths/1951/course_templates/1266/documents/607882)

-   Google Workspace with Gemini
    -   Gemini Side Panel
    -   Gemini in Gmail
    -   Gemini in Google Docs
    -   Gemini in Google Slides
    -   Gemini in Google Sheets
    -   Gemini in Google Meet

-   Prompting Techniques
    -   Zero-shot promting: 
    -   One-shot prompting
    -   Few-shot prompting
    -   Role prompting
    -   Prompt chaining
        >   Set a goal -> Start the chain -> Build the chain -> Observe and analyze -> Reflect and share

-   Reusing prompts with Gemini and Gems
    -   Gemini Advanced
    -   Gems

-   How Gems Work
    -   Personalized Responses
    -   Streamlined Workflows
    -   Reset Context

-   Grounding and RAG
    -   Grounding
        >   For example, you can create a Gemini prompt that helps you refine your writing by editing your text to meet your organization’s specific guidelines and standards. You can provide Gemini with resources, such as your company’s style guides within the prompt itself, or by uploading relevant files.
    -   RAG (Retrieval-Augmented Generation)
        >   One powerful grounding technique is retrieval-augmented generation (RAG). It involves:
        
        -   Retrieving Relevant Information
            >    The AI model first retrieves relevant information from a vast knowledge base (like a database, a set of documents, or even the entire web). This retrieval process is often powered by sophisticated techniques, like semantic search or vector databases.
        -   Generating Output
            >   The model then uses this retrieved information to generate the final output. This could be anything from answering a question to writing a creative story.
        
        Benefits of RAG
        -   Improved Accuracy and relevance
        -   Improved explainability and transparency
        -   Extending LLM Capabilities

-   NotebookLM
    >   NotebookLM is an AI-first notebook, grounded in your own documents, designed to help you gain insights faster.

    Advanced versions of NotebookLM
    -   NotebookLM Plus
    -   NotebookLM Enterprise

    NotebookLM versus Gems
    -   Hyper-focused knowledge
    -   Interactive Learning
    -   Source-based answers

    Use Cases
    -   Create training materials and documentation
    -   Researching a new topic
    -   Learn by listening to audio
    -   Preparing for a presentation
    -   Summarize documentation
    -   Project proposals and plans

-   Gemini for Google Cloud
    -   Gemini Cloud Assist
    -   Gemini in BigQuery
    -   Gemini Code Assist
    -   Gemini Colba Enterprise
    -   Gemini in Databases
    -   Gemini in Looker
    -   Gemini in Security

    Increased agility, Improved collaboration, Enhanced Data Literacy


### [GENAI Agents: Transform your organisation](https://www.skills.google/paths/1951/course_templates/1267/documents/607947)
-   Using Models
    -   Token Count
    -   Temperature: Controls the creativity
    -   Top-p(nucleas sampling): Controls the randomness during text generation
    -   Safety Settings: allow you to filter our potentially harmful inappropriate content
    -   Output length: Max length of generated text

-   Gen AI APIs
    -   Google AI Studio
    -   Vertex AI Studio

-   Parameter Playground

-   Adding Prompt Engineering to your reasoning loops
    -   Key aspects of the reasoning loop
        -   Iterative process
        -   Internal reasoning
        -   Decision making
        -   Reasoning frameworks

-   Prompt Engineering techniques
    -   ReAct Prompting
        >   ReAct is a prompting framework that allows the language model to reason and take action on a user query, with or without in-context examples.
    
        ReAct Key Features
        -   Dynamic problem solving
        -   Reduced Hallucination
        -   Increased Trustworthiness
    
        Key componennts of ReAct
        -   Think
        -   Act
        -   Observe
        -   Respond

        ReAct in Action
        -   Question answering
        -   Fact Verification
        -   Decision making
    
    -   Chain of Thought(CoT) prompting
        >   Chain-of-thought prompting is a technique where you guide a language model through a problem-solving process by providing examples with intermediate reasoning steps, helping it learn to approach new problems in a more structured and logical way.

        CoT Key Features
        -   Improved reasoning
        -   Better accuracy
        -   Enhanced explainability

        Key components of CoT
        -   Self consistency
        -   Active prompting
        -   Multimodal CoT

        CoT in Action
        -   Complex reasoning tasks
        -   Explanation generation
        -   Multi-step planning
    
-   Types of Agent tools
    -   Extensions (APIs)
    -   Functions
    -   Data stores
    -   Plugins

-   Google's Agent Tools
    -   Cloud Storage
    -   Databases (CloudSQL, Spanner, Firestore)
    -   Cloud Run Functions
    -   Cloud Run
    -   Vertex AI

    Pre-Built AI APIs
        -   Speech-to-Text API
        -   Text-to-Speech API
        -   Translation API
        -   Document Translation API
        -   Document AI API
        -   Cloud Vision API
        -   Cloud Video Intelligence API
        -   Nature Language API
        -   there are many more other APIs (Ex: Google Maps and many more)

-   Building applications from Agents
    > Using multiple GCP services 
    -   Google AI Studio
    -   Vertex AI Studio
    -   Cloud Run Functions
    -   Cloud Run

-   RAG and tooling
    -   Retrieval
        -   Data Stores
            -   Websites
            -   Structured Data
                -   Tables, JSON Format
            -   Unstructured Data
                -   HTML, PDF, DOCX
        -   Vector Databases
        -   Search Engines
        -   Knowledge Graphs
    -   Augmentaion
        >   retrieved information is then incorporated (or "augmented") into the prompt that is fed to the LLM. This augmented prompt now contains both the user's original query and the relevant context retrieved from external sources. 
    -   Generation
        >   LLM processes the augmented prompt and generates a response. Because the prompt includes relevant external information, the LLM can generate a more informed, accurate, and contextually appropriate response. It can also cite the sources of its information, increasing transparency and trustworthiness.

-   Vertex AI Search
    -   Document Search
    -   Media Search
    -   Healthcare Search
    -   Search for commerence

    >   A key strength of Vertex AI Search lies in its ability to ground gen AI LLM responses with your first-party data, curated third-party data, and even Google's knowledge graph (Grounding with Google Search), minimizing "hallucinations" and ensuring trustworthy information.

    Recommendation Solutions
        -   Media recommendations
        -   Retail recommendations

-   Gen AI Customer Engagement
    -   Conversational Agents
        -   Chatbots
    -   Agent Assist
        -   Support live human contact centers
    -   Conversational Insights
        -   Gain insights into all your communications with customers (Chatbot agents or Human Agents)

    Contact center as a service (CCaaS)

-   Build your own agent
    -   Metaprompting
        >   Metaprompting is about creating prompts that guide the AI to generate, modify, or interpret other prompts
        >   Metaprompting is a powerful tool for interacting with AI, enabling more dynamic, flexible, and adaptable prompt creation and interpretation. It's a key technique for unlocking the full potential of large language models.

-   Gemini Enterprise

-   Plan for generative AI integration
    -   Establish a clear vision
    -   Prioritize high-impact use cases
    -   Invest in capabilities
    -   Drive Organizational charge
    -   Measure and demonstrate value
    -   Champion responsible AI

    Plan for impact
    Plan for change
    -   Regularly review and refine your strategy
    -   Stay informed
    -   Engage with the generative AI community
    -   Invest in traning and development
    -   Attract and retail top talent


    
    




        








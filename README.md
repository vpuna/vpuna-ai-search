# Vpuna AI Search

**Vpuna AI Search is a developer-first platform** that enables you to embed, index, and perform semantic search over structured and unstructured data using vector embeddings, with optional summarization powered by large language models (LLMs).

---

## 🚀 What is Vpuna AI Search?

Vpuna AI Search is a full-stack AI-native search infrastructure that enables developers to:

- Upload and index JSON, YAML, CSV, PDF, and DOCX
- Generate and store vector embeddings
- Query semantically and optionally summarize with LLMs
- Manage tenants, projects, and schemas through a secure developer console

---

## 🌐 Learn More

- 🌍 Website: [https://aisearch.vpuna.com](https://aisearch.vpuna.com)
- 📚 Docs: [https://aisearch.vpuna.com/docs](https://aisearch.vpuna.com/docs)
- ✨ Developer Console: [https://console.aisearch.vpuna.com](https://console.aisearch.vpuna.com)

---

## 📦 Architecture

Vpuna is built with:

- **Fastify (Node.js)** for embedding and search APIs
- **React + Radix UI** for console and public frontend
- **Docusaurus** for documentation
- **Supabase** for storage, auth, queues, pgvector, and edge functions
- **Traefik + Nginx** for container routing and web hosting

> [Read the full architecture overview](https://aisearch.vpuna.com/docs/architecture)

---

## 📦 Features

- **Signup / Login**
    - Signup and Login with Google, Github
    - Signup and Login with email (Coming Soon)   
- **System Setings**  
    - Account Managemet
        - Change Password for non social login (Coming Soon)
        - Delete Account
    - User Management
        - Assign users to tenants as Admin, Developer or Monitor
        - Assign users to projects as Admin, Developer or Monitor
- **Tenants**
    - Stats
        - Total Tenants, Total Projects, Total Files
    - Management
        - Manage Tenant - Create tenant, edit tenant, delete tenant
- **Tenant-Projects**
    - Stats
        - Total Projects, Total Files, Team Members 
    - Management
        - Manage project - Create project, edit project name and description, delete project
        - Manage API Keys - Create API Keys, assign permissons to search and embed apis, assign expiry date, revoke keys
        - Manage Embedding Service
            - Support for local CPU based Hugging Face Transformers. Only supports all-MiniLM-L6-v2 for now. Other Local model support is coming soon
            - Hugging Face Cloud (Coming Soon)
            - OpenAI (Coming Soon)
    

> [Read the full architecture overview](https://aisearch.vpuna.com/docs/architecture)

---

## 🔒 Licensing

This is a closed-source SaaS platform for now. Open source or open core licensing (Elastic or dual license) may be introduced later.

---

## 📫 Contact

Have a question or feedback?  
- Get in touch at [support@aisearch.vpuna.com](mailto:support@aisearch.vpuna.com)
- Please raise any issues or feature requests at [https://github.com/vpuna/vpuna-ai-search/issues](https://github.com/vpuna/vpuna-ai-search/issues)

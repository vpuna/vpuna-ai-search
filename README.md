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
- **System Setings**  (https://aisearch.vpuna.com/docs/ui-console/account-management)
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
        - Manage LLM Sevice (Coming Soon)
            - This feature allows users to configure local or cloud based LLM services for LLM summarization, chatbots etc. Think built in RAG
        - Manage MCP Server (Coming Soon)
            - Enable/Disable MCP server access. Use your search indexes to provide more context to your MCP Clients
- **Project**
    - Stats
        - Total Documents, Total Searches (Coming Soon), Total Users, Total Storage
    - File Management
        - Manage Confogurations
            - Manage ( create, edit and delete ) parsing jsonpath configuration to select Reference ID, Text to Index and Metadaa to store for API return data and filters.
            - Supported file types are txt, json object and json array files.
            - pdf, docx, csv, xslx ( Coming Soon)
            - Enrich technical numeric fields with additional context by selecting one or more felds and provide text context. (Coming Soon)
            - Customize ranking. Currently the results are ranked based on the similarity score. This feature will allow the users to overwrite the detail ranking based on any of the fields (Coming Soon)
        - Upload Files
            - Upload files with or wutiout associated configurations
            - Manually enter hard coded configurations if needed
            - Show Curl request to use the embed API based on an existing uploaded file from the developer console (Coming Soon)
            - Connect to other data sorces like databases, git repos, gmail, google drive etc and configure pooling (Coming Soon)
            - Configure OCR for PDFs and PPTX where the text are embedded in the images (Coming Soon)
        - Search Documents
            - Test search API along with metadata filters.
            - Show Curl request for the executed search API
            - Show search result in both UI and JSON form
- **APIs**
    - POST Search
        - https://aisearch.vpuna.com/docs/api/search-documents 
    - POST Embed
        - https://aisearch.vpuna.com/docs/api/embed-document
    - DELETE Embed
        - https://aisearch.vpuna.com/docs/api/delete-document
    

> [Read the full architecture overview](https://aisearch.vpuna.com/docs/architecture)

---

## 🔒 Licensing

This is a closed-source SaaS platform for now. Open source or open core licensing (Elastic or dual license) may be introduced later.

---

## 📫 Contact

Have a question or feedback?  
- Get in touch at [support@aisearch.vpuna.com](mailto:support@aisearch.vpuna.com)
- Please raise any issues or feature requests at [https://github.com/vpuna/vpuna-ai-search/issues](https://github.com/vpuna/vpuna-ai-search/issues)

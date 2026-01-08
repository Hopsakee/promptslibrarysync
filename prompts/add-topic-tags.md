---
title: "Add topic tags"
tags: ["learning"]
created: "2025-12-26T12:17:21.332Z"
updated: "2025-12-28T12:38:58.725Z"
version: 2
---

Your job is to categorize various types of documents including web articles, ebooks, PDFs, Twitter threads, and YouTube videos into one or more of the topic, project, and back-of-mind interest labels provided below.

"""
TOPIC TAGS:

Christianity & Religion:
Bible: Documents covering biblical texts, interpretation, exegesis, or biblical scholarship, including commentary, hermeneutics, and textual analysis of scripture.
Christianity: Documents covering Christian theology, church history, denominations, practices, or Christian thought, where the Bible may be a source but is not the primary subject.
Religion: Documents covering comparative religion, religious studies, or religions other than Christianity and Judaism, including Buddhism, Islam, Hinduism, and secular perspectives on religion.
Judaism: Documents covering Jewish theology, history, traditions, and texts such as the Talmud and Mishnah, including Jewish thought and practice.

Philosophy & Ideas:
Philosophy: Documents covering philosophical theories, ethics, epistemology, metaphysics, logic, or works by and about philosophers, providing insights into fundamental questions about existence, knowledge, and values.

Technical - Programming:
Python: Documents covering the Python programming language specifically, including syntax, libraries, frameworks, best practices, and Python-specific tooling.
Programming: Documents covering general software development, coding practices, languages other than Python, and software architecture, catering to developers and engineers.
Database: Documents covering database design, SQL, NoSQL, query optimization, and data modeling, offering guidance on storing and retrieving data effectively.
Cli: Documents covering command-line tools, shell scripting, and terminal workflows, including bash, zsh, and CLI application development.
ProductManagement: Documents covering product strategy, roadmaps, user stories, stakeholder management, and product lifecycle, catering to product managers and those building products.
Design: Documents covering UX design, visual design, information architecture, and UI patterns, providing guidance on creating effective user interfaces and experiences.

Technical - AI/ML:
GenerativeAI: Documents covering large language models, image generation, text-to-X models, and prompt engineering, including practical applications of generative AI (implies MachineLearning—do not double-tag).
RAG: Documents covering retrieval-augmented generation specifically, including vector databases, embeddings, chunking strategies, and hybrid search approaches.
AI-agents: Documents covering autonomous AI systems, agent architectures, tool use, and multi-agent systems, including frameworks for building AI agents.
AI-evals: Documents covering evaluation methods for AI systems, including benchmarks, testing methodologies, and safety assessments.
MachineLearning: Documents covering classical machine learning, neural networks, training methods, and model selection, excluding content primarily about generative AI.

Technical - Infrastructure:
Devops: Documents covering CI/CD, containerization, cloud infrastructure, deployment, monitoring, and infrastructure as code, catering to operations and platform engineers.
Security: Documents covering cybersecurity, privacy, authentication, encryption, threat modeling, and secure coding practices, providing guidance on protecting systems and data.

Data & Analysis:
DataScience: Documents covering applied data analysis, visualization, exploration, and practical data workflows, focusing on using data to solve real-world problems.
Math: Documents covering mathematical theory and methods, including statistics, probability, linear algebra, calculus, discrete math, and experimental design.

Work Domain:
WaterManagement: Documents covering hydrology, water systems, flood control, water treatment, and water policy, catering to water management professionals and researchers.
Business: Documents covering organizational management, strategy, leadership, and business operations, offering insights for professionals managing teams and organizations.

Social Sciences:
Economy: Documents covering economic theory, markets, fiscal and monetary policy, and economic systems, providing analysis of how economies function.
Politics: Documents covering political systems, governance, policy, political theory, and current affairs, offering perspectives on government and political dynamics.
Sociology: Documents covering social structures, culture, group behavior, and social institutions, providing insights into how societies function.
Psychology: Documents covering human behavior, cognition, mental processes, and therapeutic approaches, offering insights into the mind and behavior.
History: Documents covering historical events, periods, historiography, and historical analysis, providing insights into the past and its impact on the present.

Entities:
Person: Documents primarily about a specific individual, including biographical content, profiles, and interviews.
Organisation: Documents primarily about a specific company, institution, or organization, including company profiles and organizational analysis.
Product: Documents primarily about a specific product or service, including reviews, documentation, and product analysis.

Entertainment:
Literature: Documents covering fiction, poetry, literary analysis, and narrative works, including content about authors and literary movements.
Movie: Documents covering films, cinema, directors, and film analysis, catering to film enthusiasts and critics.
VideoGame: Documents covering video games, game design, game reviews, and gaming culture, catering to gamers and game developers.
Event: Documents covering conferences, festivals, and specific happenings, including event summaries and announcements.

Self:
Productivity: Documents covering personal effectiveness, time management, habits, and workflows, offering tips and tools for improving personal and professional productivity.
Health: Documents covering physical health, exercise, nutrition, sleep, and medical topics, providing guidance on maintaining a healthy lifestyle.
Learning: Documents covering learning methods, study techniques, pedagogy, and meta-learning, offering insights into how to acquire skills and/or knowledge effectively.

Communication:
Communication: Documents covering writing, presenting, public speaking, visual communication, and rhetoric, providing guidance on how to convey ideas effectively.

Other:
Place: Documents primarily about a specific geographic location, including travel guides, regional information, and location profiles.
Legislation: Documents covering laws, regulations, legal frameworks, and compliance, providing analysis of legal matters and their implications.

BACK OF MIND TAGS (Current Focus Areas - prefix with BOM_):

BOM_Progress: Documents covering how to recognize progress, celebrate small wins, track achievements, and develop a growth mindset, offering practical strategies for acknowledging steps forward.
BOM_Sabbath: Documents covering rest, Sabbath practices, letting go of the need to change the world, trusting God, and finding contentment in limitations, providing theological and practical guidance on rest.
BOM_GenAI_Learning: Documents covering using generative AI and large language models for personal projects and learning to program, including practical applications, tutorials, and AI-assisted development workflows.
BOM_Parenting: Documents covering raising children, parenting strategies, child development, and family dynamics, offering advice and insights for parents.
BOM_Family: Documents covering building and maintaining family relationships, quality time, connection, and shared experiences, providing ideas for strengthening family bonds.
BOM_Python_GUI: Documents covering building graphical user interfaces for Python applications, including frameworks like Tkinter, PyQt, Streamlit, and GUI design patterns.

"""

You select all categories from these lists that are covered in depth within this document. 

# Output format

- Apply topic tags without prefixes, back-of-mind tags with the BOM_ prefix.
- Only give the categories from these lists without any further explanation.
- Seperate each tag with a space " "
- Prepend each tag with a hash symbol "#"
- Write all tags with lowercase

VERY IMPORTANT: Return only the categories with their appropriate prefixes (BOM_) and nothing else.

**Example output**

#productivity #communication #BOM_Progress

# Content


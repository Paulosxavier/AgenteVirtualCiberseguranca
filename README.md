🔐 Agente Virtual de Cibersegurança com IA Generativa
Contexto
Os assistentes virtuais estão evoluindo de simples chatbots reativos para agentes inteligentes e proativos. Neste desafio, você vai idealizar e prototipar um Agente de Cibersegurança que utiliza IA Generativa para:

Ensinar técnicas de proteção digital de forma prática e acessível

Antecipar riscos e sugerir boas práticas de segurança

Cocriar soluções de defesa com base em cenários reais

Garantir respostas confiáveis e seguras (anti-alucinação)

📦 O Que Você Deve Entregar
1. Documentação do Agente
Defina o que seu agente faz e como ele funciona:

Caso de Uso: Apoiar usuários iniciantes em cibersegurança, ensinando boas práticas contra phishing, engenharia social, uso de MFA e proteção de dados.

Persona e Tom de Voz: Didático, claro e acessível, sem jargões excessivos.

Arquitetura: Fluxo de dados integrado a uma base de conhecimento com conceitos e exemplos de ataques.

Segurança: Evitar respostas inventadas e sempre indicar quando não houver informação suficiente.

📄 Template: docs/01-documentacao-agente.md

2. Base de Conhecimento
Organize informações confiáveis sobre cibersegurança. Exemplos de arquivos mockados:

Arquivo	Formato	Descrição
ataques.csv	CSV	Tipos de ataques (phishing, ransomware, DDoS)
boas_praticas.json	JSON	Recomendações de segurança (MFA, senhas fortes, backups)
historico_perguntas.csv	CSV	Perguntas frequentes de usuários
conceitos_basicos.md	Markdown	Definições de OSINT, DevSecOps, Engenharia Social


📄 Template: docs/02-base-conhecimento.md

3. Prompts do Agente
Documente os prompts que definem o comportamento do seu agente:

System Prompt: "Você é um assistente de cibersegurança. Responda de forma clara e objetiva, usando exemplos práticos. Se não tiver informação suficiente, diga isso e sugira uma fonte confiável."

Exemplos de Interação:

Usuário: "O que é phishing?"

Agente: "Phishing é uma técnica de engenharia social que engana usuários para revelar informações sensíveis. Exemplo: e-mails falsos que imitam bancos."

Tratamento de Edge Cases: Se o usuário pedir algo fora da base de conhecimento, o agente deve responder: "Não tenho informações suficientes sobre isso. Recomendo consultar fontes confiáveis como OWASP ou CERT."

📄 Template: docs/03-prompts.md

4. Aplicação Funcional
Desenvolva um protótipo funcional do seu agente:

Chatbot interativo (sugestão: Streamlit ou Gradio)

Integração com LLM (via API ou modelo local)

Conexão com a base de conhecimento

📁 Pasta: src/

5. Avaliação e Métricas
Defina como avaliar a qualidade do agente:

Precisão das respostas

Taxa de respostas seguras (sem alucinações)

Clareza e utilidade para iniciantes

📄 Template: docs/04-metricas.md

6. Pitch
Grave um pitch de 3 minutos apresentando:

Problema: Muitas pessoas não sabem se proteger contra ataques digitais.

Solução: Um assistente virtual que ensina técnicas de cibersegurança de forma prática.

Valor: Democratizar o acesso ao conhecimento em segurança digital.

📄 Template: docs/05-pitch.md

🛠️ Ferramentas Sugeridas
LLMs: ChatGPT, Copilot, Gemini, Claude, Ollama

Desenvolvimento: Streamlit, Gradio, Google Colab

Orquestração: LangChain, LangFlow, CrewAI

Diagramas: Mermaid, Draw.io, Excalidraw

📂 Estrutura do Repositório
Código
lab-agente-ciberseguranca/
│
├── README.md
│
├── data/                          # Dados mockados para o agente
│   ├── ataques.csv                 # Tipos de ataques
│   ├── boas_praticas.json          # Recomendações de segurança
│   ├── historico_perguntas.csv     # Perguntas frequentes
│   └── conceitos_basicos.md        # Definições e conceitos
│
├── docs/                          # Documentação do projeto
│   ├── 01-documentacao-agente.md   # Caso de uso e arquitetura
│   ├── 02-base-conhecimento.md     # Estratégia de dados
│   ├── 03-prompts.md               # Engenharia de prompts
│   ├── 04-metricas.md              # Avaliação e métricas
│   └── 05-pitch.md                 # Roteiro do pitch
│
├── src/                           # Código da aplicação
│   └── app.py                      # Protótipo do chatbot
│
├── assets/                        # Imagens e diagramas
│   └── ...
│
└── examples/                      # Referências e exemplos
    └── README.md

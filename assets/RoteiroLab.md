🎬 Vídeo 1: Introdução ao Desafio
Código
Fala, pessoal! Eu sou o Paulo e hoje vou apresentar pra vocês um desafio muito especial: criar um Agente Virtual de Cibersegurança usando IA Generativa.

Os assistentes virtuais estão evoluindo. Eles não são mais apenas chatbots que respondem perguntas prontas, mas agentes inteligentes e proativos. No setor de segurança digital, isso é ainda mais importante: precisamos de soluções que antecipem riscos, eduquem usuários e ajudem a tomar decisões seguras.

Neste desafio, você vai criar um agente que não apenas responde dúvidas, mas que ensina boas práticas de cibersegurança. Que alerta sobre riscos como phishing e engenharia social. Que ajuda pessoas a protegerem seus dados e a navegarem com mais segurança. E, muito importante: que evita alucinações — ou seja, não inventa informações.

O que você vai entregar?
São seis etapas principais:
1. Documentação do agente — caso de uso, persona, arquitetura e estratégias de segurança.
2. Base de conhecimento — com dados mockados ou públicos sobre cibersegurança.
3. Prompts do agente — o coração do comportamento da solução.
4. Aplicação funcional — um protótipo interativo.
5. Avaliação e métricas — como medir se o agente está funcionando bem.
6. Pitch final — apresentando sua solução de forma objetiva.

O mais importante é dar a SUA cara ao desafio. Use sua criatividade, explore suas ideias e se permita aprender fazendo.

Bora começar?
🎬 Vídeo 2: Etapa 1 — Documentação do Agente
Código
Aqui você define O QUE seu agente faz e COMO ele funciona.

Quatro pontos principais:
- Caso de Uso: qual problema de segurança ele resolve? Exemplo: ensinar boas práticas contra phishing e engenharia social.
- Persona e Tom de Voz: educativo, claro e acessível, sem jargões técnicos.
- Arquitetura: fluxo simples mostrando como o agente recebe a pergunta, consulta a base de conhecimento e responde.
- Segurança e Anti-Alucinação: o agente só responde com base nos dados fornecidos. Se não souber, admite e sugere fontes confiáveis.

Documentar bem no início evita retrabalho depois.
🎬 Vídeo 3: Etapa 2 — Base de Conhecimento
Código
Todo agente precisa de dados. No nosso caso, você pode criar arquivos simples como:

- ataques.csv — tipos de ataques (phishing, ransomware, DDoS).
- boas_praticas.json — recomendações de segurança (MFA, senhas fortes).
- historico_perguntas.csv — perguntas frequentes de usuários.
- conceitos_basicos.md — definições de OSINT, DevSecOps, Engenharia Social.

Esses dados podem ser carregados no início da sessão ou consultados dinamicamente. O importante é que façam sentido para o problema que você quer resolver.
🎬 Vídeo 4: Etapa 3 — Prompts do Agente
Código
O prompt é o coração do agente.

- System Prompt: "Você é um assistente de cibersegurança. Responda de forma clara e objetiva, usando exemplos práticos. Nunca invente informações. Se não souber, diga isso e sugira fontes confiáveis."
- Exemplos de Interação: perguntas como "O que é phishing?" e respostas esperadas.
- Edge Cases: o que fazer quando o usuário pede algo fora do escopo ou tenta obter informações sensíveis.

Itere nos prompts. Teste, ajuste e documente as mudanças.
🎬 Vídeo 5: Etapa 4 — Aplicação Funcional
Código
Agora é hora de colocar tudo pra funcionar.

Você precisa entregar:
- Um chatbot interativo (Streamlit ou Gradio são boas opções).
- Integração com um LLM via API ou modelo local.
- Conexão com a base de conhecimento.

Comece simples. Teste com as perguntas que você definiu nos prompts. Ajuste conforme necessário.
🎬 Vídeo 6: Etapa 5 — Avaliação e Métricas
Código
Como saber se seu agente funciona bem?

Três métricas principais:
- Assertividade: respondeu corretamente?
- Segurança: evitou inventar informações?
- Clareza: a resposta foi compreensível para iniciantes?

Peça para colegas testarem e avaliarem com notas de 1 a 5. Documente os resultados.
🎬 Vídeo 7: Etapa 6 — Pitch
Código
Grave um pitch de até 3 minutos.

Estrutura:
- Problema: muitas pessoas não sabem se proteger online.
- Solução: um agente virtual que ensina técnicas de cibersegurança.
- Demonstração: mostre o agente funcionando.
- Diferencial: acessível, educativo e confiável.

Seja direto e objetivo.
🎬 Vídeo 8: Dicas Finais
Código
- Comece pelo prompt.
- Use dados mockados simples.
- Foque na segurança: nunca invente informações.
- Teste com cenários reais.
- Seja direto no pitch.
- Dê a sua cara ao projeto.

O mais importante é aprender e mostrar sua evolução.

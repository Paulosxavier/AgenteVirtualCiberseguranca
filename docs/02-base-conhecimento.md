# Base de Conhecimento

## Dados Utilizados

| Arquivo | Formato | Utilização no Agente |
| --- | --- | --- |
| ``ataques.csv`` | CSV | Contém tipos de ataques (phishing, ransomware, DDoS, engenharia social) usados para explicar ameaças e exemplos reais |
| ``boas_praticas.json`` | JSON | Lista de recomendações de segurança (MFA, senhas fortes, backups, uso de VPN) para orientar o usuário |
| ``ferramentas.csv`` | CSV | Apresenta ferramentas de proteção (antivírus, firewall, IDS/IPS) e suas funções |
| ``conceitos_basicos.md`` | Markdown | Define termos essenciais como OSINT, DevSecOps, Spoofing e Engenharia Social |
| ``historico_perguntas.csv`` | CSV | Registra perguntas frequentes e respostas esperadas para treinar o comportamento do agente |

> [!TIP]
Quer um dataset mais robusto? Você pode utilizar fontes públicas e confiáveis como:

OWASP Top 10 (owasp.org in Bing) — principais vulnerabilidades em aplicações web

CERT.br — guias e relatórios sobre incidentes de segurança

NIST Cybersecurity Framework (nist.gov in Bing) — padrões internacionais de segurança

Kaggle Datasets — bases públicas sobre cibersegurança e ataques
---

## Adaptações nos Dados

Os dados mockados foram expandidos para incluir exemplos de ataques e boas práticas de segurança digital.
Foram adicionadas colunas com impacto e exemplos práticos em ataques.csv e categorias em boas_praticas.json para facilitar o aprendizado do usuário.

---

## Estratégia de Integração

### Como os dados são carregados?
Os arquivos CSV e JSON são carregados no início da sessão e mantidos em memória.
O agente consulta dinamicamente o conteúdo conforme o tipo de pergunta — por exemplo, busca em ataques.csv quando o usuário pergunta sobre um tipo de ataque.

Como os dados são usados no prompt?
Os dados são incluídos no contexto do system prompt para garantir respostas consistentes e seguras.
Quando o usuário faz uma pergunta, o agente identifica o tema (ataque, boa prática ou conceito) e consulta o arquivo correspondente antes de responder.
---

## Exemplo de Contexto Montado

Dados de Cibersegurança:
- Ataque: Phishing
- Descrição: Tentativa de enganar usuários para obter informações sensíveis via e-mails falsos.
- Impacto: Roubo de credenciais e acesso indevido a contas.
- Exemplo: E-mail falso de banco pedindo atualização de senha.

Boas Práticas:
- Ative autenticação multifator (MFA).
- Verifique se o site usa HTTPS.
- Nunca compartilhe senhas por aplicativos de mensagem.

Ferramentas:
- Firewall: bloqueia acessos não autorizados.
- Antivírus: detecta e remove malware.
...
```

1- Configurar o Spring Boot e o Spring AI, integrar o Ollama com um modelo aberto, como Llama 3.2, implementar o serviço que envia mensagens ao modelo e recebe respostas, criar o prompt de sistema para o agente de atendimento e testar as respostas do chatbot. Entrega: agente de IA funcionando localmente, sem depender de APIs pagas.

2-
Pipeline de RAG (#3-4 a #4-4): storage de uploads, extração de texto, chunking hierárquico, embeddings em lote via Ollama, campo vetorial no PostgreSQL com a extensão vector, e a orquestração que liga tudo. Corrigi a dimensão do embedding para 768, que travava toda gravação real no banco.
Validação sem IA (#8-1): checklist determinístico de conformidade com o guia, 29 regras em código, apontando o que corrigir.
GraphRAG (#13-1 a #13-4), do começo ao fim: modelos de entidade, relação e comunidade; extração endurecida com JSON Schema, few-shot e canonização de identidade; comunidades com Louvain; ingestão incremental; retrieval no grafo ligado ao agente do chat; visualizador com barra de progresso.
Qualidade de resposta: retrieval com escopo por projeto, system prompt anti-alucinação e expansão de consulta por assunto.
Testes: cobertura da ingestão do grafo sem depender de GPU, pipeline completo de indexação e estados de upload.

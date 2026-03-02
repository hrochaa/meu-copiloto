# meu-copiloto

Coleção de prompts de sistema otimizados para uso com assistentes de IA (GitHub Copilot, ChatGPT, Claude, etc.), focados em desenvolvimento com **C# / .NET**. Cada prompt define um modo de operação distinto, com personalidade, stack, regras e formato de resposta bem definidos — garantindo consistência, qualidade técnica e produtividade nas entregas.

---

## 🗂️ Estrutura do projeto

```
meu-copiloto/
├── promp-agent.md   # Modo AGENT CODE — implementação autônoma de código
├── promp-study.md   # Modo STUDY     — aprendizado guiado e explicações didáticas
├── prompt-ask.md    # Modo ASK       — dúvidas, diagnóstico e sugestões (somente leitura)
└── prompt-plan.md   # Modo PLAN      — planejamento de implementação antes do código
```

---

## 🤖 Modos disponíveis

### `promp-agent.md` — AGENT CODE
> Modo de **implementação autônoma**. O copiloto transforma requisitos em código pronto, com estrutura de arquivos, testes, tratamento de erros e instruções de execução.

**Quando usar:** você sabe o que quer e precisa que o código seja gerado de ponta a ponta.

**Ciclo de trabalho:**
1. **(A) Descobrir** — entende objetivo e restrições
2. **(P) Planejar** — lista arquivos, dependências e critérios de aceite
3. **(I) Implementar** — gera código completo
4. **(V) Verificar** — orienta testes e validação
5. **(F) Finalizar** — checklist e próximos passos

---

### `promp-study.md` — STUDY
> Modo **didático e explicativo**. O copiloto age como um tutor técnico: explica conceitos com progressão, analogias, exemplos mínimos, armadilhas e checkpoints de compreensão.

**Quando usar:** você quer entender um conceito, padrão ou tecnologia de verdade — não só copiar código.

---

### `prompt-ask.md` — ASK (somente leitura)
> Modo de **consulta e diagnóstico**. Responde dúvidas, explica código e diagnostica erros sem executar mudanças. Segue um formato de resposta padronizado: resumo → explicação → como confirmar → opções.

**Quando usar:** você tem um erro, uma dúvida pontual ou quer entender trade-offs antes de decidir.

---

### `prompt-plan.md` — PLAN
> Modo de **planejamento estruturado**. Produz um plano revisável (escopo, arquivos afetados, riscos, testes, passos incrementais) antes de qualquer linha de código ser escrita.

**Quando usar:** a feature é complexa e você quer validar a abordagem antes de implementar.

---

## ⚙️ Stack coberta

| Categoria         | Tecnologias                                                        |
|-------------------|--------------------------------------------------------------------|
| Runtime           | .NET 8                                                             |
| Linguagem         | C# 12                                                              |
| Frameworks Web    | ASP.NET Core, Minimal APIs, MVC                                    |
| Arquitetura       | Clean Architecture, DDD, N-Layer                                   |
| Testes            | xUnit, NUnit, MSTest                                               |
| Mocking           | Moq, NSubstitute, FakeItEasy                                       |
| ORM               | Entity Framework Core, Dapper                                      |
| Validação         | FluentValidation, DataAnnotations                                  |
| Logging           | Serilog, NLog, Microsoft.Extensions.Logging                        |
| DI Container      | Microsoft.Extensions.DependencyInjection, Autofac                  |
| API Docs          | Swagger/OpenAPI, NSwag                                             |
| Package Manager   | NuGet                                                              |
| Banco de dados    | SQL Server, PostgreSQL, MySQL, MongoDB                             |
| Infra             | Docker, Kubernetes, Azure, AWS                                     |

> Os prompts são facilmente adaptáveis para outras stacks — basta editar a seção `### 1) STACK` em cada arquivo.

---

## 🚀 Como usar

1. Abra o arquivo do modo desejado (ex.: `prompt-ask.md`).
2. Copie o conteúdo completo.
3. Cole como **System Prompt** (instrução de sistema) na ferramenta de IA que estiver usando.
4. Inicie sua conversa normalmente.

> **Dica:** mantenha um arquivo por modo aberto no editor para alternar rapidamente entre contextos.

---

## ✏️ Customização

Cada prompt possui seções marcadas como `(EDITÁVEL)`. As principais são:

- **`### 1) STACK`** — troque as tecnologias conforme o projeto.
- **`### 2) PERSONALIDADE`** — ajuste tom, nome e pronomes do assistente.

As demais seções (regras, formato, diretrizes) são intencionalmente fixas para garantir consistência.

---

## 📌 Objetivo

Aumentar **produtividade**, **qualidade técnica** e **consistência** nas entregas ao trabalhar com assistentes de IA, eliminando respostas genéricas e garantindo que o copiloto sempre opere dentro do contexto certo para cada tipo de tarefa.

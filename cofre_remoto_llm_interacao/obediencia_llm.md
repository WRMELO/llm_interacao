# Guia Definitivo para Garantir Obediência Absoluta das LLMs

## 1. Compromisso Explícito

- Inicie todas as interações com uma declaração explícita: **"Você tem o compromisso absoluto de seguir rigorosamente este protocolo."**
- Reforce regularmente que qualquer desvio não é aceitável.

## 2. Definição de Papéis Rígidos

### Usuário (Gerente de Projeto)

- **Implementador:** Executa fielmente os comandos da LLM.
- **Relator:** Relata resultados e erros de maneira detalhada.
- **Orientador Estratégico:** Define claramente o "o quê" do projeto.
- **Validador:** Confirma se resultados estão corretos e alinhados.

### IA (Consultor Técnico)

- **Exclusiva Responsabilidade Técnica:** Assume integralmente todas as decisões técnicas.
- **Geração Completa de Código:** Fornece sempre códigos completos e funcionais.
- **Comunicação Proativa e Clara:** Explica cada decisão técnica detalhadamente.
- **Proibição de Assumir ou Inferir:** Se uma informação não estiver clara, a LLM deve obrigatoriamente perguntar, jamais supor.

## 3. Comunicação Estritamente Sequencial

- Estabeleça claramente duas fases sequenciais obrigatórias:
  1. **Exposição Técnica Completa:**
     - Exposição clara e detalhada sobre o que será feito, como, por que, riscos e impactos.
  2. **Execução Passo a Passo:**
     - Forneça uma única instrução ou bloco de código por vez.
     - Não permita avançar sem que o usuário confirme explicitamente o sucesso da execução anterior.

## 4. Normas de Fornecimento de Código

- **Blocos Completos:** Sempre exija códigos completos para substituir integralmente os anteriores, sem instruções parciais ou incrementais.
- **Claridade Técnica:** Sempre exija justificativas técnicas das escolhas feitas pela LLM.

## 5. Tratamento Obrigatório de Erros

- Se ocorrer um erro, exija imediatamente:
  - Diagnóstico claro e detalhado do erro pela LLM.
  - Uma solução técnica completa antes de prosseguir.

## 6. Proibição Rigorosa de Suposições

- Declare explicitamente: **"É terminantemente proibido fazer qualquer tipo de suposição sobre informações faltantes."**
- Estabeleça que, se algo não estiver claro ou incompleto, é **obrigatório perguntar**.

## 7. Formatação e Clareza

- Exija que toda comunicação seja feita em Markdown.
- Exija a utilização correta de blocos de código com especificação de linguagem (Python ou Bash).

## Exemplo Prático de Comunicação Exigida

````markdown
**IA:**
"Este é o contexto completo, incluindo arquitetura, riscos e decisões técnicas detalhadas."

**IA:**
```python
# Bloco de código completo
````

**Usuário:** "Executado com sucesso."

**IA:** "Perfeito. Próxima etapa:"

**Usuário:** "Erro ao executar: [mensagem detalhada]"

**IA:** "Diagnóstico completo do erro. Solução proposta:"

```python
# Novo bloco completo corrigido
```

```

## Conclusão
- Ao seguir rigorosamente estas diretrizes detalhadas e explícitas, você garante a obediência absoluta das LLMs, prevenindo desvios e garantindo eficiência máxima nas suas interações.

```

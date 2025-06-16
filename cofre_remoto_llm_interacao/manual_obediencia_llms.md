
# Manual de Garantia de Obediência das LLMs  
*(Complemento ao “Protocolo de Interação e Colaboração — Versão 2”)*

## 1. Princípio Supremo  

> **NENHUMA resposta pode contrariar as instruções deste manual ou do Protocolo.**  
> Se houver conflito entre camadas de mensagem, prevalece (na ordem):  
> 1. **Este Manual**  
> 2. **Protocolo de Interação**  
> 3. Mensagem *system*  
> 4. Mensagem *developer*  
> 5. Mensagem *user*  

---

## 2. Estrutura Recomendada de Todo Novo Chat  

1. **Bloco *system* (opcional, mas recomendado)**  
   ```text
   Você é um consultor técnico especializado. Siga à risca o “Manual de Garantia de Obediência das LLMs” e o
   “Protocolo de Interação e Colaboração — Versão 2”. NÃO quebre essas regras.
   ```  
2. **Bloco *developer* (cole o hash ou link da versão mais recente do protocolo)**  
   ```text
   # ProtocolRef: 2025-06-15-v2
   (Cole aqui o conteúdo íntegral ou o caminho para o arquivo `.md` no repositório.)
   ```  
3. **Bloco *user* (sua instrução)**  
   - Sempre comece declarando:  
     > “Estou utilizando o Manual de Garantia de Obediência + Protocolo v2. Responda dentro dessas regras.”  

---

## 3. Check-list Pré-Envio de Prompt  

| Item | Pergunta de verificação | OK? |
|------|------------------------|-----|
| **Contexto dado?** | O LLM recebeu tudo que precisa para não assumir? | ☐ |
| **Fase indicada?** | Especifique se é *Fase Contexto* ou *Fase Execução*. | ☐ |
| **Uma ação por vez?** | Há apenas *um* comando, pergunta ou bloco de código? | ☐ |
| **Exigiu BLOCO COMPLETO?** | Reforçou que quer código/config inteiro, nada parcial? | ☐ |
| **Pedido de confirmação explícita?** | Terminou com “Aguarde minha confirmação antes de prosseguir”? | ☐ |

---

## 4. Palavras-chave de Controle  

| Palavra-chave | Função | Quando usar |
|---------------|--------|-------------|
| **`Fase Contexto`** | Obriga o LLM a explicar *o que, por quê, alternativas, riscos*. | Início de tarefa nova. |
| **`Fase Execução`** | Instrui o LLM a dar **um** passo e parar. | Após concordar com o contexto. |
| **`BLOCO COMPLETO`** | Garante entrega de arquivo/célula inteira. | Qualquer alteração de código. |
| **`AGUARDE CONFIRMAÇÃO`** | Faz o LLM pausar até você validar. | Final de cada passo. |

> **Exemplo:**  
> “`Fase Execução:` gere o BLOCO COMPLETO do `docker-compose.yml` para o serviço X. AGUARDE CONFIRMAÇÃO.”

---

## 5. Ritual de Interrupção (“Stop-word”)  

Sempre que o comportamento sair do protocolo, envie a palavra **`REINICIAR PROTOCOLO`**.  
O LLM deve:  
1. Pedir desculpas.  
2. Retomar a última etapa **sem** perder o histórico.  
3. Aguardar confirmação.

---

## 6. Template de Prompt Inicial (copie-e-cole)  

```markdown
### ⏮️ Setup do Chat  
Estou iniciando um novo diálogo.

1. **Referência:** Manual de Garantia de Obediência + Protocolo de Interação v2 (hash 2025-06-15-v2).  
2. **Modo:** Modelo híbrido (Fase Contexto ➔ Fase Execução), uma ação por vez.  
3. **Stop-word:** REINICIAR PROTOCOLO.

### 🧩 Fase Contexto  
Explique (o que, por quê, alternativas, riscos) sobre ____________.  
AGUARDE CONFIRMAÇÃO.
```

---

## 7. Atualização de Versões  

1. **Semântica de versão:** `AAAA-MM-DD-vX`.  
2. **Commits atômicos:** Toda mudança no protocolo ou neste manual deve ser um único commit descrito em imperativo curto.  
3. **Changelog:** Mantenha no final do arquivo.  

---

## 8. Recomendações Finais  

* **Mantenha este manual e o protocolo no mesmo repositório** que seus projetos — facilita diff e auditoria.  
* **Use Tags ou Releases** no Git para versionar grandes revisões do protocolo.  
* **Automatize:** crie snippet ou comando no VS Code para inserir o *boilerplate* do chat inicial.  

> “A obediência é função direta da clareza, prioridade e repetição das instruções.”


# 🧠 Prompt Inicial para Continuidade de Projetos com LLM

Este é um prompt genérico para reinício de sessões de chat com uma IA, garantindo continuidade precisa, rastreabilidade e aderência às diretrizes do projeto.

---

## ✅ Objetivo

Garantir que a IA compreenda corretamente o estado atual de um projeto em andamento e continue o trabalho com consistência, respeitando as decisões técnicas já tomadas, a organização documental e o estilo de colaboração desejado.

---

## 📎 Instruções para a IA

1. **Leia cuidadosamente o arquivo `00_HUB.md`** enviado neste chat.
   - Esse arquivo contém a **visão consolidada do projeto**, com contexto, histórico, decisões técnicas e links para os documentos auxiliares.
   - Ele representa o **estado mais atualizado** do projeto e deve ser a principal referência inicial.

2. **Siga rigorosamente o `protocolo-de-interacao.md`**, também incluído neste chat.
   - Esse protocolo define os **papéis, fluxos de comunicação, padrões de resposta e responsabilidade técnica** da IA.
   - A IA deve respeitar o modelo híbrido obrigatório: primeiro apresentar o **panorama técnico completo**, depois conduzir a **execução sequencial passo a passo**, aguardando validações explícitas do usuário.

3. **Não faça suposições técnicas nem generalizações.**
   - Se faltar uma informação essencial (como nome de um campo, formato de tabela ou estrutura de diretório), **solicite explicitamente** ao usuário antes de continuar.

4. **Utilize os arquivos adicionais referenciados no `00_HUB.md` apenas se forem enviados.**
   - Caso algum documento mencionado não esteja presente no chat atual, peça ao usuário que o envie se necessário.

---

## 🧭 Recomendações Adicionais

- Adote uma postura proativa e explicativa: justifique decisões, explique blocos de código, esclareça riscos.
- Mantenha a rastreabilidade de tudo que for decidido ou executado neste novo chat.
- Sempre ofereça respostas que possam ser reutilizadas em futuras retomadas (como códigos completos ou resumos atualizados).

---

📌 Este prompt deve ser utilizado no início de qualquer novo chat envolvendo projetos técnicos estruturados em Markdown.  
📅 Atualizado: 13/06/2025

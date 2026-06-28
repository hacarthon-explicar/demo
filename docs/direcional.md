# ExpliCAR — Direcional de Desenvolvimento

Guia para orientar a construção da demonstração do ExpliCAR a partir do estado atual do projeto.

---

## Instrução de Desenvolvimento

Sua tarefa é produzir **3 entregáveis** a partir dos arquivos desta pasta, nesta ordem:

### Entregável 1 — Aplicar as mudanças pendentes
Atualize o conteúdo dos arquivos existentes conforme as decisões registradas neste documento:
- **Calculadora → Resumo Legal Personalizado** — substituir toda referência à calculadora genérica pelo resumo legal gerado pelo Téo com dados reais do CAR (base legal já está em `persona-tecnico.md`)
- **Persona adaptativa** — garantir que a persona Téo com 3 tons e adaptação por feedback explícito esteja refletida em todos os artefatos
- **LGPD e código aberto** — incorporar as premissas de proteção de dados e a separação código × dados

Arquivos a modificar: `plano-demonstracao.md`, `ideação.md`, `persona-tecnico.md`, e quaisquer outros que referenciem calculadora ou conceitos obsoletos.

### Entregável 2 — Demonstração navegável (HTML/CSS/JS + wireframes)
Produza uma demonstração front-end em HTML/CSS/JS puro (sem frameworks) que:

1. **Percorra a jornada completa do usuário** descrita no `plano-demonstracao.md`:
   - Tela de entrada (QR code ou CPF + CAR code)
   - Tela de identificação (propriedade reconhecida com pendências listadas)
   - Tela de escolha do tom (Direto ao ponto / Explicado com calma / Completo)
   - Chat simulado com Téo (mensagens pré-escritas seguindo a persona, com botões "Não entendi" e "Quero entender melhor" que alternam entre os níveis)
   - Barra de gamificação (progresso "1 de 3")
   - Botão "Ouvir" em cada resposta (simular ativação do OmniVoice)
   - FAQ contextual com campo de busca e fuzzy matching simulado
   - Resumo Legal Personalizado gerado dinamicamente na conversa
   - Tela de resumo final com passos numerados

2. **Inclua uma segunda página HTML** com os fluxogramas do sistema:
   - Fluxograma da jornada do usuário (usando o diagrama Mermaid do `plano-demonstracao.md` como referência)
   - Fluxograma da arquitetura do sistema
   - Fluxograma da adaptação de níveis da persona
   - Fluxograma do Resumo Legal Personalizado (regras condicionais: bioma → ZEE → módulos fiscais → marco 2008)
   - Renderizados como SVG/CSS (não como imagem), responsivos e com o esquema de cores do projeto

3. **Requisitos técnicos:**
   - HTML/CSS/JS puro (zero dependências, zero frameworks)
   - Design mobile-first, responsivo
   - Esquema de cores do projeto: verde escuro (#2F5D3A), terra (#C05A33), ouro (#D99A2E), teal (#266E77), creme (#FCF8EE / #F3ECDC), texto (#221E17)
   - Contraste acessível entre fundo e texto em todas as telas
   - Tipografia: Hanken Grotesk (texto), Bitter (títulos), DM Mono (código/dados)
   - Uma única página HTML (single-page) para a demonstração principal com transições entre telas via CSS/JS
   - Os dados mock do SICAR devem estar embutidos no JS (const MOCK_DATA)

### Entregável 3 — Roteiro de apresentação + PPTX
Produza:
1. Um **roteiro de apresentação de 3 minutos** (passo a passo, cena por cena, com falas do apresentador e notas sobre o que mostrar em cada tela da demonstração) — salvar como `roteiro-apresentacao.md`
2. Uma **apresentação em PPTX** seguindo a estrutura abaixo, com conteúdo extraído dos arquivos do projeto:
   - Slide 1: Capa — ExpliCAR
   - Slide 2: O Problema (notificação incompreensível)
   - Slide 3: O Insight (mutirão resolve em 20 minutos)
   - Slide 4: A Solução — Téo, o técnico digital
   - Slide 5: Fluxo da Jornada (usar o diagrama do entregável 2)
   - Slide 6: Diferenciais (persona adaptativa, 100% opensource, LGPD por desenho)
   - Slide 7: Funcionalidades do MVP (chat, gamificação, áudio, FAQ, resumo legal)
   - Slide 8: Impacto esperado
   - Slide 9: Equipe e agradecimento

### Ordem de trabalho
1. Primeiro o Entregável 1 (atualizar artefatos existentes)
2. Depois o Entregável 2 (demonstração navegável + fluxogramas)
3. Por último o Entregável 3 (roteiro + PPTX)

### Critérios de sucesso
- A demonstração navegável funciona sem servidor (só abrir o HTML no navegador)
- O chat simulado reflete fielmente a persona Téo (tom, níveis, adaptação)
- Os fluxogramas estão precisos e usam as cores do projeto
- O roteiro de apresentação cabe em 3 minutos
- O PPTX pode ser aberto e editado no PowerPoint / Google Slides / LibreOffice

---

## Estado da Arte (o que já está definido)

### Persona Téo
- **Arquivo:** `persona-tecnico.md`
- **O que contém:** definição completa da persona — identidade, tom, regras de ouro, 3 níveis de explicação (Direto ao ponto / Explicado com calma / Completo), tabela de adaptação por sinais do usuário, frases-âncora, antipadrões
- **Formato:** otimizado para uso como system prompt de LLM (YAML frontmatter + seções estruturadas + exemplos)
- **Ação necessária:** se já existir um arquivo com este nome no projeto, **substitua pela versão enviada** — está desatualizada
- **Status:** ✓ Completo (nova versão)

### Plano de Demonstração
- **Arquivo:** `plano-demonstracao.md`
- **O que contém:** jornada do usuário completa (fluxo visual), especificação das funcionalidades do MVP (chat, gamificação, áudio com OmniVoice, FAQ contextual, resumo legal personalizado), arquitetura 100% opensource, stack tecnológica, mapeamento ExpliCAR × critérios do Desafio 3, roteiro de apresentação de 3 minutos, roadmap pós-MVP
- **Ação necessária:** **Arquivo novo** — adicionar ao projeto
- **Status:** ✓ Completo

### Ideação (entrega do hackathon)
- **Arquivo:** `ideação.md`
- **O que contém:** respostas para as 10 seções da fase de ideação — brainstorm, problema, solução, público-alvo, impacto, diferencial, viabilidade, implementação, código aberto + LGPD + segurança, mentoria com feedback da Lorrana Nunes
- **Ação necessária:** **Arquivo novo** — adicionar ao projeto
- **Status:** ✓ Completo

### Protótipo Visual (existente, como referência)
- **Arquivo:** removido da estrutura final
- **O que contém:** protótipo navegável com telas de home, chat, cards, calculadora, termos e salvos, com 2 temas visuais (cartilha e mutirão)
- **Nota:** a "calculadora" do protótipo foi substituída pelo **Resumo Legal Personalizado** gerado pelo Téo com base nos dados reais do CAR
- **Observação:** serviu como referência visual de layout, cores e componentes, mas não foi reutilizado como código

### Direcional de Desenvolvimento (este arquivo)
- **Arquivo:** `direcional.md`
- **O que contém:** instrução principal de desenvolvimento — define os 3 entregáveis, ordem de trabalho, critérios de sucesso, stack, decisões de projeto e referências para os demais arquivos
- **Ação necessária:** **Arquivo novo** — adicionar ao projeto. **Comece por ele:** leia a seção "Instrução de Desenvolvimento" antes de qualquer outra coisa
- **Status:** ✓ Completo

---

## O que falta para a demonstração

### Prioridade máxima (necessário para o pitch)

| Item | Descrição | Referência |
|---|---|---|
| **Frontend React (PWA)** | Aplicação mobile-first com as telas da jornada: entrada → identificação → escolha de tom → chat → resumo | `plano-demonstracao.md` — seção 1 (jornada) e 2.1 (chat) |
| **Backend FastAPI (mock funcional)** | API com rota de chat que recebe a mensagem do produtor e retorna resposta do Téo no tom escolhido, com dados mockados do SICAR | `plano-demonstracao.md` — seção 3 (arquitetura) |
| **Integração com LLM auto-hospedado** | Conectar backend a um LLM aberto (Ollama com Llama 3 / Mistral / Qwen) rodando na infraestrutura do órgão, usando a persona de `persona-tecnico.md` como system prompt | `persona-tecnico.md` completo |
| **Gamificação funcional** | Barra de progresso "X de Y pendências" que avança conforme o produtor interage no chat | `plano-demonstracao.md` — seção 2.2 |
| **Áudio (OmniVoice)** | Botão "Ouvir" em cada resposta de Téo — TTS processado no servidor | `plano-demonstracao.md` — seção 2.3 |
| **FAQ Contextual** | Respostas rápidas com fuzzy matching para perguntas frequentes, embutido no chat | `plano-demonstracao.md` — seção 2.4 |
| **Dados Mock do SICAR** | Conjunto de dados de exemplo de um produtor com 3 pendências típicas (APP, Reserva Legal, Matrícula) para alimentar a demonstração | `plano-demonstracao.md` — seção 4 (roteiro) |

### Importante (mas não bloqueia o pitch)

| Item | Descrição |
|---|---|
| **Autenticação real** | CPF + CAR code + QR code |
| **LGPD na prática** | Pseudonimização, política de retenção, exclusão |
| **Testes com produtores** | Validação da persona com usuários reais |

---

## Orientações para Implementação

### Stack a usar
- Frontend: React + Vite + PWA
- Backend: Python + FastAPI + Uvicorn
- LLM: Ollama (dev) / vLLM (prod) com Llama 3, Mistral ou Qwen
- TTS: OmniVoice (k2-fsa, Apache 2.0)
- Banco: PostgreSQL
- Container: Docker Compose

### Como usar os arquivos existentes

1. **persona-tecnico.md** → usar como system prompt do LLM. O arquivo já está formatado para isso (instrução do sistema, regras, níveis, exemplos)
2. **plano-demonstracao.md** → usar como especificação de produto. Cada funcionalidade descrita lá é um card de implementação
3. **ideação.md** → usar como documento de submissão do hackathon (já completo)
4. **Protótipo Visual** (existente no histórico) — usado como referência visual para layout, cores e componentes, sem reaproveitamento de código

### Decisões já tomadas (não reabrir)

| Decisão | Escolha |
|---|---|
| Público-alvo | Produtor rural (não o técnico) |
| Níveis de tom | 3 fixos selecionados no cadastro, com adaptação por feedback explícito |
| LLM | Agnóstico — a persona controla o comportamento |
| TTS | OmniVoice (Apache 2.0, auto-hospedado) |
| Licenciamento | MIT / Apache 2.0 |
| Integração SICAR | Mock na demo, adapter preparado para real depois |
| **Calculadora** | **Removida.** Substituída por **Resumo Legal Personalizado** gerado pelo Téo no chat, com base nos dados reais do CAR |

### Resumo Legal Personalizado (substitui a calculadora)

A calculadora genérica do protótipo foi removida porque:
- O sistema já conhece a área, bioma e dados da propriedade — não faz sentido o produtor digitar
- A legislação real tem regras condicionais encadeadas (ZEE, módulos fiscais, marco 2008) que uma calculadora simples não captura
- O que o produtor precisa é de **explicação contextual**, não de um número solto

Em vez disso, Téo gera automaticamente um resumo legal personalizado durante o chat:

> *"Seu Raimundo, o Sítio Boa Esperança tem 85 hectares e fica na Amazônia Legal. Pela lei, a Reserva Legal precisaria ser de 80% — 68 hectares. Mas como o Pará tem Zoneamento Ecológico-Econômico e sua área está em zona de consolidação, esse percentual cai para 50%. E como sua propriedade tem menos de 4 módulos fiscais, o senhor pode manter como RL a vegetação nativa que já existia em julho de 2008."*

**Status:** ✓ Já adicionado à persona em `persona-tecnico.md` — seção "Base de conhecimento legal" com tabelas de RL, ZEE, Art. 67, APP, área consolidada e exemplo de resumo

---

## Estrutura de Diretórios Recomendada

```
explicar/
├── frontend/           # React + Vite + PWA
│   ├── src/
│   │   ├── screens/    # Home, Chat, Resumo
│   │   ├── components/ # ProgressBar, AudioPlayer, MessageBubble
│   │   └── service-worker.js
│   └── package.json
├── backend/            # FastAPI
│   ├── app/
│   │   ├── routes/     # chat.py, auth.py, sicar.py
│   │   ├── persona/    # prompt_templates/
│   │   ├── llm/        # orchestrator.py
│   │   ├── tts/        # omnivoice_adapter.py
│   │   └── models/     # user.py, session.py
│   ├── mock/           # dados_sicar_exemplo.json
│   └── requirements.txt
├── docker-compose.yml
└── docs/
    ├── persona-tecnico.md
    ├── plano-demonstracao.md
    ├── direcional.md (este arquivo)
    └── ideação.md
```

---

## Anexo: Atualização do Pitch (export/CAR Explica - Pitch.pptx)

O arquivo `export/CAR Explica - Pitch.pptx` existe mas reflete o estado anterior do projeto (com calculadora genérica, sem a persona adaptativa refinada, sem OmniVoice). Para alinhar ao estado atual, o pitch precisa ser atualizado com:

### O que trocar

| Slide atual | Substituir por |
|---|---|
| Calculadora como funcionalidade | **Resumo Legal Personalizado** gerado pelo Téo com dados reais do CAR |
| Persona genérica | **Persona Téo com 3 tons** (Direto ao ponto, Explicado com calma, Completo) + tabela de adaptação |
| TTS genérico | **OmniVoice** (Apache 2.0, 646 línguas, 40× tempo real) |
| Sem menção a LGPD | **LGPD como premissa arquitetural** (pseudonimização, minimização, transparência) |
| Sem menção a código aberto | **Estratégia de código aberto** com separação claro do que é público vs protegido |
| Gamificação ausente | **Barra de progresso** "1 de 3 pendências" |
| Sem menção a testes | **Testes com produtores reais** como fase de calibragem da persona |

### Estrutura sugerida para o pitch atualizado

1. **Problema** — notificação incompreensível, processos parados
2. **Insight** — mutirão resolve em 20 minutos. A conversa é o diferencial
3. **Solução** — ExpliCAR: Téo, o técnico digital que explica no tom certo
4. **Demonstração** — fluxo completo: QR code → identificação → tom → chat adaptativo → gamificação → áudio → resumo legal
5. **Diferenciais** — persona adaptativa, 100% opensource, LGPD por desenho
6. **Impacto** — menos processos parados, produtor entende e resolve
7. **Equipe** — quem somos
8. **Agradecimento**

### Como gerar o novo pitch

O conteúdo atualizado está distribuído nestes arquivos:
- **Persona + base legal:** `persona-tecnico.md`
- **Fluxo, funcionalidades, arquitetura, roteiro:** `plano-demonstracao.md`
- **LGPD, segurança, código aberto:** `ideação.md` (seção 9)
- **Referência visual (cores, componentes):** protótipo existente no histórico do projeto

# Fase de Ideação — ExpliCAR

---

## 1. BRAINSTORM

O processo começou com a experiência prática da equipe nos **mutirões do CAR promovidos pela SEMAS**. Durante esses mutirões, observamos um padrão: processos que estavam parados há anos eram resolvidos em **20 minutos de conversa presencial** entre o técnico e o produtor. O gargalo era mais de comunicação do que técnico.

Listamos várias ideias para resolver isso:

| Ideia | Por que foi descartada |
|---|---|
| **Cartilha ilustrada** (PDF explicativo) | Estática, não se adapta ao nível de entendimento de cada produtor |
| **Vídeos educativos** | Via de mão única, sem interação, não responde dúvidas específicas |
| **WhatsApp Bot** | Dependente de plataforma proprietária (Meta), sem garantia de privacidade dos dados do produtor |
| **FAQ online** | Não cobre a personalização que um atendimento presencial oferece |
| **Sistema de perguntas e respostas com IA** | Era a direção certa, mas ainda muito genérica |

A ideia escolhida foi o **ExpliCAR**: um chat conduzido por uma persona (Téo) que replica a dinâmica do atendimento presencial do mutirão, com **linguagem adaptativa**, **dados reais da propriedade** e **múltiplos canais de acesso** (texto, áudio, gamificação).

**Por que venceu:** porque parte de uma experiência validada em campo (os mutirões funcionam) e a digitaliza sem perder a essência: a conversa lado a lado, no tom certo para cada perfil de proprietário/possuidor.

---

## 2. PROBLEMA

**O problema:** As notificações do SICAR são emitidas em linguagem jurídica e técnica, repletas de siglas (APP, RL, AC, PRA) e referências a artigos de lei. O pequeno e médio produtor rural não entende o que precisa fazer. Como resultado, processos de regularização ficam parados por anos, não por má vontade, mas por falta de compreensão.

**Quem enfrenta:** Pequenos e médios proprietários e possuidores rurais, especialmente aqueles com baixa familiaridade com termos jurídicos e tecnologia.

**O que acontece hoje:** O produtor recebe uma notificação, não entende, sente medo (por vezes acha que é multa), não procura ajuda, e a pendência se arrasta. Quando busca informação, recorre a fontes nem sempre confiáveis.

**Por que é importante:** O CAR é a espinha dorsal da regularização ambiental no Brasil (Lei 12.651/2012). Se o produtor não entende o que precisa fazer, a regularização não avança, o desmatamento não é combatido, e o produtor perde acesso a crédito e incentivos ambientais. O custo desse gap de entendimento é ambiental, econômico e social.

---

## 3. SOLUÇÃO

O **ExpliCAR** é um assistente digital (Téo) que traduz a notificação do SICAR para a linguagem do produtor rural, em formato de conversa.

**Como funciona:**

1. **Entrada** — O produtor chega por QR code na notificação ou digita CPF + código do CAR
2. **Identificação** — O sistema reconhece a propriedade e lista as pendências
3. **Escolha do tom** — O produtor escolhe o nível de explicação: **Direto ao ponto**, **Explicado com calma** ou **Completo**
4. **Chat adaptativo** — Téo explica cada pendência usando:
   - Dados reais da propriedade ("Sítio Boa Esperança", "Riacho Seco")
   - Estrutura clara: O que significa → Por que aconteceu → O que fazer
   - Adaptação em tempo real: se o produtor não entende, Téo simplifica; se quer detalhes, Téo aprofunda
5. **Gamificação** — Barra de progresso visível ("1 de 3 pendências resolvidas") reduz ansiedade e mostra avanço
6. **Áudio** — Botão "Ouvir" com OmniVoice TTS para produtores que preferem escutar
7. **FAQ contextual** — Respostas rápidas a perguntas frequentes, com tolerância a erros de digitação
8. **Saída** — Resumo numerado dos passos, salvável e compartilhável

**Como resolve o problema:** Substitui o juridiquês da notificação por uma conversa clara, personalizada e adaptativa — exatamente como o técnico faz no mutirão, mas disponível a qualquer hora, pelo celular do produtor, onde ele estiver.

---

## 4. PÚBLICO-ALVO

**O foco é o proprietário ou possuidor rural** — pequeno e médio produtor que recebeu uma notificação do SICAR e precisa entender o que fazer.

**Por que esse público:**
- É quem está na ponta do problema — recebe a notificação, não entende, e o processo trava
- A vivência nos mutirões da SEMAS mostrou que, quando o produtor **entende**, ele **resolve** — processos parados há anos se desenrolam em minutos
- O produtor rural não é analfabeto funcional na sua realidade — ele conhece a própria terra, os limites, as nascentes. O problema é que a notificação fala uma língua que não é a dele

Técnicos e extensionistas também se beneficiam: a ferramenta pode ser usada como roteiro de atendimento, padronizando a qualidade da explicação entre diferentes profissionais e reduzindo o tempo de cada atendimento. Mas o centro do desenho é o produtor.

---

## 5. IMPACTO

| Para quem | Impacto esperado |
|---|---|
| **Produtor rural** | Entende a pendência, perde o medo ("não é multa"), sabe exatamente o que fazer. Sai de "não sei" para "vou resolver" |
| **CAR / SICAR** | Redução do tempo de regularização. Menos processos parados por falta de entendimento. Melhora na qualidade dos dados declarados |
| **Órgãos ambientais (OEMAs)** | Menos retrabalho, menos atendimentos repetitivos, mais eficiência na análise. A base de referência geoespacial melhora porque o produtor entende a importância de declarar corretamente |
| **Sociedade** | Mais imóveis regulares → mais preservação e recuperação florestal → mais segurança jurídica para a produção |

**Resultado esperado:** replicar digitalmente o que o mutirão faz no presencial — transformar anos de espera em 20 minutos de entendimento.

---

## 6. DIFERENCIAL

**Como o problema é resolvido hoje:**
- Manuais e cartilhas do SICAR (densos, técnicos)
- Atendimento presencial nos mutirões (funciona, mas tem alcance limitado)
- WhatsApp com vizinhos ou síndicos rurais (informação não validada)
- Balcão da OEMA (demanda presencial, horário comercial, deslocamento)

**O que o ExpliCAR faz de diferente:**
- **Persona adaptativa:** 3 níveis de explicação que mudam em tempo-real conforme a reação do produtor — sem que ele precise pedir
- **Personalização real:** usa o nome da propriedade, os dados do CAR, o nome do rio — não é uma resposta genérica
- **Digitaliza o mutirão:** não substitui o técnico, mas replica a dinâmica que funciona (conversa lado a lado, com paciência, mostrando na tela)
- **Gamificação que engaja:** mostrar progresso ("2 de 3 resolvidas") reduz a ansiedade e motiva a concluir
- **Áudio:** produtor ouve em vez de ler — essencial para baixa alfabetização
- **100% código aberto:** qualquer estado ou município pode implantar sem depender de fornecedor

---

## 7. VIABILIDADE

**Tecnológica:** A solução usa tecnologias maduras e 100% abertas — Python/FastAPI no backend, React no frontend, LLMs abertos (Llama, Mistral, Qwen) para o chat, OmniVoice para TTS, PostgreSQL para dados. Nenhum componente proprietário ou service lock-in. O LLM é agnóstico: a persona (prompt) dita o comportamento, não o modelo.

**Legal:** A solução não armazena dados sensíveis desnecessariamente. Pode ser hospedada em infraestrutura pública (gov.br), respeitando a LGPD. A base de conhecimento usa leis e normativas públicas (Lei 12.651/2012, Decreto 7.830/2012).

**Operacional:** A arquitetão permite deploy em servidor único (fase inicial) ou escalada horizontal. O PWA elimina a necessidade de lojas de aplicativo. O atendimento é assíncrono e pode ser retomado. Uma equipe de 2 a 3 desenvolvedores consegue manter e evoluir o sistema.

---

## 8. IMPLEMENTAÇÃO

Com todos os recursos disponíveis, estimamos **4 a 5 meses** para uma versão funcional testada com produtores reais.

| Fase | Duração | O que inclui |
|---|---|---|
| **1. Fundação** | 4 semanas | Setup do projeto (React + FastAPI + PostgreSQL), integração com LLM aberto, mock do SICAR, estrutura da persona |
| **2. Núcleo** | 4 semanas | Chat funcional com 3 níveis de tom, gamificação básica, FAQ contextual, adaptação de nível por feedback |
| **3. Áudio** | 3 semanas | Integração OmniVoice TTS, cache de mensagens |
| **4. Testes com produtores** | 4 semanas | Sessões presenciais com produtores reais, calibragem da persona e dos níveis, ajustes de linguagem |
| **5. Refinamento** | 3 semanas | Correções dos testes, acessibilidade básica (WCAG), polimento de UX |
| **6. Entrega** | 2 semanas | Documentação, empacotamento Docker, deploy em homologação |

**Total: ~20 semanas (5 meses)**

---

## 9. CÓDIGO ABERTO E LGPD

O ExpliCAR será desenvolvido como **código aberto** (licenças MIT / Apache 2.0) — conforme exige o briefing do desafio — mas com uma separação clara e obrigatória: **o código é aberto, os dados não são.**

### LGPD como premissa arquitetural

A solução lida com dados pessoais do produtor (CPF, geolocalização do imóvel) e dados cadastrais do CAR. Por isso, a LGPD (Lei 13.709/2018) é um requisito de desenho:

- **Pseudonimização:** o identificador do produtor no sistema é um hash derivado do CPF + CAR code. O dado bruto só trafega na autenticação e não é armazenado em logs ou cache
- **Minimização:** o sistema só coleta o necessário para o atendimento, não rastreia localização, não coleta contatos além do necessário, não persiste conteúdo da conversa após o encerramento (salvo se o produtor salvar explicitamente)
- **Finalidade:** os dados são usados exclusivamente para explicar a pendência do CAR daquela pessoa. Sem compartilhamento, sem perfilamento, sem publicidade
- **Transparência:** o produtor vê exatamente quais dados estão sendo usados (nome da propriedade, área, pendências) e pode solicitar a exclusão conforme art. 18 da LGPD
- **Segurança:** todas as comunicações via HTTPS, LLM roda em infraestrutura própria (sem envio de dados para terceiros), banco criptografado em repouso

### O que fica aberto × o que fica protegido

| Aberto (repositório público) | Protegido (não versionado) |
|---|---|
| Código do frontend (React) | Chaves de API e tokens |
| Código do backend (FastAPI) | Dados reais de produtores |
| Persona Téo (prompt) | Logs de conversas |
| Infraestrutura (Docker + scripts) | Configurações de banco em produção |
| Adapter de SICAR (mock público) | Credenciais de integração com SICAR real |
| FAQ e base de conhecimento | Dados de autenticação |

### Como outros órgãos reutilizam

1. **Repositório público** com Docker Compose — um comando sobe o sistema completo com dados mockados para demonstração
2. **Persona parametrizada** — o prompt da persona Téo é um arquivo de texto independente. Cada órgão pode criar sua própria persona sem alterar código
3. **Adapter de SICAR** — interface padronizada. O mock público pode ser substituído pela API real de cada estado, que roda na rede interna do órgão
4. **Modelo agnóstico** — funciona com qualquer LLM aberto (Llama, Mistral, Qwen). O comportamento é controlado pela persona, não pelo modelo
5. **Separação código × configuração** — o repositório contém exemplos e schemas, nunca dados reais. Cada implantação copia o repositório, configura suas credenciais e conecta sua base
6. **LGPD por herança** — o código já embute as práticas de proteção de dados. Quem implanta só precisa adequar ao contexto local (ex: política de retenção do estado)

### Notas de segurança

- **Sigilos versionados:** nenhum dado real de produtores, credenciais de banco, chaves de API ou tokens de integração SICAR é versionado no repositório. O uso de variáveis de ambiente e gerenciadores de segredos (ex: HashiCorp Vault) é obrigatório para implantação
- **Superfície de ataque reduzida:** o backend expõe apenas endpoints restritos (/chat, /auth, /sicar). O LLM opera em rede interna. O banco de dados não tem acesso público. O frontend é um PWA estático
- **Revisão por pares:** por ser código aberto, a base é revisada por diferentes órgãos que implantam o sistema, aumentando a chance de detecção precoce de vulnerabilidades
- **Responsible disclosure:** o repositório incluirá SECURITY.md com canal para reportar vulnerabilidades, política de disclosure e prazo estimado de resposta

### Modelo de governança

A solução pode ser mantida como **Bem Público Digital** sob guarda do poder público, com contribuições de estados e municípios via repositório central — cada um operando sua própria instância com seus próprios dados.

---

## 10. MENTORIA E FEEDBACK DA SOLUÇÃO

**Nome do(a) mentor(a):** Lorrana Nunes (@lorrana_nunes)

**Resumo do feedback recebido:**

A mentora destacou os seguintes **pontos fortes** da solução:

- **Experiência validada em campo:** a vivência em mutirões da SEMAS prova que a solução responde a uma dor real e recorrente
- **Tradução técnica simplificada:** transforma notificações cheias de jargões em instruções claras e práticas
- **Persona adaptativa:** ajusta automaticamente a linguagem conforme o perfil do produtor, sem burocracia extra
- **Simulação de atendimento humano:** aproxima a experiência digital da realidade de campo, acolhendo o produtor
- **Impacto imediato:** resolve pendências que poderiam ficar anos paradas por falta de compreensão

E apontou as seguintes **fragilidades** a serem resolvidas:

- **Dependência tecnológica:** precisa de integração robusta com bases oficiais do CAR
- **Complexidade da IA:** calibrar a persona adaptativa exige testes extensivos e refinamento contínuo
- **Exclusão parcial:** sem recursos inclusivos, pessoas com deficiência podem ficar de fora
- **Conectividade rural:** em áreas com conectividade limitada, o alcance pode ser restrito

A mentora sugeriu direções para tornar a solução mais acessível, escalável e competitiva: multimodalidade (áudio, Libras, legendas), gamificação, exemplos práticos de mutirões, FAQ contextual, diretrizes WCAG e testes com produtores reais.

**O que ajustamos a partir do feedback:**

Cada fragilidade apontada gerou uma ação concreta:

| Fragilidade | Ação |
|---|---|
| **Complexidade da IA** | Implementamos **3 tons fixos selecionados no cadastro** (Direto ao ponto, Explicado com calma, Completo) em vez de depender de detecção automática. A adaptação acontece dentro do tom escolhido, via feedback explícito do usuário. Reduz drasticamente a necessidade de calibragem |
| **Conectividade rural** | O serviço exige conexão com internet para funcionar (LLM + SICAR). O produtor pode acessar de qualquer lugar com sinal — pelo celular, no sindicato, na casa do vizinho. O resumo final pode ser salvo como PDF e consultado depois |
| **Exclusão parcial** | Adicionamos **áudio (TTS)** como prioridade no MVP. Libras, legendas e WCAG completo entram no roadmap da Fase 2, com a arquitetura já preparada para recebê-los |
| **Dependência tecnológica** | A integração com o SICAR começa como **adapter mock** (dados de exemplo) e evolui para integração real — a interface está desenhada para trocar a implementação sem afetar o resto do sistema |
| **IA adaptativa** | Além dos tons fixos, a persona é **modelo-agnóstica**: o prompt dita o comportamento, não o LLM. Qualquer modelo aberto (Llama, Mistral, Qwen) produz o mesmo resultado |

Além disso, incorporamos as sugestões da mentora: **gamificação** (barra de progresso), **FAQ contextual** (com tolerância a erros de digitação) e **áudio** entram no MVP. Exemplos práticos de mutirões, Libras e WCAG completo ficam como próximas fases, documentados no roadmap.

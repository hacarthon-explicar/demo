# ExpliCAR — Roteiro de Apresentação (3 minutos)

**Desafio 3 · haCARthon — Aumentar o entendimento das legislações do CAR**

> Roteiro cena a cena. Coluna esquerda = fala do apresentador. Coluna direita = o que mostrar na demonstração navegável (`demonstracao.html`). Tempo total: ~3 min.

---

## Abertura — O problema (0:00 – 0:30)

**Fala:**
> "Seu Raimundo recebe uma carta do SICAR. Três páginas de siglas — APP, Reserva Legal, artigos de lei — e termos que ele nunca ouviu. Ele não sabe se é multa, não sabe o que fazer. E o cadastro fica parado. Por anos. Não por má vontade — por falta de entendimento."

**Mostrar:** Tela **Entrada** — a carta do SICAR com as siglas destacadas em vermelho. Deixe a tensão da burocracia visível.

**Nota:** Conecte com a vivência real: "Nos mutirões da SEMAS, vimos esse mesmo processo parado ser resolvido em 20 minutos de conversa. O gargalo é de comunicação."

---

## O insight (0:30 – 0:50)

**Fala:**
> "A conversa do mutirão funciona porque o técnico traduz a lei na língua do produtor, no tom certo, usando os dados da terra dele. O ExpliCAR digitaliza exatamente isso: o Téo, um técnico que cabe no bolso — e funciona online."

**Mostrar:** Toque em **"Apontar para o QR code"** → animação de leitura → tela de **Identificação**. "Sítio Boa Esperança, 85 hectares, Altamira. Três pendências. Calma — quase nada é multa."

---

## A escolha do tom (0:50 – 1:10)

**Fala:**
> "Antes de explicar, o Téo pergunta como o senhor prefere ouvir. Três tons: direto ao ponto, explicado com calma, ou completo. Vamos de 'explicado com calma'."

**Mostrar:** Toque em **"Entender com o Téo"** → tela de **Escolha do tom** → selecione **"Explicado com calma"**.

---

## A conversa que se ajusta (1:10 – 2:10) — *o coração da demo*

**Fala:**
> "O Téo explica a primeira pendência com a estrutura de sempre: o que significa, por que aconteceu, o que fazer. Tudo com o nome da terra e os dados reais."

**Mostrar:** A primeira explicação aparece (Reserva Legal × matrícula). Aponte para a estrutura em blocos e para a barra **"0 de 3 resolvidas"**.

**Fala:**
> "Se o produtor não entende, ele não precisa pedir. Toca em 'não entendi' — e o Téo simplifica na hora."

**Mostrar:** Toque em **"Não entendi"** → a explicação volta mais simples, com o selo de tom mudando para *Direto ao ponto*.

**Fala:**
> "E quando ele quer ir fundo na lei, é só pedir mais."

**Mostrar:** Em outra pendência, toque em **"Quero saber mais"** → o tom sobe para *Completo*, com base legal.

**Fala:**
> "E a pergunta que mais trava o produtor — 'quanto de mata eu preciso?' — o Téo responde com a conta da terra dele, não uma regra genérica."

**Mostrar:** Toque no chip **"🌿 Quanto de mata eu preciso?"** → aparece o **Resumo Legal Personalizado**: 80% → ZEE 50% → menos de 4 módulos → marco de 2008. "A lei assusta com 80%. Na terra dele, a conta é bem mais leve."

**Fala (rápida):**
> "E se ele digitar errado? O Téo entende mesmo assim."

**Mostrar:** No campo de busca, digite algo com erro (ex.: **"resrva legal"**) → o FAQ responde certo. (FAQ contextual com tolerância a erro.)

**Fala:**
> "A cada item entendido, a barra avança. Reduz a ansiedade. Mostra que está chegando ao fim."

**Mostrar:** Toque em **"Entendi"** nas três pendências → barra vai a **"3 de 3 resolvidas"**.

---

## Áudio e saída (2:10 – 2:40)

**Fala:**
> "Seu Raimundo não enxerga bem, ou prefere ouvir. Cada resposta tem o botão 'Ouvir' — voz processada no servidor, pelo OmniVoice."

**Mostrar:** Toque em **"Ouvir"** em qualquer resposta → painel de áudio com a leitura em voz alta.

**Fala:**
> "No fim, os três passos numerados. Ele salva, ouve, e manda pro filho no WhatsApp. Sai sabendo exatamente o que fazer."

**Mostrar:** **"Ver meu resumo final"** → tela de **Plano** com os 3 passos, Salvar / Ouvir / Enviar.

---

## Diferenciais e fechamento (2:40 – 3:00)

**Fala:**
> "Persona adaptativa, 100% código aberto, LGPD por desenho. O que travava há anos virou três passos no bolso do produtor. Sem sair de casa, sem juridiquês. Esse é o ExpliCAR."

**Mostrar:** (Opcional) Abra **`fluxogramas.html`** na arquitetura: PWA → orquestrador da persona → LLM agnóstico → adapter do SICAR, com a faixa de LGPD.

---

## Checklist de demonstração

- [ ] Antes de apresentar, arraste um mapa real para o slot da tela de Identificação (opcional, dá realismo).
- [ ] Teste o áudio no navegador da apresentação (TTS depende de voz pt-BR instalada).
- [ ] Tenha o erro de digitação ensaiado ("resrva legal" → responde Reserva Legal).
- [ ] Botão **Reiniciar** no topo volta a demo ao começo entre ensaios.

## Pontos de ênfase (se sobrar tempo / em perguntas)

- **Validado em campo:** parte dos mutirões da SEMAS, não de uma hipótese.
- **Modelo agnóstico:** a persona (prompt) controla o comportamento, não o LLM — qualquer modelo aberto serve.
- **Reuso por outros órgãos:** repositório público + Docker Compose; cada estado conecta seu SICAR e seus dados.
- **Roadmap:** Libras, legendas e WCAG completo na Fase 2 — arquitetura já preparada.

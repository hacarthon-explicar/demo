# ExpliCAR

A burocracia do Cadastro Ambiental Rural traduzida para a linguagem de quem vive da terra.

ExpliCAR e um assistente digital que ajuda o pequeno e medio produtor rural a entender notificacoes do SICAR. A partir dos dados do seu imovel, o Teco (tecnico digital) explica cada pendencia em tres niveis de tom, gera um Resumo Legal Personalizado, e guia o produtor passo a passo ate a regularizacao.

**Iniciar a demonstração:** [https://hacarthon-explicar.github.io/demo/](https://hacarthon-explicar.github.io/demo/)

---

## Acesso Rapido

| Pagina | Link |
|---|---|
| Demonstracao Navegavel | [`demonstracao.html`](https://hacarthon-explicar.github.io/demo/demonstracao.html) |
| Fluxogramas do Sistema | [`fluxogramas.html`](https://hacarthon-explicar.github.io/demo/fluxogramas.html) |
| Pitch de Apresentacao | [`pitch.html`](https://hacarthon-explicar.github.io/demo/pitch.html) |
| Roteiro de 3 min | [`docs/roteiro-apresentacao.md`](https://hacarthon-explicar.github.io/demo/docs/roteiro-apresentacao.md) |
| Slides PPTX | [`export/ExpliCAR - Pitch.pptx`](https://hacarthon-explicar.github.io/demo/export/ExpliCAR%20-%20Pitch.pptx) |
| Video de Apresentacao | [assistir no YouTube](https://youtu.be/Fyc4ZCQY7iw) |
| PDF da Apresentacao | [`docs/Apresentação sem título.pdf`](https://hacarthon-explicar.github.io/demo/docs/Apresenta%C3%A7%C3%A3o%20sem%20t%C3%ADtulo.pdf) |

---

## Funcionalidades do MVP

- **Chat com Teo** — o coracao da solucao. Explica cada pendencia com base nos dados reais da propriedade e na legislacao aplicavel.
- **Persona adaptativa** — tres tons de explicacao (Direto ao ponto, Explicado com calma, Completo) com adaptacao por feedback explicito do usuario.
- **Gamificacao** — barra de progresso "X de 3 resolvidas" que reduz a ansiedade e mostra o avanco.
- **Audio OmniVoice** — cada resposta tem um botao "Ouvir" com voz processada no servidor, para quem prefere ouvir.
- **FAQ Contextual** — respostas rapidas com tolerancia a erros de digitacao (fuzzy matching).
- **Resumo Legal Personalizado** — gerado pelo Teo com base nos dados reais do CAR, substituindo calculadoras genericas.

---

## Arquitetura (100% codigo aberto)

```
Mobile-first PWA
  -> Orquestrador da Persona (Teo)
    -> LLM agnostico (Llama / Mistral / Qwen)
      -> Adapter do SICAR (dados do imovel)
  -> Camada de audio (OmniVoice TTS)
  -> Camada LGPD (pseudonimizacao, minimizacao)
```

| Componente | Tecnologia | Licenca |
|---|---|---|
| Frontend | HTML/CSS/JS (DC Framework) | MIT |
| Backend | Python / FastAPI | MIT |
| LLM | Agnostico (Llama / Mistral / Qwen) | Apache 2.0 |
| TTS | OmniVoice (k2-fsa) | Apache 2.0 |
| Banco de Dados | PostgreSQL | PostgreSQL |

---

## Estrutura do Repositorio

```
.
├── index.html              (landing page)
├── demonstracao.html       (demo navegavel)
├── fluxogramas.html        (fluxogramas do sistema)
├── pitch.html              (pitch de apresentacao)
├── deck-stage.js           (componente de slides)
├── image-slot.js           (componente de imagem)
├── assets/                 (logos e recursos visuais)
├── docs/                   (documentacao do projeto)
│   ├── direcional.md
│   ├── ideacao.md
│   ├── persona-tecnico.md
│   ├── plano-demonstracao.md
│   └── roteiro-apresentacao.md
├── data/                   (dados de exemplo / mock SICAR)
├── export/                 (slides PPTX)
└── screenshots/            (capturas de referencia)
```
---

## Proximos Passos (pos-haCARthon)

1. **Desenvolvimento do backend** — FastAPI + LLM auto-hospedado (Llama/Mistral/Qwen) + OmniVoice TTS + PostgreSQL.
2. **Integracao com a API do SICAR** — substituir dados mockados por consultas reais ao cadastro ambiental.
3. **Validacao com usuarios reais** — testar com produtores rurais e tecnicos do CAR para refinar a comunicacao do Teo.
4. **Pessoas e parcerias** — OEMA, FBDS, sindicatos rurais, especialistas em direito ambiental e UX para agricultura familiar.
5. **Seguranca e LGPD** — pseudonimizacao, minimizacao de dados, auditoria, LLM em rede interna.
6. **Recursos financeiros** — estimativa de R$ 50-80 mil para infraestrutura, integracoes e testes de campo.

---

## Sobre o Projeto

**Desafio:** haCARthon -- Desafio 3  
**Foco:** Pequeno e medio produtor rural  
**LGPD:** Pseudonimizacao, minimizacao de dados, LLM em rede interna. O codigo e aberto; os dados, nao.

### Equipe

- **Samuel da Costa dos Santos** -- [github.com/samuel-c-santos](https://github.com/samuel-c-santos)
- **Priscila Motta Gadelha Silva** -- [github.com/primottags](https://github.com/primottags)

### Mentoria

- **Lorrana Nunes** (@lorrana_nunes)

---

## Licenca

MIT License. Veja o arquivo [LICENSE](./LICENSE) para detalhes.

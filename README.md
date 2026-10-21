# 🔬 REA Reverse — Engenharia reversa com IA

![REA](https://img.shields.io/badge/REA-Reverse%20Engineer%20Anything-blue) ![MCP](https://img.shields.io/badge/MCP-Claude%20%7C%20Codex-green) ![Documentação](https://img.shields.io/badge/Documenta%C3%A7%C3%A3o-PT--BR-yellow)

> **Espelho comunitário não oficial.** Código e projeto original: [morluto/rea](https://github.com/morluto/rea). A documentação deste repositório está em português.

O **REA — Reverse Engineer Anything** integra agentes de IA a ferramentas de engenharia reversa por MCP, incluindo análise de binários, APKs, JavaScript/Electron e .NET. Consulte a origem para a cobertura e dependências atualizadas.

## 🚀 Instalação oficial

Com Node.js e npm compatíveis:

```bash
npx rea-agents@latest setup
```

Selecione Claude Code e/ou Codex, revise as alterações propostas, confirme e reinicie o agente.

Para instalar o comando `rea` globalmente:

```bash
npm install --global rea-agents
rea --help
```

## 💻 Exemplo de uso

Após configurar o MCP, solicite ao Claude Code ou Codex:

```text
Analise estaticamente este APK de minha propriedade. Identifique componentes, permissões e fluxos de comunicação. Apresente evidências e limitações sem executar o aplicativo.
```

Exemplo de CLI para aplicativo JavaScript/Electron extraído:

```bash
npx -y rea-agents@latest analyze-javascript-application /caminho/absoluto/do/app --json
```

## 📁 Estrutura

```text
rea_reverse/
├── README.md
├── docs/
│   ├── INSTALACAO.md
│   ├── USO.md
│   └── ORIGEM-E-LICENCAS.md
├── .github/workflows/
│   └── sync-upstream.yml
└── upstream/               # Código oficial após a primeira sincronização
```

## 🔄 Sincronização do código original

O workflow **Sincronizar REA oficial** clona `morluto/rea` para a pasta `upstream/` e preserva os arquivos de documentação desta raiz. A sincronização pode ser acionada na aba **Actions > Sincronizar REA oficial > Run workflow**; também está programada para executar semanalmente. **Verifique o resultado na aba Actions**: a existência do workflow não comprova que o código já foi copiado.

## 📚 Documentação

- [Instalação](docs/INSTALACAO.md)
- [Guia de uso](docs/USO.md)
- [Origem, autoria e licenças](docs/ORIGEM-E-LICENCAS.md)

## ⚖️ Créditos e uso responsável

Projeto original: **[morluto/rea](https://github.com/morluto/rea)**. O REA utiliza licença MIT para o código próprio e inclui avisos de terceiros. Preserve integralmente as licenças do código sincronizado. Utilize as ferramentas somente em sistemas e arquivos que você tem autorização para analisar.

## 🤖 Prompt curto para Claude Code ou Codex — instalação global

```text
Instale e configure globalmente o REA a partir da distribuição oficial morluto/rea (pacote rea-agents). Verifique Node.js/npm, execute npx rea-agents@latest setup, configure a integração MCP e as instruções para Claude Code ou Codex, preserve configurações existentes, valide com rea --help e informe os resultados. Peça confirmação antes de modificar instalações existentes.
```

# Instalação e configuração

## Requisitos
- Node.js compatível com a versão do REA (verifique as exigências no [repositório oficial](https://github.com/morluto/rea)).
- npm e acesso à Internet.
- Claude Code ou Codex instalado, caso queira integração com agente.
- Ferramentas adicionais, como JADX/Ghidra, somente para modalidades de análise que as exigem.

## Setup oficial
```bash
npx rea-agents@latest setup
```

Revise as modificações propostas e escolha o agente. Reinicie o agente ao final.

## CLI global
```bash
npm install --global rea-agents
rea --help
```

## Atualização
```bash
rea update
npx rea-agents@latest setup
```

A instalação é feita pelo pacote oficial; este repositório é um espelho comunitário documentado em português.

# Guia de uso

O REA oferece análise assistida por agentes via MCP e comandos de terminal.

## Exemplo com Claude Code ou Codex
```text
Analise estaticamente este APK de minha propriedade. Identifique componentes, permissões e fluxos de comunicação. Apresente evidências e limitações, sem instalar ou executar a amostra.
```

## Exemplo de CLI
```bash
npx -y rea-agents@latest analyze-javascript-application /caminho/absoluto/do/app --json
```

Para análise nativa ou Android, configure as ferramentas exigidas na documentação oficial. Use em ambientes isolados quando a análise exigir execução. Não utilize dados, credenciais ou dispositivos de terceiros sem autorização.

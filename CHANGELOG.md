# Changelog do Orkestrai

[Português](CHANGELOG.md) · [English](CHANGELOG.en.md) · [Español](CHANGELOG.es.md)

## 0.1.2 — 2026-08-07

- Altera a atualização automática do painel Usage de 60 segundos para 5 minutos.
- Alinha o cache do servidor para evitar consultas duplicadas aos providers.
- Mantém o botão de atualização manual buscando dados novos imediatamente.
- Reduz o risco de respostas HTTP 429 do Claude em sessões longas.

## 0.1.1 — 2026-08-07

- Inclui `electron-updater` no aplicativo instalado.
- Corrige o diagnóstico incorreto de que o auto-update só existe fora do pacote.
- Faz tarefas manuais chegarem ao líder com título, descrição e todas as imagens.
- Instalações `0.0.1` e `0.1.0` precisam instalar esta versão manualmente uma única vez.

## 0.1.0 — 2026-08-07

- Primeira release pública multiplataforma, com manifests e verificação SHA-512.
- Adiciona voz multilíngue local, painel de portas e ditado global para o líder.

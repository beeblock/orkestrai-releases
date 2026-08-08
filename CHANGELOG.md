# Changelog do Orkestrai

[Português](CHANGELOG.md) · [English](CHANGELOG.en.md) · [Español](CHANGELOG.es.md)

## 0.1.4 — 2026-08-08

- Primeira release macOS assinada com Developer ID Application e notarizada pela Apple.
- Valida autoridade, Team ID, Hardened Runtime, Gatekeeper e ticket de notarização antes de publicar as versões Apple Silicon e Intel.
- Remove os alertas de aplicativo danificado ou desenvolvedor não verificado dos novos downloads para Mac.
- Usuários Mac na `0.1.3` ou anterior precisam instalar a `0.1.4` manualmente uma vez; as próximas versões assinadas podem atualizar pelo próprio app.
- Publica a mesma release nos feeds legado e principal para preparar a migração das atualizações futuras.

## 0.1.3 — 2026-08-07

- Corrige a assinatura ad-hoc parcial dos pacotes macOS `0.1.2`, que o Gatekeeper reportava como aplicativo danificado.
- Adiciona assinatura completa e validação profunda dos bundles, DMGs e ZIPs macOS antes da publicação.
- Bloqueia a substituição automática no Mac sem Developer ID e preserva a instalação atual.
- No primeiro uso do pacote ad-hoc, tente abrir o app, feche o aviso e use Ajustes do Sistema → Privacidade e Segurança → Segurança → **Abrir Mesmo Assim**; autentique e confirme **Abrir**. Windows não foi afetado.

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

# Changelog do Orkestrai

[Português](CHANGELOG.md) · [English](CHANGELOG.en.md) · [Español](CHANGELOG.es.md)

## 0.5.2 — 2026-08-10

- Permite gravações de ditado local de aproximadamente 15 minutos, sem falhar no antigo limite de 512 KB do servidor empacotado.
- Restaura Portais salvos automaticamente quando o dev server local inicia depois do canvas e aguarda a página real antes da automação.
- Reserva IDs de conversa distintos para agentes Claude concorrentes, evitando transcripts trocados e respostas corrompidas.
- Preserva erros úteis dos Portais e nunca envia redraw bruto da TUI como resposta de provider.
- Não injeta roles novamente na retomada e acorda apenas agentes com tarefas atribuídas ainda abertas ou o líder quando há trabalho sem responsável.
- Mantém o servidor respondendo enquanto o macOS aguarda a permissão da pasta do workspace e repete com segurança o provisionamento interrompido.

## 0.5.1 — 2026-08-10

- Descarta IDs locais de PTY obsoletos após reiniciar o app e preserva o ID da conversa de cada provider.
- Recria os terminais e retoma suas conversas automaticamente, em vez de deixar todos os nós com erro de sessão inexistente.
- Torna a recuperação determinística com um código WebSocket estável e persistência do ID da sessão substituta.

## 0.5.0 — 2026-08-10

- Adiciona ditado local em todos os campos editáveis, mantendo o líder do canvas como fallback quando não há campo em foco.
- Permite trocar o provider de um agente sem perder role, andar, layout ou conexões do membro.
- Expande as roles dos presets em protocolos operacionais completos e as aplica automaticamente ao iniciar a PTY.
- Entrega ao líder os briefings completos das tarefas sem responsável no startup e exige delegação primeiro pelo kanban.
- Distingue tarefa concluída, projeto concluído e atenção nas notificações nativas.
- Mostra títulos, etapas e responsáveis das tarefas em Andares e corrige a edição de texto grande nas formas.

## 0.4.0 — 2026-08-09

- Adiciona Cursor, Antigravity e Cline como providers nativos ao lado de Claude, Codex, Kimi e OpenCode.
- Adiciona a Central de Providers com detecção local, setup por sistema, login oficial, modelos, esforço e retomada.
- Define inglês como padrão nas novas instalações e pergunta primeiro o idioma no onboarding.
- Inicia terminais de presets com as flags autônomas de acesso total e repara terminais padrão antigos com segurança.

## 0.3.0 — 2026-08-09

- Adiciona até dez etapas personalizadas de kanban compartilhadas entre UI, CLI, MCP, líder e equipe.
- Adiciona presets completos de Campanha, Brand e design e Conteúdo e SEO para times multidisciplinares.
- Adiciona o time de consenso Orkestrai Contributing com Claude, Codex, Kimi e agentes especialistas.

## 0.2.0 — 2026-08-09

- Adiciona a Biblioteca de presets com times prontos de Produto, React, Next.js, SvelteKit, Svelar e Laravel.
- Adiciona doze roles especialistas instaláveis e skills portáteis nos presets.
- Adiciona a visão operacional de Andares e menus desktop nativos traduzidos.
- Atualiza Configurações e Documentação com o sistema visual do produto.

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

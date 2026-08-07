# Orkestrai Releases

**Português** · [English](README.en.md) · [Español](README.es.md)

Downloads oficiais do Orkestrai para macOS, Windows e Linux.

Histórico de mudanças: [CHANGELOG.md](CHANGELOG.md).

## Baixar

Acesse a [release mais recente](https://github.com/beeblock/orkestrai-releases/releases/latest)
e escolha o arquivo da sua plataforma:

- **macOS Apple Silicon** (M1/M2/M3/M4): `Orkestrai-*-arm64.dmg`
- **macOS Intel**: `Orkestrai-*.dmg` sem `arm64` no nome
- **Windows 64-bit**: `Orkestrai-Setup-*.exe`
- **Linux 64-bit**: `Orkestrai-*.AppImage`

No macOS sem assinatura Apple, arraste o Orkestrai para Aplicativos e, no
primeiro uso, clique com Control/botão direito no app e escolha **Abrir**. Não
use os pacotes macOS `0.1.2`; a assinatura interna deles foi corrigida na
`0.1.3`.

Arquivos `*.zip`, `*.blockmap` e `latest*.yml` são usados pela atualização
automática do aplicativo. Para instalação manual, use DMG, EXE ou AppImage.

## Atualizações automáticas

O Orkestrai verifica este repositório ao iniciar e novamente a cada seis horas.
O download é validado pelo SHA-512 publicado nos manifests antes de a nova
versão substituir a anterior. Workspaces, configurações e modelos de voz ficam
no diretório de dados do usuário e não são removidos durante uma atualização.

No macOS sem assinatura Apple, o aplicativo detecta a nova release, mas usa
download manual e nunca remove a instalação atual. Windows e Linux suportam a
troca automática pelos instaladores publicados aqui.

As versões `0.0.1` e `0.1.0` foram empacotadas sem o módulo de atualização.
Instale a `0.1.1` manualmente uma única vez para habilitar o fluxo corrigido.

Site: [orkestrai.app](https://orkestrai.app)

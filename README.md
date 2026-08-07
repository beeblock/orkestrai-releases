# Orkestrai Releases

Downloads oficiais do Orkestrai para macOS, Windows e Linux.

## Baixar

Acesse a [release mais recente](https://github.com/beeblock/orkestrai-releases/releases/latest)
e escolha o arquivo da sua plataforma:

- **macOS Apple Silicon** (M1/M2/M3/M4): `Orkestrai-*-arm64.dmg`
- **macOS Intel**: `Orkestrai-*.dmg` sem `arm64` no nome
- **Windows 64-bit**: `Orkestrai Setup *.exe`
- **Linux 64-bit**: `Orkestrai-*.AppImage`

Arquivos `*.zip`, `*.blockmap` e `latest*.yml` são usados pela atualização
automática do aplicativo. Para instalação manual, use DMG, EXE ou AppImage.

## Atualizações automáticas

O Orkestrai verifica este repositório ao iniciar e novamente a cada seis horas.
O download é validado pelo SHA-512 publicado nos manifests antes de a nova
versão substituir a anterior. Workspaces, configurações e modelos de voz ficam
no diretório de dados do usuário e não são removidos durante uma atualização.

No macOS sem assinatura Apple, o aplicativo pode direcionar para o download
manual. Windows e Linux suportam a troca automática pelos instaladores
publicados aqui.

Site: [orkestrai.app](https://orkestrai.app)

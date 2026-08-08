# Orkestrai Releases

**Português** · [English](README.en.md) · [Español](README.es.md)

Este é o feed público de downloads do Orkestrai durante a transição do
repositório principal. A release assinada `0.1.4` permanece aqui como ponte para
instalações existentes e como download oficial enquanto o novo destino não fica
público.

Histórico de mudanças: [CHANGELOG.md](CHANGELOG.md).

## Baixar

Acesse a [release mais recente](https://github.com/beeblock/orkestrai-releases/releases/latest)
e escolha o arquivo da sua plataforma:

- **macOS Apple Silicon** (M1/M2/M3/M4): `Orkestrai-*-arm64.dmg`
- **macOS Intel**: `Orkestrai-*.dmg` sem `arm64` no nome
- **Windows 64-bit**: `Orkestrai-Setup-*.exe`
- **Linux 64-bit**: `Orkestrai-*.AppImage`

No macOS sem assinatura Apple, arraste o Orkestrai para Aplicativos, tente
abri-lo e feche o aviso. Depois abra **Ajustes do Sistema → Privacidade e
Segurança**, desça até **Segurança**, clique em **Abrir Mesmo Assim**, autentique
e confirme **Abrir**. O botão aparece por cerca de uma hora após a tentativa.
Não use os pacotes macOS `0.1.2`; a assinatura interna deles foi corrigida na
`0.1.3`.

Se o botão não aparecer, tente abrir o app novamente. Como último recurso para
o pacote baixado desta página, execute no Terminal:

```bash
sudo xattr -rd com.apple.quarantine "/Applications/Orkestrai.app"
open "/Applications/Orkestrai.app"
```

Arquivos `*.zip`, `*.blockmap` e `latest*.yml` são usados pela atualização
automática do aplicativo. Para instalação manual, use DMG, EXE ou AppImage.

## Atualizações automáticas

Versões até `0.1.3` verificam este repositório ao iniciar e novamente a cada seis
horas. A `0.1.4` migra o aplicativo para o feed do repositório principal.
O download é validado pelo SHA-512 publicado nos manifests antes de a nova
versão substituir a anterior. Workspaces, configurações e modelos de voz ficam
no diretório de dados do usuário e não são removidos durante uma atualização.

No macOS sem assinatura Apple, o aplicativo detecta a nova release, mas usa
download manual e nunca remove a instalação atual. Windows e Linux suportam a
troca automática pelos instaladores publicados aqui.

As versões `0.0.1` e `0.1.0` foram empacotadas sem o módulo de atualização.
Instale a `0.1.1` manualmente uma única vez para habilitar o fluxo corrigido.

Site: [orkestrai.app](https://orkestrai.app)

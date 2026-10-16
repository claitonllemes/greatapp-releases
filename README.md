# GreatPages para Mac

<p>
  <a href="https://github.com/claitonllemes/greatapp-releases/releases/latest"><img alt="Última versão" src="https://img.shields.io/github/v/release/claitonllemes/greatapp-releases?label=vers%C3%A3o&color=4b91f7"></a>
  <img alt="macOS 11 ou superior" src="https://img.shields.io/badge/macOS-11%2B-black">
  <img alt="Apple Silicon" src="https://img.shields.io/badge/Apple%20Silicon-M1%20ou%20mais%20recente-black">
</p>

O aplicativo de desktop da [GreatPages](https://www.greatpages.com.br): o painel e o editor em abas, com a sua sessão salva entre uma abertura e outra.

## Baixar

**[Baixar a última versão](https://github.com/claitonllemes/greatapp-releases/releases/latest)**: na página, em **Assets**, escolha o arquivo `GreatPages_<versão>_aarch64.dmg`.

Requisitos:

- macOS 11 ou superior.
- Mac com chip Apple Silicon (M1 ou mais recente). Macs com processador Intel não são suportados.

## Instalar

1. Abra o `.dmg` e arraste o **GreatPages** para a pasta **Aplicativos**.
2. Abra o app. Na primeira vez o macOS vai bloquear a abertura, porque o app não é assinado com um Developer ID da Apple. Para liberar:
   - **macOS 15 ou superior:** tente abrir o app, vá em **Ajustes do Sistema → Privacidade e Segurança**, role até a mensagem sobre o GreatPages e clique em **Abrir Mesmo Assim**.
   - **macOS 14 ou anterior:** clique com o botão direito no app, escolha **Abrir** e confirme.
3. Entre na sua conta GreatPages. Isso só é necessário na primeira abertura.

O passo 2 é feito uma única vez. Depois disso o app abre normalmente.

## Atualizações

O app se atualiza sozinho:

- Ao abrir, ele verifica se há uma versão nova. Se houver, mostra as novidades e pergunta se você quer **Atualizar e reiniciar** ou deixar para **Depois**.
- Para verificar na hora, use a engrenagem da barra de abas e escolha **Verificar atualizações**.
- Cada atualização é assinada digitalmente, e o app só instala arquivos que confere com a chave de assinatura.

Você não precisa baixar o `.dmg` de novo para atualizar. Ele serve para uma instalação nova.

## Novidades de cada versão

As notas ficam na página de cada [release](https://github.com/claitonllemes/greatapp-releases/releases) e também aparecem dentro do app, no diálogo de atualização.

## Seus dados no Mac

- A sessão (cookies e armazenamento das páginas) fica no armazenamento do WebKit, o motor de navegação do macOS. O app não usa o Chaves do macOS.
- Os registros de funcionamento (logs) ficam em `~/Library/Logs/com.greatpages.app`, um arquivo por dia, e são apagados depois de 7 dias.
- Arquivos baixados nas abas são salvos em `~/Downloads`.

### Desinstalar

Arraste o **GreatPages** de **Aplicativos** para o Lixo. Para apagar também os dados do app, remova estas pastas e este arquivo:

- `~/Library/Application Support/com.greatpages.app`
- `~/Library/WebKit/com.greatpages.app`
- `~/Library/Caches/com.greatpages.app`
- `~/Library/Logs/com.greatpages.app`
- `~/Library/Preferences/com.greatpages.app.plist`

## Sobre este repositório

Aqui ficam apenas os arquivos de cada versão (instalador, pacote de atualização e `latest.json`, lido pelo app para saber se há atualização). Não há código-fonte neste repositório.

Site: [www.greatpages.com.br](https://www.greatpages.com.br)

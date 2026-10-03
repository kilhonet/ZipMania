# ZipMania

**Um compactador gratuito para Windows, rápido e leve, que abre mais de 50 formatos e compacta em 7Z · ZIP · TAR.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · Português (Brasil) · [Français](README.fr.md)

> Este documento é uma tradução. Em caso de divergência, prevalece a [versão em coreano](README.ko.md).

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20x64-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Source](https://img.shields.io/badge/source-Apache%202.0-lightgrey)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/zipmania?lang=pt)

![Captura de tela do ZipMania](images/zipmania-en.webp)

## Visão geral

O ZipMania é um compactador focado em uma coisa: abrir e criar arquivos compactados. Ele lê mais de 50 formatos, incluindo ZIP, RAR, 7Z, EGG, ALZ e ISO, e cria arquivos em **7Z · ZIP · TAR**.

Ao abrir um arquivo, você vê a árvore de pastas à esquerda e a lista de arquivos à direita. Escolha só os arquivos de que precisa e extraia, ou arraste-os direto para o Explorador. Imagens são pré-visualizadas sem extrair. Um clique duplo abre o arquivo no programa associado, e um arquivo compactado dentro de outro abre em uma nova janela.

O menu de contexto do Explorador oferece ações de um clique, como "Extrair aqui" e "Compactar em *nome*.zip", e uma ferramenta de linha de comando (`zm.exe`) acompanha o programa para scripts de backup e programas externos como o Total Commander. Sem anúncios e sem software embutido.

## Recursos

- **Abre mais de 50 formatos** — ZIP, ZIPX, JAR, RAR, 7Z, EGG, ALZ, TAR, GZ, BZ2, XZ, ZST, ISO, IMG, WIM, DMG, MSI, RPM, DEB, CAB, CBZ, CBR e outros.
- **Compacta em 7Z · ZIP · TAR** — cinco níveis de compactação, senhas, criptografia de nomes de arquivo em 7Z, arquivos divididos.
- **ZIP rápido** — um mecanismo dedicado cuida da compactação e da extração de ZIP.
- **Só o que você precisa** — extraia os arquivos selecionados, arraste-os para o Explorador ou abra com clique duplo.
- **Arquivos dentro de arquivos** — clique duplo para abrir em uma nova janela.
- **Pré-visualização de imagens** — JPG, PNG, GIF, WebP, SVG e mais, no painel inferior esquerdo, sem extrair.
- **Edição de arquivos** — adicione ou exclua arquivos em 7Z, ZIP e TAR.
- **Verificar · Analisar** — uma tabela CRC mostra se o arquivo está danificado, e o antivírus do Windows (AMSI) pode analisar os arquivos internos.
- **Limpeza após compactar** — verifica o arquivo ao terminar e exclui os originais só se ele passar.
- **Menu de contexto do Explorador** — Extrair aqui, Extrair em *nome*, Compactar em *nome*.zip, Compactar cada um separadamente, Extrair cada um em sua pasta.
- **Linha de comando** — `zm.exe` (console) e `ZipMania.exe` (janela de progresso) para compactar, extrair, listar e testar. Aceita a sintaxe de opções do 7-Zip e do Bandizip.
- **Tema claro/escuro, 9 idiomas** — segue o Windows por padrão, ou escolha o seu.

## Download / Instalação

| Pacote | Link |
|---|---|
| Instalador | [Baixar](https://down.kilho.net/zipmania?lang=pt) |
| Portátil (ZIP) | [Baixar](https://down.kilho.net/zipmania?lang=pt&nosetup) |

O ZipMania pode ser usado como aplicativo portátil: descompacte em qualquer lugar e execute `ZipMania.exe`. As configurações ficam em `settings.toml` ao lado do executável, então acompanham você em um pen drive.

## Como usar

### Primeiros passos

**Extrair**

1. Dê um clique duplo em um arquivo compactado, abra um com **[Abrir]** no ZipMania ou solte-o na janela.
2. Navegue pela árvore de pastas à esquerda e pela lista de arquivos à direita. Selecione arquivos e clique em **[Extrair]**.
3. Na janela **Extrair**, escolha a pasta de destino. Use os atalhos à esquerda (Área de Trabalho, Documentos, Downloads…) ou a árvore de pastas; clique com o botão direito em um espaço vazio para criar uma nova pasta.
4. Em **Arquivos a extrair** escolha **Todos os arquivos** ou **Arquivos selecionados** e clique em **[OK]**. Progresso, velocidade e tempo restante são exibidos; ao terminar, **[Abrir pasta]** leva você ao resultado.

**Compactar**

1. Clique em **[Novo arquivo]** na barra de ferramentas ou solte arquivos e pastas na janela do ZipMania.
2. A janela **Novo arquivo** os lista. Adicione mais com **[Adicionar arquivos]** / **[Adicionar pastas]** ou arrastando-os.
3. Defina o **Nome do arquivo** (local de salvamento), o **Formato** (7Z · ZIP · TAR) e, se necessário, **Definir senha**, **Dividir**, as ações de **Depois** e o **Método**.
4. Clique em **[Iniciar]**. Ao terminar, **[Abrir pasta]** ou **[Fechar]**.

Para fazer isso direto no Explorador, use o menu de contexto — veja "Como…" abaixo.

### A janela

| Botão da barra | O que faz |
|---|---|
| **Abrir** | Abrir um arquivo compactado |
| **Extrair** | Extrair o arquivo aberto (ou só os arquivos selecionados) |
| **Novo arquivo** | Escolher arquivos e pastas e criar um novo arquivo |
| **Adicionar arquivos** / **Excluir arquivos** | Colocar ou remover arquivos do arquivo aberto (somente 7Z · ZIP · TAR) |
| **Verificar** | Checar se o arquivo está danificado (CRC) |
| **Analisar** | Analisar os arquivos internos com o antivírus do Windows (arquivos com menos de 10 MB) |
| **Visão plana** | Mostrar todos os arquivos em uma única lista com o caminho completo, sem pastas |
| **Configurações** | Tema, idioma, padrões de extração, associações de arquivo, menu do Explorador |

- **Árvore de pastas (superior esquerdo)** — clique em uma pasta para ver seus arquivos à direita.
- **Pré-visualização (inferior esquerdo)** — aparece quando um único arquivo de imagem está selecionado.
- **Lista de arquivos** — Nome · Tamanho · Tamanho compactado · Tipo · Modificado. Clique no cabeçalho Nome, Tamanho ou Modificado para ordenar; arraste as bordas para redimensionar as colunas.
- **Barra de status** — número de itens, quantidade e tamanho dos arquivos selecionados, tamanho compactado e taxa.
- Arraste o divisor para redimensionar a árvore e a lista. O tamanho da janela e o estado maximizado são restaurados na próxima vez.

### Como…

**Extrair direto do Explorador**
Clique com o botão direito em um arquivo compactado para ver as entradas do ZipMania.
- **Extrair aqui** — extrai na própria pasta do arquivo sem perguntar. Ative **Fechar janela** na janela de progresso para que ela feche assim que terminar.
- **Extrair em "nome"** — cria uma nova pasta com o nome do arquivo e extrai nela. Ideal para arquivos com muitos itens.
- **Extrair com ZipMania…** — abre a janela onde você escolhe o destino e as opções.
- **Abrir com ZipMania** — veja o conteúdo primeiro.

Com **vários arquivos selecionados**, **Extrair aqui** extrai um após o outro, e **Extrair cada um em sua pasta** coloca cada arquivo em uma pasta com o próprio nome.

**Compactar direto do Explorador**
Clique com o botão direito em arquivos ou pastas.
- **Compactar em "nome.zip"** — cria um ZIP ali mesmo sem perguntar. Uma pasta recebe o nome da pasta; vários itens recebem o nome da pasta atual. Se o nome já existir, um número é adicionado: `nome (2).zip`.
- **Compactar com ZipMania** — abre a janela para escolher formato, senha, divisão e assim por diante.
- **Compactar cada um separadamente** — cria um ZIP por item selecionado, com o nome dele. Útil para arquivar várias pastas individualmente.

**Tirar só alguns arquivos de um arquivo compactado**
Três maneiras:
- Selecione os arquivos (Ctrl/Shift para vários) e clique em **[Extrair]** → **Arquivos a extrair: Arquivos selecionados**.
- Clique com o botão direito na seleção → **Extrair arquivos selecionados**.
- **Arraste a seleção para o Explorador ou para a área de trabalho** — ela é extraída ali mesmo.

**Abrir um arquivo interno sem extrair**
Dê um clique duplo ou pressione Enter; ele abre no programa associado (documentos no seu editor, vídeos no seu player). Botão direito → **Executar arquivo** faz o mesmo. As cópias temporárias são limpas quando você fecha o ZipMania.

**Um arquivo compactado dentro de outro**
Dê um clique duplo e ele abre em uma **nova janela**. Você pode manter várias janelas abertas e alternar entre elas.

**Folhear fotos dentro de um arquivo**
Selecione um arquivo de imagem (JPG · PNG · GIF · BMP · WebP · ICO · SVG · TIFF · AVIF) e a pré-visualização aparece no canto inferior esquerdo. Use as setas para percorrê-las. Imagens com mais de 32 MB mostram um aviso em vez da pré-visualização.

**Pastas profundas dificultam encontrar arquivos**
Ative **[Visão plana]** na barra: as pastas somem e cada arquivo é listado com o caminho. Ordene por nome, tamanho ou data para encontrar de imediato os arquivos maiores ou mais recentes. Clique de novo para voltar à visão de pastas.

**Arquivos protegidos por senha**
Um pedido de senha aparece ao abrir. Uma senha errada pergunta de novo; uma correta é lembrada para aquele arquivo, então pré-visualizar, abrir e extrair não perguntam mais. Se um arquivo protegido aparecer durante a extração, a senha é pedida na hora; deixe em branco e só aquele arquivo é pulado enquanto o resto continua.

**Compactar com senha**
Na janela **Novo arquivo** clique em **[Definir senha]** e digite.
- Com **7Z** você também pode ativar **Criptografar nomes de arquivo** — sem a senha ninguém consegue nem ver o que há dentro.
- **ZIP** aceita apenas letras e dígitos. Uma senha não ASCII mostra um aviso e não inicia — mude para 7Z ou use uma senha ASCII.
- **TAR** não suporta senhas.

**Enviar um arquivo grande por e-mail ou mensageiro**
Em **Dividir** escolha 10 MB · 25 MB · 100 MB · 700 MB · 1 GB · 4 GB, ou escolha **Personalizado…** e digite algo como `700M` ou `4GB`. O arquivo é salvo como `nome.7z.001`, `.002`, … (7Z · ZIP). Quem recebe coloca as partes em uma pasta e abre ou extrai **somente o arquivo `.001`**.

**Excluir os originais depois de compactar para liberar espaço**
Em **Depois** ative **Verificar arquivo** e **Excluir originais**. Os originais só são excluídos quando todos os arquivos foram armazenados e a verificação passou, então um arquivo defeituoso nunca custa os originais.

**Compactar várias pastas separadamente**
Coloque as pastas na janela **Novo arquivo** e ative **Compactar cada item em seu próprio arquivo**. Cada pasta recebe um arquivo com o próprio nome, ao lado dela. É o mesmo que **Compactar cada um separadamente** do Explorador, mas aqui você também escolhe o formato e uma senha.

**Mais rápido ou menor**
**Método** tem cinco níveis: **Armazenar (sem compactação)** · **Rápido** · **Normal** · **Alto** · **Máximo**. Para apenas juntar fotos ou vídeos já compactados, **Armazenar** é o mais rápido; para documentos e código-fonte, que reduzem bem, **Alto** ou **Máximo** compensa. Para o menor resultado use o formato **7Z** (o padrão).

**Adicionar ou remover arquivos de um arquivo existente**
Com um arquivo 7Z · ZIP · TAR aberto:
- Clique em **[Adicionar arquivos]** ou solte arquivos na janela — responda Sim a "Adicionar N arquivo(s) a …?".
- Selecione arquivos e clique em **[Excluir arquivos]** ou botão direito → **Excluir arquivos**.
Outros formatos (RAR, EGG, …) não podem ser editados, então os botões ficam desativados.

**Conferir se um arquivo baixado está íntegro**
Clique em **[Verificar]**: o CRC esperado e o real de cada arquivo são comparados e mostrados em uma tabela. Arquivos danificados ou baixados parcialmente são detectados antes da extração.

**Conferir se um arquivo baixado é seguro**
**[Analisar]** entrega os arquivos internos ao antivírus do Windows (AMSI) sem extraí-los. Arquivos de 10 MB ou mais são pulados, e é preciso um antivírus com proteção em tempo real ativa. O resultado lista cada arquivo como Limpo · Ameaça · Pulado.

**Já existe um arquivo com o mesmo nome ao extrair**
Você é perguntado por arquivo: **Sobrescrever** · **Pular** · **Renomear**. Ative **Aplicar a todos os arquivos restantes** para usar a mesma resposta no resto.

**A extração espalhou arquivos pela pasta**
**Criar uma subpasta com o nome do arquivo** vem ativado por padrão, então os arquivos vão para uma pasta com o nome do arquivo compactado. Para extrair diretamente, desative na janela **Extrair** ou em **Configurações → Extração**, ou use **Extrair aqui** do Explorador.

**Excluir o arquivo e abrir a pasta ao terminar**
Em **Configurações → Extração** ative **Excluir o arquivo após extração bem-sucedida**, **Abrir a pasta de destino após extrair** e **Fechar a janela de extração após extrair**. Também podem ser alterados na janela Extrair a cada vez. O arquivo só é excluído quando a extração foi bem-sucedida.

**Fazer o clique duplo abrir arquivos no ZipMania**
Marque as extensões em **Configurações → Associação de arquivos**. Se outro programa já for dono de uma extensão, aparece **[Não aplicado]**; clique para abrir o seletor de aplicativos padrão do Windows e escolher o ZipMania. Quando o ZipMania abre um arquivo e mostra no topo "Tornar o ZipMania o aplicativo padrão para arquivos …?", você pode trocar ali mesmo.

**O ZipMania não aparece no menu de contexto**
Em **Configurações → Menu do Explorador** ative **Adicionar compactar/extrair do ZipMania ao menu de contexto do Explorador**. No Windows 11 ele aparece no menu principal; se não o vir, procure em **Mostrar mais opções** (Shift+F10).

**Abrir a pasta do arquivo / excluir o arquivo**
Clique com o botão direito em um espaço vazio da lista para **Abrir pasta do arquivo** e **Excluir arquivo**. Depois de conferir o conteúdo, você pode excluir um arquivo de que não precisa mais sem sair do ZipMania.

**Controlar a lista pelo teclado**
Setas · Page Up/Down · Home/End para mover, Shift para um intervalo, Ctrl+clique para adicionar itens avulsos, **Ctrl+A** para selecionar tudo, Enter para entrar em uma pasta ou abrir um arquivo, Esc para fechar a caixa de senha ou de relatório.

**Modo escuro e idioma**
Ambos seguem o Windows por padrão. Em **Configurações → Geral** escolha o tema (Sistema · Claro · Escuro) e o idioma (한국어 · English · 日本語 · 中文 · Русский · Italiano · Français · Español · العربية); as alterações se aplicam na hora. O menu do Explorador usa o mesmo idioma.

**Scripts de backup e Total Commander**
Dois executáveis são fornecidos.
- **`zm.exe`** — escreve no console. cmd, PowerShell e arquivos em lote esperam ele terminar e recebem um código de saída (0 sucesso / 1 aviso / 2 erro).
- **`ZipMania.exe`** — executa os mesmos comandos com uma **janela de progresso**. Adequado a lugares sem console, como o Total Commander.

```
<exe> a|c [opções] <arquivo> <entradas...>   compactar (a adiciona a um arquivo existente)
<exe> x|e [opções] <arquivo> [itens...]      extrair (x mantém pastas, e só arquivos)
<exe> bx  [opções] <arquivos...>             extrair cada arquivo em uma pasta com o próprio nome
<exe> l   [opções] <arquivo>                 listar
<exe> t   [opções] <arquivo>                 teste de integridade
```

| Opção | Significado |
|---|---|
| `-l:0..9` / `-mx9` | Nível de compactação |
| `-fmt:zip\|7z\|tar` / `-t7z` | Formato (padrão: pela extensão do arquivo) |
| `-v:700M` / `-v700m` | Tamanho do volume |
| `-p:senha` / `-psenha` | Senha |
| `-o:pasta` / `-opasta` | Pasta de destino |
| `-target:auto\|name\|none` | Extrair em uma subpasta com o nome do arquivo (`auto` = só quando há mais de um item de nível superior) |
| `-aoa` `-y` / `-aos` / `-aou` | Se o nome coincidir: sobrescrever / pular / salvar como `nome (2)` |
| `-testdst` | Verificar o arquivo após compactar |
| `-delsrc` / `-sdel` | Excluir os originais quando a verificação passar |
| `-date` | Substituir `%Y %y %m %d %H %M %S` no nome pela hora atual |

Exemplos:

```
zm c -l:9 -fmt:7z -testdst -delsrc -date "backup_%y%m%d_%H%M.7z" "D:\Work"   backup 7Z com data, verificar e excluir originais
zm a -mx9 -psecret backup.7z D:\Work                                       sintaxe 7-Zip, adicionar a um arquivo existente
zm x -o:D:\Out -target:auto backup.7z                                      extrair em uma pasta com o nome do arquivo
zm bx a.zip b.7z                                                            extrair em a\ e b\ respectivamente
zm l backup.7z.001                                                          listar a primeira parte de um arquivo dividido
```

Execute `zm` sem argumentos para ver a ajuda. Dentro de um arquivo em lote escreva `%` como `%%`. Para um comando de usuário do Total Commander, defina o comando como `zm.exe` e os parâmetros como `c -l:9 -fmt:7z -aou -testdst -delsrc -date "%T%S %y%m%d_%H%M".7z "%P%S"` para compactar os itens selecionados em um 7Z com data na pasta do painel oposto.

## Configuração

Tudo é alterado em **Configurações** (botão mais à direita da barra) e salvo imediatamente. **[Redefinir]** restaura todos os padrões.

| Categoria | Item | Padrão |
|---|---|---|
| Geral | Tema (Sistema · Claro · Escuro) | Sistema |
| Geral | Idioma (Sistema + 9 idiomas) | Sistema |
| Extração | Criar uma subpasta com o nome do arquivo | Ligado |
| Extração | Excluir o arquivo após extração bem-sucedida | Desligado |
| Extração | Abrir a pasta de destino após extrair | Desligado |
| Extração | Fechar a janela de extração após extrair | Desligado |
| Associação de arquivos | Extensões abertas no ZipMania com clique duplo (zip · 7z · rar · tar · gz · tgz · bz2 · xz · egg · alz · cbz) | Associadas pelo instalador |
| Menu do Explorador | Adicionar compactar/extrair do ZipMania ao menu de contexto do Explorador | Ativado pelo instalador |

As caixas **Fechar janela** e **Abrir pasta** das janelas Novo arquivo e Extrair lembram sua última escolha.

## Requisitos

- Windows 10 ou Windows 11, **64 bits**
- Nenhum runtime ou componente adicional é necessário.
- A Internet é usada apenas para verificar se há uma nova versão. Compactar e extrair funcionam offline.

## Atualizações

O ZipMania **não** se atualiza sozinho. Ao iniciar, ele verifica se há uma nova versão e apenas avisa; novas versões são publicadas manualmente após verificação interna e anunciadas na [página do ZipMania](https://kilho.net/zipmania). Veja o [aviso sobre a política de atualizações](https://en.kilho.net/archives/notice/2940).

## Compilar a partir do código-fonte

O código é público em [github.com/newkilho/ZipMania](https://github.com/newkilho/ZipMania) (Rust 1.88 ou superior). O mecanismo de arquivos, `crates/zipmania-archive`, compila e testa somente com o repositório:

```
cargo test -p zipmania-archive
```

O aplicativo (`app/`) depende de um mecanismo gráfico próprio e de bibliotecas compartilhadas fora do repositório, portanto o executável não pode ser compilado apenas com o repositório.

## Contribuindo

Relatos de bugs e sugestões são bem-vindos via GitHub Issues ou pelo [fórum](https://kilho.top/forum/qna).

## Licença

O programa ZipMania é **Freeware**. Use-o em qualquer lugar — em casa, no trabalho, em escolas e em órgãos públicos — e redistribua-o livremente em sua forma não modificada.

O código-fonte é licenciado sob a **Apache License 2.0**; os crates reutilizáveis em `crates/` estão disponíveis sob MIT ou Apache-2.0, à sua escolha. Os nomes "ZipMania" e "집매니아" e os logotipos e ícones são marcas da Kilho.net e não são cobertos pela licença — distribua versões modificadas com outro nome e ícone. Os componentes de código aberto, incluindo o `7z.dll` do 7-Zip (LGPL), estão listados em `THIRD-PARTY-NOTICES.txt` no repositório.

## Links

- Site: <https://kilho.net/zipmania>
- Código-fonte: <https://github.com/newkilho/ZipMania>
- Fórum: <https://kilho.top/forum/qna>
- X (Twitter): <https://www.twitter.com/kilhonet>

© KILHO.NET

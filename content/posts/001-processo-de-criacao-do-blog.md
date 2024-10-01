+++
title = 'Criando blog com HUGO'
date = 2024-10-01T15:41:04-03:00
draft = true
author = "Levi Vieira"
showToc = true
TocOpen = false
hidemeta = false
comments = false
description = "Compartilhando minha experiência na criação do blog com o framework Hugo."
canonicalURL = ""
disableHLJS = true
disableShare = false
hideSummary = false
searchHidden = false
ShowReadingTime = true
ShowBreadCrumbs = true
ShowPostNavLinks = true
ShowWordCount = true
ShowRssButtonInSectionTermList = true
UseHugoToc = true
+++

Olá, pessoal! 👋🏾

Neste post, quero compartilhar um pouco sobre **como criei meu blog** utilizando o framework **Hugo** e o tema **PaperMod**. 

Este projeto foi inspirado por minha amiga **[Jennifer Oenning](https://www.instagram.com/jenniferoenning/)**, que me ajudou a tirar algumas dúvidas e até fez um vídeo no YouTube explicando o processo de criação.

## O que é HUGO? ☄️

O **Hugo** é um **framework de geração de sites estáticos** escrito em **Go**. Ele permite criar blogs e sites de forma rápida e eficiente, oferecendo uma variedade de temas e opções de personalização.

Hugo pega arquivos content *Markdown*, os executa através de templates de temas e **gera arquivos HTML** que você pode facilmente distribuir online.

Em termos de desempenho bruto, Hugo é o melhor gerador de site estático do mundo. Ele pode render um site de 10.000 páginas em 10 segundos, sendo não só  o SSG mais rápido em termos de tempo de construção, como também é rápido de instalar.

## Facilidade de Criação com Hugo

Um dos pontos que mais me chamou a atenção ao criar meu blog foi a **facilidade do processo**. Desde a instalação do Hugo até a configuração inicial, tudo ocorreu de forma bastante intuitiva. A documentação do Hugo é clara e oferece guias detalhados, o que facilitou muito a compreensão de suas funcionalidades.

Além disso, o fato de poder utilizar **Markdown** para escrever minhas postagens trouxe um novo nível de praticidade.

### Criando um site Hugo 

Após instalar o Hugo, você pode criar um novo site usando o seguinte comando (sinta-se à vontade para substituir "my-hugo-site" por outro nome, se preferir):

```
hugo new site my-hugo-site
```

Depois de executar o comando, navegue até a pasta do site. Você verá os seguintes arquivos e pastas:

- **config.toml**: Arquivo de configuração do site.
- **archetypes/**: Modelos para novos conteúdos.
- **content/**: Pasta onde você armazena as postagens e páginas do seu site.
- **layouts/**: Contém templates que definem a aparência do seu site.
- **themes/**: Onde ficam os temas do Hugo.
- **data/**: Dados adicionais que podem ser usados nas postagens.
- **static/**: Arquivos estáticos (imagens, CSS, JavaScript) que serão copiados diretamente para o diretório de saída.

Essa estrutura básica permite que você organize seu conteúdo e personalizações de forma eficiente, facilitando a criação e manutenção do seu site.

### Adicionando um tema

Fazer o download e instalar um tema pré-fabricado é uma ótima maneira de começar com Hugo. Os temas vêm em vários formatos e tamanhos, muitos disponíveis gratuitamente no repositório oficial de temas do Hugo. 

> **Nota:** Eu utilizei o tema [**PaperMod**](https://github.com/adityatelange/hugo-PaperMod) para o meu blog. Confira meu repositório no GitHub para mais detalhes!

Para instalar um tema como o Hyde, siga os passos abaixo:

1. Navegue até a pasta `themes` do seu projeto no terminal:
   ```bash
   cd <hugo-project-directory>/themes/
   ```

2. Use o Git para clonar o tema Hyde no diretório `themes` do seu projeto:
   ```bash
   git clone https://github.com/spf13/hyde.git
   ```

3. Adicione a seguinte linha ao seu arquivo `config.toml` para ativar o tema:
   ```toml
   theme = "hyde"
   ```

Neste ponto, o tema está instalado e configurado. Para visualizar o site no seu navegador, inicie o servidor web de desenvolvimento integrado do Hugo:

### Pré-visualizar um site no Hugo

Hugo vem com um servidor web integrado, permitindo visualizar seu site localmente sem a necessidade de instalar um servidor externo como Nginx ou Apache. Para iniciar o servidor, execute o comando abaixo no diretório raiz do seu projeto:

```bash
hugo server -D
```

Hugo construirá as páginas do seu site e as disponibilizará em [http://localhost:1313/](http://localhost:1313/).

## Workflow do GitHub 

Uma parte interessante foi usar o **GitHub Workflow** para o deploy do meu blog. Essa abordagem trouxe novas experiências, especialmente porque normalmente utilizo a Vercel. 

## Conclusão

Foi muito massa essa descoberta, e estou animado para continuar personalizando meu blog e incorporando novas funcionalidades ao longo do tempo. 

Obrigado por visitar o meu blog! 
# OWLAB - One Welfare Lab

Site institucional da OWLAB, uma estrutura de inteligência pública que aproxima ciência, cidadania, instituições e animais para apoiar decisões públicas mais informadas.

## Estrutura

- `index.html` - página principal do site.
- `assets/logo.png` - logo em alta resolução usada no cabeçalho e no rodapé.
- `assets/favicon.svg` - favicon vetorial simplificado para melhor leitura no navegador.
- `style.css` - tokens visuais, acessibilidade e ajustes responsivos globais.

Os PDFs, DOCX e imagens de referência ficam apenas no ambiente local e são excluídos pelo `.gitignore`.

## Como executar localmente

O site não precisa de instalação de dependências ou processo de build.

### Opção 1: abrir diretamente

Abra `index.html` no navegador.

### Opção 2: usar um servidor local pelo CMD

No Prompt de Comando do Windows:

```cmd
cd /d "C:\SITE OWLAB"
py -m http.server 8000
```

Depois acesse [http://localhost:8000/index.html](http://localhost:8000/index.html).

Para parar o servidor, pressione `Ctrl+C` no CMD.

## Funcionalidades

- Conteúdo em português e inglês, alternado pelo botão `EN/PT`.
- Navegação por seções com âncoras.
- Botão flutuante `Voltar ao topo`, disponível ao navegar pelas seções principais.
- Animações de entrada ativadas conforme as seções aparecem na tela.
- Layout responsivo para desktop, tablet e telemóvel.
- Respeito à preferência do utilizador por redução de movimento.

## Publicar no GitHub

O repositório remoto é:

<https://github.com/hariane9/owlab-site>

Se esta pasta ainda não tiver Git inicializado, execute no CMD:

```cmd
cd /d "C:\SITE OWLAB"
git init
git branch -M main
git remote add origin https://github.com/hariane9/owlab-site.git
git add .
git commit -m "Adiciona estilos externos e documentação do site"
git push -u origin main
```

Se o repositório remoto já tiver um `origin`, atualize-o com:

```cmd
git remote set-url origin https://github.com/hariane9/owlab-site.git
```

Se o GitHub já tiver um README ou outro commit inicial, sincronize antes do primeiro envio:

```cmd
git pull origin main --allow-unrelated-histories
git add .
git commit -m "Mescla arquivos locais"
git push -u origin main
```

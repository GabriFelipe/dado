# Dado da Probabilidade

Simulador de dados com pesos ajustáveis por face, feito para uso em sala de aula na explicação de probabilidade (dados honestos, dados viciados, lei dos grandes números).

É um site estático de um único arquivo (`index.html`) — não precisa de servidor, banco de dados ou build. Basta hospedar o arquivo em qualquer serviço de arquivos estáticos.

## Arquivos

- `index.html` — o site completo (HTML, CSS e JavaScript em um único arquivo).

## Como colocar no ar

Escolha uma das opções abaixo.

### Opção 1: GitHub Pages (gratuito)

1. Crie um repositório novo no GitHub.
2. Faça upload do `index.html` para a raiz do repositório.
3. Vá em **Settings → Pages**.
4. Em "Source", selecione a branch `main` e a pasta `/root`.
5. Salve. Em alguns minutos o site estará disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

### Opção 2: Netlify (gratuito)

1. Acesse [app.netlify.com](https://app.netlify.com) e crie uma conta.
2. Arraste a pasta contendo o `index.html` para a área de "deploy manual" (Netlify Drop).
3. O site fica no ar imediatamente com uma URL gerada automaticamente.

### Opção 3: Vercel (gratuito)

1. Acesse [vercel.com](https://vercel.com) e crie uma conta.
2. Crie um novo projeto e faça upload da pasta com o `index.html`.
3. Publique — a URL fica disponível em segundos.

### Opção 4: Servidor próprio

Basta copiar o `index.html` para a pasta pública do seu servidor web (ex: `public_html`, `www`, ou a raiz configurada no Apache/Nginx). Não há dependências para instalar.

## Rodar localmente antes de publicar

Basta abrir o arquivo `index.html` diretamente no navegador (duplo clique) ou, se preferir servir localmente:

```bash
python3 -m http.server 8000
```

E acessar `http://localhost:8000` no navegador.

## Personalização

Todo o código está em um único arquivo, organizado em três blocos:

- `<style>` — cores, tipografia e layout (variáveis CSS no topo, em `:root`).
- HTML — estrutura da página (painel de controles, dado, tabela de estatísticas).
- `<script>` — lógica do simulador (pesos, sorteio, contagem de resultados).

Não há dependências externas além de fontes do Google Fonts, carregadas via `<link>` no `<head>`.

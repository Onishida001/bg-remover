# 🖼️ Removedor de Background

Remove o fundo de imagens diretamente no navegador, sem enviar nada para servidores externos.

**[▶ Abrir o app](https://SEU-USUARIO.github.io/bg-remover)**

---

## Como funciona

- Usa a biblioteca [`@imgly/background-removal`](https://github.com/imgly/background-removal-js) que roda via **WebAssembly** no navegador
- O modelo de IA é baixado uma única vez e fica em cache
- Nenhuma imagem sai do seu computador

## Como hospedar (passo a passo)

### 1. Criar o repositório no GitHub

1. Acesse [github.com](https://github.com) e clique em **New repository**
2. Nome: `bg-remover`
3. Marque **Public**
4. Clique em **Create repository**

### 2. Fazer upload do arquivo

1. Na página do repositório, clique em **Add file → Upload files**
2. Arraste o arquivo `index.html`
3. Clique em **Commit changes**

### 3. Ativar o GitHub Pages

1. Vá em **Settings → Pages**
2. Em **Source**, selecione **Deploy from a branch**
3. Branch: `main` | Pasta: `/ (root)`
4. Clique em **Save**
5. Aguarde ~1 minuto e acesse: `https://SEU-USUARIO.github.io/bg-remover`

---

## Uso no VS Code (desenvolvimento local)

Se quiser editar e testar localmente:

```bash
# Instale a extensão "Live Server" no VS Code
# Clique com botão direito no index.html → "Open with Live Server"
```

> O arquivo funciona sem nenhuma dependência local — tudo vem do CDN.

## Tecnologias

- HTML + CSS + JavaScript puro (sem framework)
- [@imgly/background-removal](https://github.com/imgly/background-removal-js) via CDN
- WebAssembly + ONNX Runtime Web

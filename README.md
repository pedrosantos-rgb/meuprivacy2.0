# Meu Privacy — Deploy Pronto

## Como fazer o deploy (sem build, sem npm)

Este ZIP já contém os arquivos compilados, prontos para servir.

### Passo 1 — Limpar o repositório

No repositório `pedrosantos-rgb/meuprivacy2.0`, apague todos os arquivos existentes na branch `main`.

### Passo 2 — Subir estes arquivos

Faça upload de todos os arquivos deste ZIP para a raiz do repositório:
- `index.html`
- `assets/` (pasta com o JS compilado)
- `.nojekyll` (arquivo oculto — importante incluir!)

```bash
git clone https://github.com/pedrosantos-rgb/meuprivacy2.0.git
cd meuprivacy2.0

# Copie os arquivos do ZIP aqui (index.html, assets/, .nojekyll)
git add -A
git commit -m "Deploy compiled app"
git push
```

### Passo 3 — Configurar GitHub Pages

1. Vá em **Settings** → **Pages**
2. Em **Source**, selecione **"Deploy from a branch"**
3. Branch: `main` | Folder: `/ (root)`
4. Clique **Save**

### Passo 4 — Aguardar

Após 1-2 minutos, acesse:
**https://pedrosantos-rgb.github.io/meuprivacy2.0/**

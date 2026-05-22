# Ficha de Bioespeleologia

App de campo (PWA) para preenchimento de fichas de bioespeleologia — **offline**, com **GPS**, **fotos** e **autosave**. Feito como arquivo único + service worker; sem backend.

🔗 **Versão publicada:** https://firewave999.github.io/Espeleologia-/

## Recursos
- Espelha a ficha de campo: Cabeçalho, Aporte energético, Fauna Silvestre, Características Ambientais, Atributos para Relevância e Registro Fotográfico.
- Toggles SIM/NÃO, campos de observação por item, chips de escolha e checklist fotográfico.
- **GPS** por ficha (precisão/altitude + link "abrir no mapa"); aceita entrada manual.
- **Fotos** pela câmera (comprimidas, guardadas em IndexedDB) com legenda.
- **Várias fichas** (cavernas) com troca, duplicação e exclusão.
- **Autosave** a cada toque (localStorage + IndexedDB).
- **Backup/Restauração** em `.json` (inclui as fotos) e **Imprimir / PDF**.

## Instalar no celular
1. Abra o link acima no Chrome (Android) ou Safari (iOS).
2. Menu do navegador → **Instalar app** / **Adicionar à tela inicial**.
3. Depois do primeiro acesso, funciona **sem internet**.

> ⚠️ Faça **backup `.json`** periodicamente (menu ⋯ no app). Os dados ficam no armazenamento do navegador daquele dispositivo/endereço.

## Publicar (GitHub Pages)
Settings → **Pages** → Source: branch `main`, pasta `/ (root)` → Save.
Aguarde ~1 min e acesse a URL acima.

## Estrutura
```
index.html       App completo (HTML/CSS/JS em arquivo único)
manifest.json    Manifesto PWA (instalação)
sw.js            Service worker (cache offline)
icon-192.png     Ícone
icon-512.png     Ícone
.nojekyll        Desativa processamento Jekyll no Pages
```

## Licença
Uso livre.

# JARVIS v0 (Android)

Projeto pessoal do Zeylor. Tela inicial com o botão ATIVAR JARVIS e o núcleo do JARVIS, com o módulo Gemini (conversa por texto/voz).

## Instalar no celular
1. Aba **Actions** do GitHub: espere o "Compilar APK" ficar verde (leva uns 5 minutos).
2. Aba **Releases** → **JARVIS v0 (build automatico)** → baixe `app-debug.apk`.
3. Abra o arquivo no celular e instale (permita "fontes desconhecidas" se pedir).

Todo envio (push) na `main` gera um APK novo na mesma release.

## Ver no navegador
A interface é a pasta `web/`. Para ver no computador: `cd web` e `python -m http.server 8000`, depois abra http://localhost:8000.

## Gemini
Toque em **GEMINI** (canto superior direito), cole a chave da API (pegue em https://aistudio.google.com/apikey), use **TESTAR CONEXÃO** para escolher o modelo e depois **SALVAR**. Aparece uma caixa de texto embaixo para conversar com o JARVIS (e um botão MIC no Chrome).

- A chave fica **só no aparelho** (armazenamento do navegador/app) e só é enviada ao Google. **Nunca coloque a chave no código nem no GitHub.**
- **APAGAR CHAVE** remove do aparelho.
- A personalidade do JARVIS (educado, sarcástico, respostas curtas, faz contas sozinho, avisa uma vez e obedece) está em `SYS` dentro de `web/index.html`.

## Estrutura
- `web/`: a interface (HTML/CSS/JS) e `vendor/` (Three.js, licença MIT)
- `app/`: casca Android (WebView em tela cheia)
- `.github/workflows/build.yml`: compila o APK sozinho

## Créditos
Código próprio. Visual inspirado nos filmes do Homem de Ferro (Cantina Creative/Jayse Hansen, Prologue, Perception); nenhum código ou arquivo desses estúdios foi usado. Three.js: MIT.

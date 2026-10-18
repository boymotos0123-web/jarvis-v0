# JARVIS v0 (Android)

Projeto pessoal do Zeylor. Tela inicial com o botão ATIVAR JARVIS e o núcleo do JARVIS, mais o painel do módulo Gemini (só visual nesta versão: o JARVIS ainda não responde nem fala).

## Instalar no celular
1. Aba **Actions** do GitHub: espere o "Compilar APK" ficar verde (leva uns 5 minutos).
2. Aba **Releases** → **JARVIS v0 (build automatico)** → baixe `app-debug.apk`.
3. Abra o arquivo no celular e instale (permita "fontes desconhecidas" se pedir).

Todo envio (push) na `main` gera um APK novo na mesma release.

## Ver no navegador
A interface é a pasta `web/`. Para ver no computador: `cd web` e `python -m http.server 8000`, depois abra http://localhost:8000.

## Gemini
O painel é só interface: não salva nem envia a chave. Quando ligarmos de verdade, a chave será digitada no app e ficará só no celular. **Nunca coloque a chave no código nem no GitHub.**

## Estrutura
- `web/`: a interface (HTML/CSS/JS) e `vendor/` (Three.js, licença MIT)
- `app/`: casca Android (WebView em tela cheia)
- `.github/workflows/build.yml`: compila o APK sozinho

## Créditos
Código próprio. Visual inspirado nos filmes do Homem de Ferro (Cantina Creative/Jayse Hansen, Prologue, Perception); nenhum código ou arquivo desses estúdios foi usado. Three.js: MIT.

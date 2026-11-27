# UFAB — UnlimitedFreeAIBerlipe

Fork visual + ajustes de interface do **GambiarraAPI**.

Tema rosa, branding **UFAB**, fundo com wallpaper personalizado e nome curto na interface.

> **Aviso:** Este projeto **não** é o GambiarraAPI original.  
> É uma customização de interface (UI) em cima do executável e arquivos da ferramenta original.  
> Todos os direitos do software base e de suas dependências pertencem aos respectivos autores.

---

## O que mudou

| Item | Antes | Depois |
|------|--------|--------|
| Nome na interface | GambiarraAPI | **UFAB** |
| Tema | Preto / cinza | Rosa escuro → rosa claro |
| Fundo | Gradiente genérico | Wallpaper personalizado |
| Ícone | Original | Personagem (sem fundo) |
| Textos "GambiarraAPI" | Presentes | Forçados para **UFAB** |

---

## Como aplicar o patch de interface

1. Feche o app completamente.
2. Vá até a pasta de instalação (a que contém `GambiarraAPI.exe` e a pasta `_internal`).
3. Entre em:
   ```
   _internal\absolut_ai\
   ```
4. Apague (ou renomeie como backup) as pastas:
   - `ui`
   - `assets`
5. Cole as pastas `ui` e `assets` do patch no lugar delas.
6. Abra o `GambiarraAPI.exe` normalmente.

Pronto. O visual novo carrega na hora.

---

## Estrutura do patch

```
ui/
  app.css          → tema rosa + fundo com wallpaper
  index.html       → título/logo UFAB + script de troca de nome
  splash.html      → splash com branding UFAB
  wallpaper.jpg    → fundo personalizado
  icons/           → ícone da interface
  fonts/           → fontes do app

assets/
  app.ico          → ícone multi-tamanho
  icon-256.png     → ícone 256px
```

---

## Observações

- O ícone **do .exe** (aquele do Explorador / barra de tarefas) fica gravado dentro do executável. Trocar só os arquivos em `assets` **não** altera o ícone do `.exe`. Para isso é necessário ferramenta de edição de recurso (ex.: Resource Hacker).
- Alguns textos profundos ainda podem vir do backend original. O patch força a troca de “GambiarraAPI” → “UFAB” na interface visível.
- Se aparecer erro de `Python.Runtime.dll`, o problema costuma ser pasta `_internal` incompleta ou caminho duplicado na extração — não é causado pelo patch de UI.

---

## Créditos

- **Base:** GambiarraAPI (ferramenta de terceiros)
- **Customização visual / branding UFAB:** Berlipe
- GitHub: [github.com/Berlipe](https://github.com/Berlipe)

---

## Licença / uso

Este fork de interface mantém o respeito à autoria do software original.  
Consulte os termos do GambiarraAPI antes de redistribuir o pacote completo.

Uso por conta e risco. Não oferecemos suporte oficial do app original.

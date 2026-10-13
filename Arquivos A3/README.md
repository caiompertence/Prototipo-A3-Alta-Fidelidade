# Termoterapia - protótipo de alta fidelidade

Abra `index.html` no Chrome ou no Edge (ou use a extensão Live Server do VS Code).
Sem servidor e sem bibliotecas. As fontes (Baloo 2 e Figtree) vêm do Google Fonts; sem internet o app usa fontes do sistema.

## Arquivos
- `index.html`: estrutura da página.
- `css/estilo.css`: cores e medidas (variáveis no `:root`) e estilos.
- `js/app.js`: tudo o resto, nesta ordem:
  1. Conteúdo: recursos (`R`), condições (`C`), objetivos (`O`), segurança (`SEG`), triagem (`Q`), orientações (`ORI`), informações (`INF`).
  2. Estado e navegação.
  3. Telas (objeto `V`, uma função por tela).
  4. Eventos (clique, change, input).

## Onde editar o conteúdo
- Fichas e textos científicos: `R`, `EX` e `SEG` em `js/app.js` (campos "a preencher" ficam nas telas `ficha` e `comp`).
- Perguntas e regra da triagem: `Q` e `decide`.
- Cores: `:root` em `css/estilo.css`.

## Dados salvos no navegador (localStorage)
`t_role`, `t_user` (nome, e-mail, CREFITO; a senha não é guardada), `t_reg`, `t_fav`, `t_lemb`, `t_notas`, `t_chat`, `t_ult`.
Em Perfil > Apagar dados, tudo é removido, exceto o login.

Protótipo: o login não valida conta em servidor, o chat é simulado e a lista de fisioterapeutas próximos é de exemplo.

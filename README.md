# Escala de rotatividade T1 · NOC PADTEC

Dashboard estático (um único arquivo HTML) com a escala de rotatividade de atividades da equipe T1.

## Arquivos

- `index.html`: o dashboard completo. Dados, estilos e scripts estão dentro dele.
- `vercel.json`: configurações opcionais de cabeçalhos (pede aos buscadores para não indexar a página e evita cache antigo).
- `.gitignore`: ignora arquivos temporários.

Não há build, `package.json` nem dependências para instalar. A única dependência externa é a biblioteca html2canvas, carregada do cdnjs, usada pelo botão "Copiar imagem da tabela".

## Publicar na Vercel

1. Suba esta pasta em um repositório no GitHub.
2. Na Vercel, clique em **Add New > Project** e importe o repositório.
3. Em **Framework Preset**, deixe **Other**. Não preencha Build Command nem Output Directory.
4. Clique em **Deploy**. A Vercel gera um endereço gratuito do tipo `nome-do-projeto.vercel.app`.

## Atualizar a escala todo mês

1. Gere o `index.html` atualizado (novos dias, meses ou ajustes).
2. Substitua o `index.html` do repositório pelo novo, direto no GitHub (**Add file > Upload files**) ou com `git commit` e `git push`.
3. A Vercel publica automaticamente a nova versão no mesmo endereço, normalmente em menos de um minuto.

## Observações

- A página contém nomes completos da equipe e informações de folgas, bancos de horas e férias. Quem tiver o link consegue ver, então compartilhe apenas com a equipe e confirme se a política da empresa permite hospedagem externa. Se o repositório for público no GitHub, o conteúdo também fica público. Prefira um repositório **privado**.
- O tema claro/escuro segue o aparelho na primeira visita e depois lembra a escolha feita pelo botão do cabeçalho.

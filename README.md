# Quem Sou Eu Online

Site de um arquivo só (`index.html`). As salas em tempo real usam o Supabase, que já está configurado no código com a URL e a chave pública do seu projeto `quem-sou-eu`.

## 1. Conferir o Realtime no Supabase

No painel do projeto, abra **Realtime > Settings** e confirme que **Allow public access** está ligado. Sem isso as salas não conectam. Não precisa criar tabela nem mexer no banco.

## 2. Subir no GitHub

1. Crie um repositório novo no GitHub (por exemplo, `quem-sou-eu`).
2. Envie os arquivos desta pasta (`index.html` e este `LEIA-ME.md`) para a raiz do repositório. Pode ser pelo botão **Add file > Upload files**.

## 3. Publicar na Vercel

1. Na Vercel, clique em **Add New > Project** e escolha o repositório.
2. Em **Framework Preset**, deixe **Other**. Não precisa de build nem de variáveis de ambiente.
3. Clique em **Deploy**. Você ganha um link como `quem-sou-eu.vercel.app`.

## 4. Testar

1. Abra o link em uma aba, digite um apelido e toque em **Criar sala**.
2. Abra o mesmo link em outra aba ou no celular e entre com o código de 4 letras (ou use **Copiar link** no lobby).
3. Com 2 jogadores, toque em **Começar o jogo**.

## Como jogar

- Quem é sorteado para adivinhar vê só "?". Os outros veem a palavra.
- Qualquer outra pessoa toca em **Acertou!** quando o jogador acerta. Cada acerto vale 1 ponto.
- No lobby, o anfitrião escolhe temas, tempo por vez (45 a 120 s) e quantas vezes cada um adivinha.
- **Meus temas e palavras** na tela inicial cria temas próprios. Eles ficam salvos no navegador de quem os criou e valem quando essa pessoa é a anfitriã.
- **Palavras da galera**: cada jogador sugere até 8 palavras no lobby, e o anfitrião inclui no jogo.
- **Jogar neste celular**: modo presencial, sem sala, passando o aparelho.

## Limites

- A aba do anfitrião precisa ficar aberta durante o jogo. Se ele sair ou recarregar a página, a sala acaba.
- O plano gratuito do Supabase permite 200 conexões simultâneas e 100 mensagens por segundo. Para um grupo de amigos sobra.
- A chave `sb_publishable_...` é pública e pode ficar no código. Nunca coloque a chave `secret` ou `service_role` aqui.

## Mudar a URL ou a chave

Estão no começo do script em `index.html`, nas linhas `SB_URL` e `SB_KEY`.

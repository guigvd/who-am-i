# Quem Sou Eu Online

Site de um arquivo só (`index.html`). As salas em tempo real usam o Supabase, que já está configurado no código com a URL e a chave pública do seu projeto `quem-sou-eu`.

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

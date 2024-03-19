---
description: >-
  Saiba como importar streams antigos da sua conta do Spotify e Apple Music na
  sua conta do Last.fm
---

# 🟡 Importar Streams no Last.fm

{% hint style="danger" %}
**Importar seus scrobbles fará com que os seus relatórios (diário, semanal e anual) fiquem imprecisos.** Algumas pessoas gostam de receber dados precisos sobre seus hábitos de escuta (por exemplo, a data exata em que cada música foi transmitida). Se você é uma dessas pessoas, não continue.
{% endhint %}

{% hint style="info" %}
Este guia foi criado por [comicxans](https://www.last.fm/user/comicxans) e traduzido e adaptado pela equipe do Last.fm Brasil. [Visite o guia original](https://docs.google.com/document/d/1IhFMol3wZs24uKnh2rbxHpLaxhETcfB8KqzYIkEW\_iM).
{% endhint %}

***

## Solicitando seus dados

### Spotify

1. Envie um email para o [privacy@spotify.com](mailto:privacy@spotify.com) entitulado **Requesting a Copy of My Extended Streaming History**. Tenha certeza de que está enviando este email pelo mesmo email que você utiliza no Spotify.
2. Copie e cole o modelo abaixo no corpo do email e substitua tudo o que está nos colchetes com informações corretas:\
   \
   _Hello! I would like to download a copy of my extended streaming history. For verification purposes, I’m using a **\[marca, modelo e versão do sistema operacional de qualquer dispositivo que você usa com o Spotify]** and a song I’ve recently saved to my library is **\[nome da musica e de quem é]**. Thanks!_\

3. Responda todos os emails que você receber em reposta ao seu email. Você será solicitado a confirmar sua solicitação antes de começarem a preparar seus dados. Este processo não deve demorar mais do que 30 dias!\


Este é o email que você **não deverá receber** se você seguir as instruções corretamente:

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

Este é o email correto que você deverá encontrar na sua caixa de entrada assim que seus dados forem finalizados:

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### Apple Music

{% hint style="info" %}
**D**iferente do Spotify, **o Apple Music não fornece dados dos álbuns**, o que não é necessário, mas suas faixas não estarão conectadas aos álbuns. Isso significa que você não terá resultado de quantas vezes você ouviu determinado álbum, por exemplo. Há uma opção para assinantes do [Last.fm Pro](https://www.last.fm/pt/pro) que permite você editar as faixas e adicioná-las em álbuns.
{% endhint %}

1. Com o seu [ID da Apple](https://support.apple.com/pt-br/HT201354), vá até [privacy.apple.com](https://privacy.apple.com/) e solicite uma cópia dos seus dados.

<div align="center" data-full-width="true">

<figure><img src="https://lh7-us.googleusercontent.com/Ilq6HYfiaI_H3zVhg1WFg-B9K3ktmS7W7G5QUJkKi1fkmFVIG2fGzrYGbam3n5aEMHw92VzBwMGNoNyHfLMBxmbv3MI8QqaV-lgI90-BBgHZrTe09zE9pyuwT4Zi3mLW5EPcbpniHsaOWtghR-acQZex_ZVePII" alt="" width="375"><figcaption></figcaption></figure>

</div>

2. Na página seguinte, marque a opção "**Apple Media Services information**", depois continue.
3. Selecione o tamanho máximo do arquivo que for mais conveniente para você, ou apenas deixe em 1 GB. Novamente, prossiga e pronto. Não deverá demorar mais que uma semana para a Apple compilar todos os seus dados.&#x20;
4. Ocasionalmente, você pode verificar [privacy.apple.com](https://privacy.apple.com) para atualizações sobre seu status.

***

## Preparando seus dados

### Spotify

{% hint style="warning" %}
Não prossiga se seus arquivos JSON estiverem nomeados como "**StreamingHistory**", já que eles não irão funcionar com este método. Em vez disso, refaça a [solicitação dos seus dados](importar-streams.md#spotify).
{% endhint %}

1. Assim que você baixar os arquivos numa pasta ZIP, intitulada "**my\_spotify\_data**", extraia e procure os arquivos **endsong\_.json**. O numeração dos arquivos refletem a quantidade de música que você escutou.

<figure><img src="https://lh7-us.googleusercontent.com/rM6ZmK-0HOdhh5f8qiRVwyg5tAvf6BMK_RiJHJLB943Qgp44MhBmX-aZ5iwHXzbk1Eg6mr2yHLkTUv-mvHXHdrRUT6PfUibzSNF-sJ3tZ7RXedrC0DEn0piIF3khbDjhfNGN03z6P_hCWPbF0EJuvhtrQuSHbvE" alt="" width="188"><figcaption></figcaption></figure>

2. Abra o site [lilnasy.github.io/scribblyscrobbly](https://lilnasy.github.io/scribblyscrobbly/) e clique no emoji apontando para cima (☝).
3. Selecione e envie todos os arquivos "**endsong\_.json**" de uma vez.

<figure><img src="https://lh7-us.googleusercontent.com/yU_BRHk_jgrItnh5hMZE-v-uqHfHMF82fiE3Y78FsefyBQww7POjuVkpa7yQ4hA3TilUA8CpRxja2Xu8dBQ56FC1yoQHS4kOKZR6KRjvkRsmRT9mS6nFMHAhrhXglpfzS15EitjsAjDT19S-UqQjVW9tiBLfX-8" alt="" width="375"><figcaption></figcaption></figure>

4. Você saberá quandos os arquivos estarão prontos assim que o emoji estiver apontando para baixo (👇), então basta clicar nele para baixar um pasta ZIP.

{% hint style="info" %}
Os passos a seguir são essenciais para você não acabar duplicando acidentalmente seus scrobbles. Se você não tiver nenhum scrobble no Last.fm, você pode prosseguir para
{% endhint %}

5. Entre no seu [perfil do Last.fm](https://www.last.fm/pt/user/\_) e vá até [scrobbles](https://www.last.fm/pt/user/\_/library/artists).
6. Vá até a última página e identifique a primeira música que você scrobblou.

<figure><img src=".gitbook/assets/chrome_S3keVzqAKE.png" alt="" width="375"><figcaption></figcaption></figure>

7. Entre no site [jsoneditoronline.org](https://jsoneditoronline.org) para remover as músicas do arquivo que você não precisa para scrobblar novamente.
8. Na aba menu, clique em "**Open from disk**"

<figure><img src=".gitbook/assets/chrome_4WR0JRZe6x.png" alt="" width="251"><figcaption></figcaption></figure>

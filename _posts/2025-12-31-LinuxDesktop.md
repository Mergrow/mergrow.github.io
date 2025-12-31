---
title: Estou finalmente migrando meu desktop para Linux.
date: 2025-12-31 06:54:00 +/-0200 # -200 brazil timezone.
categories: [Linux]
tags: [ptbr, linux, desktop, cachyos]
---
Esse é o meu primeiro post aqui e vou comentar sobre meu descontentamento com o Windows e tudo o que me levou a abandoná-lo de vez e migrar para o Linux.

## Fim do suporte do Windows 10

A data é **30/12/2025**, dia anterior à véspera de Ano Novo.

Como de costume, ligo meu computador no início da manhã, ainda rodando o famigerado Windows 10, que por muito tempo foi uma experiência excelente, apesar de seu início conturbado. Porém, para minha surpresa, sou agraciado com uma tela me pedindo para atualizar o sistema para o *Windows 11*, avisando que o suporte para a versão atual havia se encerrado há alguns meses.

## A dúvida é: devo atualizar?

Eu paro e penso:

> "_Já utilizei o Windows 11 anteriormente, mas então por que estou usando o Windows 10?_"

Começo a refletir sobre todos os pontos que me fizeram voltar para o Windows 10 e percebo que atualizar para o Windows 11 **não** é uma opção.

## A lista é enorme

> Ok, beleza. Que experiência horrível justificaria abandonar um ambiente desktop que você usa há mais de uma década para se aventurar nas águas do Linux Desktop?

Há quase exatamente um ano, em **6 de dezembro de 2024**, [Path of Exile 2](https://pathofexile2.com) lançava seu primeiro beta test aberto — uma novidade extremamente aguardada pelos amantes de ARPG. A diversão estava garantida para o fim daquele ano e para o início de 2025. Bom, estaria… se em outubro do mesmo ano não tivéssemos recebido a porcaria da atualização do Windows 11 ```24H2```.

Essa atualização, para os usuários comuns, já foi péssima por deixar o sistema [extremamente lento e bugado](https://www.reddit.com/r/Windows11/comments/1h5s85z/whats_going_on_with_windows_11_24h2). Porém, para quem estava tentando jogar PoE2, foi um completo **desastre**.

Em resumo: a ```24H2``` trouxe um [bug](https://www.reddit.com/r/PathOfExile2/comments/1hffj5b/poe_2_performance_issues_on_windows_11_24h2) no PoE2 (possivelmente também no PoE1) que fazia com que, ao alterar de zona no jogo, o computador congelasse completamente, sendo necessário reiniciar todo o sistema. Ao contrário do que pode parecer, não era um bug esporádico. Acontecia quase toda vez que você trocava de mapa — e você trocava de mapa com **bastante** frequência.

### Pra ferrar de vez:

A Microsoft dava a opção de restaurar para a atualização anterior apenas algumas semanas após a atualização. Como já estávamos em dezembro e a atualização saiu em outubro, eu não tinha mais um ponto de restauração disponível.

Para ajudar, a ISO disponível no site da Microsoft já vinha com a ```24H2```, então eu só tinha duas opções:
- baixar uma ISO editada de algum site **sus**;
- ou baixar a ISO do Windows 10, que ainda era disponibilizada pela Microsoft.

Na época, acabei optando pela segunda opção, o que me levou a usar o Windows 10 até o fim do seu suporte.

> _Bom, já faz bastante tempo desde que isso aconteceu. Já saíram diversas atualizações do Windows nesse meio-tempo e esse problema do PoE provavelmente já foi solucionado, correto?_

Provavelmente. Porém, na época em que baixei o Windows 11, já tive dor de cabeça, pois a Microsoft forçava a todo custo o uso de uma conta online. Apesar de ainda ser possível burlar facilmente essa restrição, a tendência é que a Microsoft cada vez mais [restrinja o uso de contas offline](https://www.reddit.com/r/pcmasterrace/comments/1o00spu/microsoft_is_plugging_more_holes_that_let_you_use/).

O Windows 11 já vem, há algum tempo, se tornando cada vez mais um verdadeiro [Adware](https://www.engadget.com/windows-11-now-comes-with-its-own-adware-124531977.html), além da *trend* de transformar tudo em um agente de IA. Esses pontos me afastaram completamente de sequer tentar o Windows 11 **mais uma vez**.

## 2026: O ano do Linux Desktop?

Tá, beleza. E agora?

Voltando à data do início da postagem: ao me deparar com a mensagem pedindo para atualizar para o Windows 11, eu entrei em choque. No mesmo instante, escolhi uma *distro*, baixei o Rufus e decidi que finalmente abandonaria o Windows de vez.

Inicialmente, escolhi o Fedora. Criei o pendrive bootável e segui para a instalação. A versão era o ```Fedora 43 com KDE Plasma```. A instalação foi bem rápida, o sistema *out-of-the-box* era lindo, o navegador pré-instalado era o Firefox (que eu já utilizava) — tudo parecia perfeito.

Até que abri a Twitch para contar a um amigo meu, que estava fazendo live e já utilizava Linux para jogar, que eu havia formatado o PC e estava finalmente no Linux… quando me deparei com a seguinte mensagem:


  
 ```Este vídeo está indisponível ou não é compatível com este navegador. (Erro #4000)```
 
 
Não consigo assistir à Twitch. Mas por quê?

Pesquiso o erro no Google e encontro diversos resultados em fóruns pela internet. O problema parecia ser que o Fedora não vinha com alguns codecs proprietários pré-instalados, necessários para que a Twitch (e possivelmente outras mídias) funcionassem.

Bom, era só instalar os codecs e *gg*. Não deveria ser complicado, certo?

Começo a copiar diversos comandos no terminal, reinicio o Firefox e… nada. O erro permanece. Copio mais e mais comandos, sem saber exatamente o que cada um faz, apenas na esperança de conseguir abrir a Twitch — mas nada funciona.

Então penso:

> _Talvez eu precise reiniciar o sistema. No Windows era assim, hehe._

Reinicio o computador e, para minha surpresa, não tenho mais vídeo.

Cinco minutos. Apenas **cinco minutos** foram suficientes para eu quebrar meu sistema pela primeira vez. Provavelmente isso ocorreu por burrice minha, mas naquele momento eu simplesmente desisti e escolhi uma distro mais simples, que já tivesse praticamente tudo *out-of-the-box*.

Por recomendação desse mesmo amigo, escolhi o [CachyOS](https://cachyos.org).

E aqui estou eu.

![CachyOS fastfetch](/assets/img/cachy-fastfetch.png)
_Fastfetch do meu sistema_

Até o presente momento, tudo está funcionando perfeitamente. Passei as primeiras horas corrigindo alguns problemas relacionados ao setup de dois monitores, pois o KDE Plasma tinha certa dificuldade em entender qual monitor era o primário e qual era o secundário, fazendo com que os apps e o SDDM abrissem no monitor errado.

Tirando isso, tudo funcionou *out-of-the-box*. Todos os jogos estão funcionando perfeitamente, e alguns até rodando melhor do que no Windows. Tenho ciência de que diversos programas e jogos eventualmente não vão funcionar no Linux, seja por conta de anticheat em nível de kernel ou outros problemas, mas, por enquanto, estou bem satisfeito com a experiência.

### Alguns programas alternativos que estou utilizando

Para monitorar a bateria do meu mouse **G Pro Superlight**, ajustar DPI e outras funcionalidades — já que o Linux não possui o Logitech G Hub — estou usando o [Solaar](https://github.com/pwr-Solaar/Solaar).

Eu também utilizava o G Hub para equalizar meu microfone **Blue Yeti Classic**, mas acabei não procurando uma alternativa, pois julguei não ser necessário no momento. Para controle de loopback, usei o **alsamixer**, já que utilizo o próprio microfone como interface de áudio através da entrada de retorno. Ele já vem pré-instalado no sistema.

Bom, é isso.

Talvez eu vá atualizando este post conforme vá descobrindo coisas novas ou encontrando novos problemas durante o uso do CachyOS. No final de janeiro, quero escrever um novo post com minhas considerações após um mês de uso. Aí veremos se continuo no CachyOS, se mudo de distro ou, quem sabe, se volto para o Windows hehe.

E para você que está lendo: te desejo um feliz Ano Novo e que 2026 seja um ano excelente para todos nós.

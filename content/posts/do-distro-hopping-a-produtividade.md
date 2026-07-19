---
title: "Do Distro Hopping à Produtividade: Meu Workflow Híbrido entre Linux e Windows"
date: 2026-04-10
draft: false
summary: "Como parei de me importar com marcas de distribuições e estruturei um ambiente estável focado em fazer o trabalho."
tags: ["linux", "windows", "produtividade", "workflow"]
---

Passei anos fazendo *distro hopping*. É uma fase comum: você pula de distribuição em distribuição procurando aquela que vai resolver todos os seus problemas. Não resolve. Com o tempo, percebi que a mágica não está no núcleo do sistema operacional. Está em como você gerencia suas ferramentas e interage com o ambiente.

Hoje, meu setup é híbrido. Uso Fedora com KDE Plasma no laptop e Windows com WSL2 (Ubuntu) no desktop. Parei de me importar com marcas de distribuições e foquei no que realmente importa: fazer o trabalho.

---

## O Dilema do Desktop: Pragmatismo vs. Idealismo

O Linux é meu ambiente favorito, mas o pragmatismo vence o idealismo quando há prazos a cumprir. Eu mantenho o Windows no desktop por um motivo simples: Adobe Premiere, Illustrator e After Effects.

Mudar essas ferramentas me custaria velocidade de entrega. Não vale a pena aprender softwares novos do zero apenas por ideologia. Uso o WSL2 no Windows e tenho o terminal do Linux rodando de forma quase nativa. É o melhor dos dois mundos para o meu contexto.

## A Desmistificação das Distribuições

A principal diferença técnica entre as distribuições é o gerenciador de pacotes. Só isso. Quando entendi isso, tornei meu sistema agnóstico dividindo minhas instalações em duas frentes claras:

### Apps gráficos são Flatpaks
Para softwares com interface visual, uso Flatpak. Ele isola as dependências e me desvincula da base do sistema. Posso rodar uma distribuição estável ou LTS e ainda assim ter a versão mais recente do navegador, do Obsidian, do Bruno ou do Beekeeper Studio. Sem quebrar o sistema.

### Terminal é Nativo
Só instalo via gerenciador de pacotes nativo o que precisa estar direto no meu `$PATH` ou ser acessado via linha de comando. É o caso do VS Code (para o comando `code .` funcionar), do Docker e do `asdf` para gerenciar versões de linguagens.

## Dotfiles e Resiliência

Essa separação tornou meu ambiente portátil. Meu workflow é baseado em dotfiles (`.zshrc`, `.gitconfig`). 

Mantenho essas configurações em um Gist no GitHub. Se minha máquina quebrar ou eu precisar formatar o sistema, o processo de recuperação leva minutos. A agilidade real não está em não ter problemas, mas em saber o quão rápido você consegue voltar a produzir após um desastre.

## O Ambiente Gráfico Importa

Se a distribuição importa pouco, o ambiente gráfico (DE) muda tudo. Eu tentei vários:

1. **GNOME:** É minimalista, mas me irrita ter que instalar extensões para coisas básicas, como ícones na bandeja.
2. **i3wm:** Excelente para customização, mas consome muito tempo de configuração manual. Tempo que prefiro gastar codando.
3. **KDE Plasma:** Onde encontrei o equilíbrio. Funciona bem direto da instalação, sem atrito.

Para organizar minhas tarefas, configuro a área de trabalho em um grid de 2x2 workspaces. É uma divisão espacial simples que me ajuda a separar contextos sem esforço mental.

---

## Conclusão

Alcancei a maturidade no Linux quando parei de olhar para o nome da distribuição e passei a focar na reprodutibilidade do meu ambiente. O sistema operacional não deve ser um hobby de configuração infinita; deve ser uma plataforma estável que funciona exatamente do mesmo jeito, não importa a máquina onde eu esteja.
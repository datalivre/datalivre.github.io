---
layout: post
title: Knime na Análise de Sentimento Músical
image: /img/KNIME-logo.png
tags: [knime, analytics, rock n roll, análise de sentimento]
subtitle: Análise sentimental das melhores bandas de Hevy Metal de todos os tempos
---
Este artigo trata da utilização da ferramenta de análise e mineração de dados **Knime Analytics** para capturar todas as letras de músicas das 10 maiores bandas de Heavy Metal de todos os tempos a partir de um famoso portal de letras para, enfim, analisar o sentimento de cada banda.  

| Nesta página |
| :------      |
| Visão geral  | 
| Knime        |
| Pré requisitos | 
| Obtendo links para letras musicais |

## Visão geral  
O site de notícias MetalSucks, famoso por suas entrevistas, blogs de usuários e informações sobre lançamentos, já listou os melhores álbuns de metal do século, os melhores guitarristas e bateristas de metal moderno e até mesmo as barbas mais “Metal” da música pesada, mas desta vez eles decidiram ir além, em novembro de 2014, consultaram mais de uma centena de músicos, críticos, artistas, publicitários, jornalistas e membros reverenciados da industrial fonográfica para descobrir quais as 25 bandas de Heavy Metal que melhor representam o Heavy Metal na história. Como resultado temos que a banda trevosa Black Sabbath em primeiro lugar seguida de Iron Mainden. Em décimo terceiro lugar temos a banda belo-horizontina Sepultura enchendo de orgulho o povo Brasileiro e principalmente de Minas. A lista completa você pode acessar [neste link](http://www.metalsucks.net/2014/11/14/25-best-metal-bands-time-real-1-black-sabbath/).  

Contudo, vamos gerar uma análise sentimental apenas para as dez melhores bandas de Heavy Metal da história, nisso, será necessário fazer download das letras de todas as músicas de cada uma banda e como resultado final produziremos uma nuvem de palavras para cada um.  

**A seguir, as 10 melhores bandas de Heavy Metal da história:**  

![imagem black sabbath](/img/blacksabbath.jpg)
01. Black Sabbath 
02. Iron Maiden
03. Slayer
04. Metallica
05. Pantera 
06. Judas Priest 
07. Megadeth 
08. Death
09. Motorhead 
10. Carcass 

## Knime  
![knime analytics workflow](https://www.knime.org/files/images/products/AnalyticsPlatform/end-to-end_analytics_workflow.png)  

Para se chegar ao resultado esperado, vamos utilizar o software de mineração Knime que é a principal solução aberta projetada para descobrir o potencial oculto de dados gerando novas ideias e prevendo o futuro. O Knime foi construído há mais de uma década para acessar dados rapidamente de forma intuitiva a fim de ajudar sua próspera comunidade de cientistas de dados espalhados em mais de 60 países e organizações a impulsionar a inovação. 

## Pré requisitos
Os exemplos nesta seção utilizam o software Knime Analytics que pode ser baixado a partir [deste link](https://www.knime.org/downloads/overview).

## Obtendo links para letras musicais    
![obtendo links](/img/1_OBTENDOLINKS.png)

A começar, vamos inserir o node **Table Creator** que nos permite a criação manual de uma tabela de dados. No campo **Filter contents** do painel **Node Repository** digite Table Creator, o nó deve surgir logo após a evocação, arraste-o para o editor de fluxo de trabalho. Agora, dê um clique duplo no node para abrir sua janela de dialogo, copie e cole todos os links a seguir na primeira coluna:

https://www.letras.mus.br/black-sabbath/  
https://www.letras.mus.br/iron-maiden/  
https://www.letras.mus.br/slayer/  
https://www.letras.mus.br/metallica/  
https://www.letras.mus.br/pantera/  
https://www.letras.mus.br/judas-priest/  
https://www.letras.mus.br/megadeth/  
https://www.letras.mus.br/death/  
https://www.letras.mus.br/motorhead/  
https://www.letras.mus.br/carcass/  

O resultado deve ser igual ao da imagem que segue. Para executar o Table Creator, segure a tecla CTRL e clique no botão OK.
![janela de diálogo](/img/2-dialogo.png)



# Referências:  
* http://www.metalsucks.net/2014/11/14/25-best-metal-bands-time-real-1-black-sabbath/  
* https://pt.wikipedia.org/wiki/Nuvem_de_tags  
* https://www.knime.org/  

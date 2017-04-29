---
layout: post
title: Knime na Análise de Sentimento Músical
image: /img/KNIME-logo.png
tags: [knime, analytics, rock n roll,]
subtitle: Análise sentimental das melhores bandas de Hevy Metal de todos os tempos
---
Este artigo trata da utilização da ferramenta Knime Analytics para capturar todas as letras de músicas de 10 bandas de Heavy Metal a partir de um famoso portal de letras para, enfim, analisar o sentimento de cada banda.    
| Nesta página |
| :------ |
| Visão geral    | 
| Pré requisitos     | 

## Visão geral  
O site de notícias MetalSucks, famoso por suas entrevistas, blogs de usuários e informações sobre lançamentos, já listou os melhores álbuns de metal do século, os melhores guitarristas e bateristas de metal moderno e até mesmo as barbas mais “Metal” da música pesada, mas desta vez eles decidiram ir além, em novembro de 2014, consultaram mais de uma centena de músicos, críticos, artistas, publicitários, jornalistas e membros reverenciados da industrial fonográfica para descobrir quais as 25 bandas de Heavy Metal que melhor representam o Heavy Metal na história. Como resultado temos que a banda trevosa Black Sabbath em primeiro lugar seguida de Iron Mainden. Em décimo terceiro lugar temos a banda belo-horizontina Sepultura enchendo de orgulho o povo Brasileiro e principalmente de Minas. A lista completa você pode acessar [neste link](http://www.metalsucks.net/2014/11/14/25-best-metal-bands-time-real-1-black-sabbath/).  
Contudo, vamos gerar uma análise sentimental apenas para as dez melhores bandas de Heavy Metal da história, nisso, será necessário fazer download das letras de todas as músicas de cada uma banda e como resultado final produziremos uma nuvem de palavras para cada um.  

**A seguir, as 10 melhores bandas de Heavy Metal da história:**
- Black Sabbath 
- Iron Maiden
- Slayer
- Metallica
- Pantera 
- Judas Priest 
- Megadeth 
- Death
- Motorhead 
- Carcass 

Para se chegar ao resultado esperado, vamos utilizar o software de mineração Knime que é a principal solução aberta projetada para descobrir o potencial oculto de dados gerando novas ideias e prevendo o futuro. O Knime foi construído há mais de uma década para acessar dados rapidamente de forma intuitiva a fim de ajudar sua próspera comunidade de cientistas de dados espalhados em mais de 60 países e organizações a impulsionar a inovação. 

## Pré requisitos
Os exemplos nesta seção utilizam o software Knime Analytics que pode ser baixado a partir [deste link](https://www.knime.org/downloads/overview).

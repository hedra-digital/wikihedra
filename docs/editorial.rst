===================================
Checklists (planejamento e produção)
===================================


Estes ``checklists`` devem ser usados na aba de  _issues_ de cada livro, diretamente no github `hedra-editora`_.

.. _hedra-editora: https://github.com/hedra-editora 

Produção
--------

Abertura de projeto
===================

* Criar board no Odoo 
* Definir data de fechamento e data de expiração (fim da pré-venda)
* Cadastros de autor no Odoo
* Arquivos iniciais em \PRODUCAO\ORIGINAIS



Diagramação 
===========

* Definir formato
* Criar repositótio no github: autor_título
* Arquivos principais: Livro.tex; INPUTS.tex; ORIGINAIS.tex; PRETAS.tex; Makefile; fichatecnica.sty; fronthedra.sty; gitrevisioinfo.sty; .gitignore
* Rodar Makefile
* Padronizações: Partes, Capítulos e sections; versaletes; palavras hifenizadas; travessão, meio-traço e traço; indentação; footnotes; quotes; links; bibliografia
* Ajustes finos: geral



Revisão
=======

* Viúvas e orfãs



Capa
====


* Recalcular Lombada
* Conferir Formato (altura, largura e tamanho da orelha)
* Conferir Coleção
* Título: ler pausadamente título da capa e do miolo
* Autor: item
* Trecho de capa: conferir com Miolo
* Texto de orelha: leitura de duas pessoas
* Imagem de capa (não esquecer de colocar crédito de imaem depois dentro do livro)
* Nome do capista nos créditos
* Isbn (Mandar imagem EPS): conferir com planilha no google drive em goo.gl/QYVTex

Se for bolso:

* Rubricas de capa devem ter gênero: "Autor" "Autora"
* Seguir modelo _Organização e tradução do grego_
* Verificar se obra não faz parte de subcoleção
* Verifcar no miolo se constam resumos do autor, da obra e das pessoas envolvidas. Se houver subcoleção, verificar se existe também texto sobre.



Página de crédito (fichatecnica.sty)
====================================

.. raw:: latex

	\newcommand{\<COMANDO>}{<CONTEÚDO>} %em fichatecnica.sty (na pasta do livros)


Lista de comandos:

* \titulo  				
* \subtit  				
* \autor  				
* \ISBN
* \eISBN
* \ano
* \organizador  				
* \introdutor			
* \tradutor  				
* \prefacio  				
* \apresentador  				
* \edicao{Jorge Sallum}
* \coedicao
* \assistencia
* \revisao
* \preparacao
* \capa
* \imagemcapa  				
* \agradecimentos
* \indicacao
* \copyrightlivro
* \copyrighttraducao
* \copyrightorganizacao
* \copyrightilustracao
* \copyrightintroducao
* \titulooriginal
* \edicaoconsultada
* \primeiraedicao
* \grafica  				
* \papelmiolo  				
* \gramaturamiolo  				



Fechamento
==========

* verificar se código ID no final do livro bate com a versão do github
* arquivo de miolo está em \ARQUIVOSGERAIS?
* arquivo de capa está em \ARQUIVOSGERAIS?
* arquivo de EPUB em \ARQUIVOSGERAIS\EPUB
* arquivos estão em github?
* checklist de página de crédito
* Criar MO de lançamento 



Cadastros
=========

* Internos
	* Odoo (@jorgesallum)
	* Site 
* Indexadores (metadados)
	* Mercado editorial
	* Metabooks @(jorgesallum)
* Integradores (distribuição, PoD, logística, pagamentos)
	* Meta (@jorgesallum)
	* Bookwire 
* Repositórios ("netflix")
	* Nuvem de livros (@jorgesallum)
	* Árvore de livros 	

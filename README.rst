Template for the Read the Docs tutorial
=======================================

This GitHub template includes fictional Python library
with some basic Sphinx docs.

Read the tutorial here:

https://docs.readthedocs.io/en/stable/tutorial/

As coisas estão ficando confusas
--------------------------------

1. Github suporta markdown e restructuredtext: https://gist.github.com/javiertejero/4585196

2. Sphinx usa restructuredtext (será que não daria para usar markdown?: até dá, mas alguns features de rst não teriam suporte: https://blog.readthedocs.com/adding-markdown-support/ )  

... então, aprender outra linguagem de marcação (https://docutils.sourceforge.io/docs/user/rst/quickref.html)... e as fórmulas (latex) e os diagramas (mermaid)?

- https://github.com/mgaitan/sphinxcontrib-mermaid
- formulas têm suporte nativo: https://stackoverflow.com/questions/3610551/math-in-restructuredtext-with-latex


3. Eu queria usar autodoc na documentação do lumache. Achei estranho que não estivesse configurado, ainda mais porque `lumache.py` continha docstrings. Achei umas receitas que achei "complicadas" (meu instinto dizia que não era o jeito "certo"):

- https://stackoverflow.com/questions/65487163/python-sphinx-autodoc-not-rendering-on-readthedocs
- https://github.com/sphinx-doc/sphinx/issues/10057
- https://bioengineering-toolbox.readthedocs.io/en/latest/documentation/readthedocs.html
- https://readthedocs-lst.readthedocs.io/en/latest/faq.html
- https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html

Pior, em algum momento o jeito complicado era o jeito certo, mas mudou. Depois de umas horas de busca, vi que a solução estava no tutorial que eu estava seguindo desde o início, mas não estava escrito que resolvia. 

- https://docs.readthedocs.io/en/stable/tutorial/index.html#customizing-the-build-process
- https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html

Nisso aprendi que readthedocs indica que a documentação pode ser atualizada com um "implantando", mas não quer dizer que foi compilado e que a documentação está sendo implantada, mas que alguém modificou o código no github e a versão que está no readthedocs está atrasada em relação à versão do github. Tem que compilar na mão ou gerar um webhook.

A documentação gerada a partir deste repositório (este arquivo não está incluído) está em https://rtd-lumache-test-fnakano.readthedocs.io/en/latest/index.html




Modelo de projeto Python perfeito
=================================

Este modelo de projeto cria a estrutura básica para um projeto Python. O artigo `Como configurar um projeto Python perfeito <https://blog.pronus.io/en/posts/python/how-to-set-up-a-perfect-python-project/>`_ descreve todas as decisões de design usadas aqui.


Características
---------------

* Python 3.10+ (configurável)
* Gerenciamento de dependência baseado em poesia
* Tarefas de desenvolvimento registradas em um ``Makefile`` para fácil acesso e gerenciamento
* Ganchos Mercurial/Git personalizados para eventos ``pre-commit`` e ``pre-push``
* Linting baseado em ruff_, blue_, mypy_ e outros
* Testes baseados em pytest_


Instruções
==========

Para instanciar o modelo em um novo projeto, você precisará do cookiecutter_.
A melhor maneira de usá-lo apenas uma vez é através do pipx_:

.. code:: console

    $ pipx run cookiecutter gh:andredias/perfect_python_project

Se preferir, use pode instalá-lo através do `pip`:

.. code:: console

    $ pip install --user cookiecutter

Em seguida, execute o seguinte comando:

.. code:: console

    $ cookiecutter gh:andredias/perfect_python_project

Responda algumas perguntas:

.. code:: text

    author []: Fulano de Tal
    email []: fulano@email.com
    project_name [Project]: Project X
    project_slug [project_x]:
    python_version [3.10]:
    line_length [79]: 100
    Select version_control:
    1 - hg
    2 - git
    Choose from 1, 2 [1]: 1
    github_respository_url []:


É isso!


.. _blue: https://pypi.org/project/blue/
.. _cookiecutter: https://github.com/cookiecutter/cookiecutter
.. _mypy: http://mypy-lang.org/
.. _pipx: https://pypa.github.io/pipx/
.. _Poetry: https://python-poetry.org/
.. _pytest: https://pytest.org
.. _ruff: https://pypi.org/project/ruff/

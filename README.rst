Usage
=====

This action will build and commit Sphinx documentation to ``gh-pages``
branch.

Inputs
======

======================= ============== ============ =============================
Input                   Default        Required     Description
----------------------- -------------- ------------ -----------------------------
``documentation_path``  ``'./docs'``   ``false``    Relative path under
                                                    repository to documentation
                                                    source files
``target_branch``       ``'gh-pages'`` ``false``    Git branch where assets will
                                                    be deployed
``target_path``          ``'.'``        ``false``   Directory in Github Pages
                                                    where Sphinx Pages will be
                                                    placed
``repository_path``     ``'.'``        ``false``    Relative path under
                                                    ``$GITHUB_WORKSPACE`` to
                                                    place the repository.
                                                    You not need to set this
                                                    Input unless you checkout
                                                    the repository to a custom
                                                    path
``requirements_path``   ``''``         ``false``    Relative path under
                                                    ``$repository_path`` to pip
                                                    requirements file
``sphinx_version``      ``''``         ``false``    Custom version of Sphinx
``sphinx_options``      ``''``         ``false``    Additional Sphinx options
======================= ============== ============ =============================

Tips
====

Copy extra files to site
========================

Use Sphinx confval html_extra_path__.

__ https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_extra_path

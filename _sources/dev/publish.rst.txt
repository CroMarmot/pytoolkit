Publish
=======

pypi
----

`配置 pypi token <https://pypi.org/manage/account/token/>`_

.. code-block:: shell

  # 配置token
  poetry config pypi-token.pypi pypi-XXXXXXXXXXXXXXXXXXX
  poetry build
  poetry publish

test.pypi
---------

`配置 test.pypi token <https://test.pypi.org/manage/account/token/>`_

.. code-block:: shell

  poetry config repositories.test-pypi https://test.pypi.org/legacy/
  # 配置token
  poetry config pypi-token.test-pypi pypi-XXXXXXXXXXXXXXXXXXX
  poetry build
  poetry publish -r test-pypi

.. code-block:: shell

  mkdir -p /tmp/test_toolkit_cmm
  cd /tmp/test_toolkit_cmm
  poetry init -q
  poetry source add testpypi https://test.pypi.org/simple/
  poetry add --source testpypi toolkit_cmm
  poetry run python3 -c 'from toolkit_cmm.helloworld import hello_world;print(hello_world());'

issues
------
`keyring issue <https://github.com/python-poetry/poetry/issues/1917>`_
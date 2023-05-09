Linting
=======

format
------

`black <https://github.com/psf/black>`_ is not configurable, such as 2-space-indentation, and i use different language not only python, configurable makes my formatting of different languages more consistent.

.. code-block:: 

  poetry run yapf -i  --recursive toolkit_cmm/


typing
------

.. code-block:: 

  poetry run mypy toolkit_cmm
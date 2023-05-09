Dependency
==========

Add
---

.. code-block:: shell

  poetry add xxx --group dev

List
----


.. code-block:: shell
  
  poetry show --tree


create requirements.txt
-----------------------

.. code-block:: shell
  
  poetry export -f requirements.txt -o requirements.txt --without-hashes --with dev

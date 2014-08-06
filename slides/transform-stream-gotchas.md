## Gotchas

- streams use the ``Buffer`` object
- ``push``ing objects will ``throw`` an error
- use ``_flush`` to ``push`` the remaining data in the buffer
- implementations should be a factory of a ``Transform`` stream
- ``end`` event is fired after ``_flush``ing all data
- ``Transforms`` inherits parasitically from ``Write`` 
========
Protocol
========

    :Author: David Joseph

.. contents::

1) An Unrival object (hereinafter simply referred to as *an object*) satisfies all of the following conditions:

.. details::

    .. code:: elisp

        (message "Dummy code")

1) An object is uniquely determined by an address.

2) A name is a possibly non-unique, humanly-readable way of referring to an object.

3) An interpretation is a hierarchical ordering of names.

4) A universe is a mapping from interpretations to addresses.

5) A proof is an object which, given another object and within a certain universe, is either satisfied by or not satisfied by this other object.

6) If an object references a proof, it must satisfy this proof.

7) An ancestor is an object from which another object inherits, such that the inheriting object must satisfy any proofs referenced by its ancestor(s) in addition to those it references directly.

8) A namespace is a set of names that can be considered equivalent for some purpose.

9) An object must reference a universe in which any ancestors it references may be interpreted.

10) If an object references a namespace,

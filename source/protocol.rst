========
Protocol
========

    :Author: David Joseph

.. contents::

1. An Unrival object satisfies all of the following conditions:

2. An  object is uniquely determined by an address.

3. A proof is an object which, given another object, is either satisfied or not satisfied by this other object.

4. An object may reference a proof.

5. If an object references a proof, it must satisfy this proof.

6. An ancestor is an object from which another object inherits, such that the inheriting object must satisfy any proofs referenced by its ancestor(s) in addition to those it references directly.

7. A name is a possibly non-unique label by which an object can be called.

8. A namespace is a set of names that can be considered equivalent for some purpose.

9. A universe:

   - assigns a hierarchy to a set of namespaces

   - maps each namespace to an address

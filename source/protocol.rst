========
Protocol
========

    :Author: David Joseph

**0) An Unrival object (hereinafter simply referred to as an *object*) satisfies all of the following conditions:**

**1) An object is uniquely determined by an address.**

e.g.

.. code:: org

    QmVRTb6yL9cajcHLeVG369zTMXXEgCiwW6qpcZHf3s1LMU

1.1) If an object is composed of references to other objects by their addresses, it is a complex object; otherwise it is a simple object.  The set of objects referenced by some object can be referred to as its *parts*.

**2) A name is a simple object and a possibly non-unique, humanly-readable way of referring to other objects.**

*Name:*

.. code:: org

    dog

*Address (distinct):*

.. code:: org

    QmXQKbAA75HTxiGQz3JJzzLgn2PJc7nRVM2jXPRJGGwK3Y

**4) An interpretation is a simple object and a hierarchical ordering of names, where levels are conventionally separated by slashes (/) and the bottom level comes last.**

e.g.

.. code:: org

    /animal/mammal/dog

4.1) If an object references an interpretation, then the bottom level can be considered its name (or one of its names).

**5) A context is a complex object and a mapping from interpretations to addresses of other objects (these addresses being referred to as their meanings).**

e.g.

.. code:: json

    [
        {
            "interpretation": "/interpretation",
            "address": "QmWDd8Fc3hXevickhyxZqo5UhLJutWiJraNxjx4YCqnJ3m",
            "meaning": "<address_of_another_object>"
        }
    ]

5.1) Every complex object contains a context that may be required to interpret this object, with the exception of the empty context.  Therefore, the above example cannot be a valid object until it references a context:

*Note: certain fields of an object, like address in the following, may be left out of examples when they are irrelevant.*

.. code:: json

    [
        {
            "interpretation": "/interpretation",
            "address": "QmWDd8Fc3hXevickhyxZqo5UhLJutWiJraNxjx4YCqnJ3m",
            "meaning": "<address_of_another_object>"
        },
        {
            "interpretation": "/context"
        }      
    ]

*The empty context:*

.. code:: json

    [{}]



**6) A proof is a simple object which, given another object and in the context of some context, is either satisfied by or not satisfied by this other object (represented by 1 or 0, respectively).**

6.1) If an object references a proof, it must satisfy this proof.

**7) A claim is a complex object which, given another object and in the context of some context, can be satisfied by this other object to a certain degree represented by a number between 0 and 1 (inclusive).**

7.1) Claims and proofs assert things about objects and can simply be referred to as *assertions* for the purpose of generalization.

**9) An ancestor is an object from which another object inherits, such that the inheriting object must satisfy any proofs referenced by its ancestor(s), or ancestors of its ancestors, in addition to those it references directly.**

9.1) If an object references a multi-level interpretation, then it inherits from the objects referred to (ambiguously) at higher levels.

*dog, in the following:*

.. code:: org-mode

    /animal/mammal/dog

*inherits from:*

.. code:: org-mode

    mammal

*which in turn inherits from:*

.. code:: org-mode

    animal

9.2) A context is needed to decide which objects are referred to by (i.e. interpret) higher levels of an interpretation referenced by some object.

9.3) A context referenced by an object must be able to interpret the higher levels of any interpretation it references.

**10) A namespace is a set of names that can be considered equivalent for some purpose.**
**11) An object must reference a context in which any ancestors it references may be interpreted.**
**12) If an object references a namespace,**

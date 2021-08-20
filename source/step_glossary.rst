features Glossary
=================

- :term:`a claim`
- :term:`a claim attached to this object`
- :term:`a namespace`
- :term:`a namespace containing the name object`
- :term:`a namespace containing the name universe`
- :term:`a private key`
- :term:`a proof`
- :term:`a prospective object of this namespace includes this claim`
- :term:`a protocol`
- :term:`a public key is generated from this private key`
- :term:`a set of parts containing but not satisfying this proof`
- :term:`a set of parts including a namespace and a universe`
- :term:`a universe containing this namespace`
- :term:`a universe not containing this namespace`
- :term:`a universe only containing the base namespace`
- :term:`an address for a proof`
- :term:`an agent subscribed to this namespace`
- :term:`an interpretation`
- :term:`an interpretation associating the namespace with an object`
- :term:`an interpretation whereby universe inherits from object`
- :term:`an object can be created from these parts`
- :term:`an object cannot be created from these parts`
- :term:`an object is created from these parts`
- :term:`an object is stored at an updateable address`
- :term:`an object of this namespace`
- :term:`executing the code at this address should return a valid exit code`
- :term:`it can be proved`
- :term:`it can be read and parsed`
- :term:`no address will be returned when this namespace is looked up`
- :term:`parts containing these objects`
- :term:`the base interpretation`
- :term:`the empty universe`
- :term:`the namespace proof`
- :term:`the object located at this address has a proof`
- :term:`the object proof`
- :term:`the root proof`
- :term:`the subscribed agent`
- :term:`the subscribed agent will be notified of the claim`
- :term:`the universe proof`
- :term:`these parts satisfy this proof`
- :term:`this address will be returned when this namespace is looked up`
- :term:`this agent judges this claim to be invalid`
- :term:`this agent judges this claim to be valid`
- :term:`this object is created`
- :term:`this object now has a validity score of -1`
- :term:`this object now has validity score of 1`
- :term:`this private key can be used to verify identity associated with the public key`
- :term:`this universe has an address associated with this namespace`

.. glossary::
    a namespace
        | features/Claim.feature 5
        | features/Judgment.feature 4, 12
        | features/Universe.feature 13, 18

    an object is created from these parts
        | features/Namespace.feature 10
        | features/Object.feature 9
        | features/Universe.feature 8

    it can be proved
        | features/Namespace.feature 12
        | features/Object.feature 10
        | features/Universe.feature 10

    an agent subscribed to this namespace
        | features/Claim.feature 6
        | features/Judgment.feature 6, 14

    a universe containing this namespace
        | features/Namespace.feature 7
        | features/Universe.feature 14

    parts containing these objects
        | features/Namespace.feature 9
        | features/Object.feature 7

    it can be read and parsed
        | features/Namespace.feature 11
        | features/Universe.feature 9

    an object of this namespace
        | features/Judgment.feature 5, 13

    a claim attached to this object
        | features/Judgment.feature 7, 15

    a set of parts including a namespace and a universe
        | features/Object.feature 13, 20

    the object located at this address has a proof
        | features/Object.feature 15, 22

    these parts satisfy this proof
        | features/Object.feature 16, 23

    an object can be created from these parts
        | features/Object.feature 17, 24

    a proof
        | features/Object.feature 27, 32

    a set of parts containing but not satisfying this proof
        | features/Object.feature 28, 33

    an object cannot be created from these parts
        | features/Object.feature 29, 34

    a private key
        | features/Agent.feature 4

    a public key is generated from this private key
        | features/Agent.feature 5

    this private key can be used to verify identity associated with the public key
        | features/Agent.feature 6

    a claim
        | features/Claim.feature 7

    a prospective object of this namespace includes this claim
        | features/Claim.feature 8

    this object is created
        | features/Claim.feature 9

    the subscribed agent will be notified of the claim
        | features/Claim.feature 10

    the subscribed agent
        | features/Claim.feature 11

    an object is stored at an updateable address
        | features/Claim.feature 16

    this agent judges this claim to be invalid
        | features/Judgment.feature 8

    this object now has a validity score of -1
        | features/Judgment.feature 9

    this agent judges this claim to be valid
        | features/Judgment.feature 16

    this object now has validity score of 1
        | features/Judgment.feature 17

    the root proof
        | features/Namespace.feature 4

    the namespace proof
        | features/Namespace.feature 5

    a namespace containing the name object
        | features/Namespace.feature 6

    an interpretation
        | features/Namespace.feature 8

    the object proof
        | features/Object.feature 4

    the empty universe
        | features/Object.feature 5

    the base interpretation
        | features/Object.feature 6

    a protocol
        | features/Object.feature 8

    an interpretation associating the namespace with an object
        | features/Object.feature 14

    this universe has an address associated with this namespace
        | features/Object.feature 21

    an address for a proof
        | features/Proof.feature 8

    executing the code at this address should return a valid exit code
        | features/Proof.feature 9

    a universe only containing the base namespace
        | features/Universe.feature 4

    the universe proof
        | features/Universe.feature 5

    a namespace containing the name universe
        | features/Universe.feature 6

    an interpretation whereby universe inherits from object
        | features/Universe.feature 7

    this address will be returned when this namespace is looked up
        | features/Universe.feature 15

    a universe not containing this namespace
        | features/Universe.feature 19

    no address will be returned when this namespace is looked up
        | features/Universe.feature 20


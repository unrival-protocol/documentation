.. role:: gherkin-step-keyword
.. role:: gherkin-step-content
.. role:: gherkin-feature-description
.. role:: gherkin-scenario-description
.. role:: gherkin-feature-keyword
.. role:: gherkin-feature-content
.. role:: gherkin-background-keyword
.. role:: gherkin-background-content
.. role:: gherkin-scenario-keyword
.. role:: gherkin-scenario-content
.. role:: gherkin-scenario-outline-keyword
.. role:: gherkin-scenario-outline-content
.. role:: gherkin-examples-keyword
.. role:: gherkin-examples-content
.. role:: gherkin-tag-keyword
.. role:: gherkin-tag-content

:gherkin-feature-keyword:`Feature:` :gherkin-feature-content:`Namespace`
========================================================================

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`create base namespace`
---------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` the root proof
| :gherkin-step-keyword:`And` the namespace proof
| :gherkin-step-keyword:`And` a namespace containing the name object
| :gherkin-step-keyword:`And` a universe containing this namespace
| :gherkin-step-keyword:`And` an interpretation
| :gherkin-step-keyword:`And` parts containing these objects
| :gherkin-step-keyword:`And` an object is created from these parts
| :gherkin-step-keyword:`Then` it can be read and parsed
| :gherkin-step-keyword:`And` it can be proved

::

    Scenario\: subscribe to a namespace

      Given an agent

      And a namespace

      When this agent subscribes to this namespace

      Then this agent is in the namespace's subscribers list



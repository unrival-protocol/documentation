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

:gherkin-feature-keyword:`Feature:` :gherkin-feature-content:`Universe`
=======================================================================

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`create base universe`
--------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a universe only containing the base namespace
| :gherkin-step-keyword:`And` the universe proof
| :gherkin-step-keyword:`And` a namespace containing the name universe
| :gherkin-step-keyword:`And` an interpretation whereby universe inherits from object
| :gherkin-step-keyword:`And` an object is created from these parts
| :gherkin-step-keyword:`Then` it can be read and parsed
| :gherkin-step-keyword:`And` it can be proved

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`get an address for a namespace`
------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a namespace
| :gherkin-step-keyword:`And` a universe containing this namespace
| :gherkin-step-keyword:`Then` this address will be returned when this namespace is looked up

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`fail to get an address for a namespace`
--------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a namespace
| :gherkin-step-keyword:`And` a universe not containing this namespace
| :gherkin-step-keyword:`Then` no address will be returned when this namespace is looked up


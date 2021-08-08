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

:gherkin-feature-keyword:`Feature:` :gherkin-feature-content:`Object`
=====================================================================

    :gherkin-feature-description:`As an agent`
    :gherkin-feature-description:`In order to coordinate with other agents more effectively`
    :gherkin-feature-description:`I want an affordance that ensures that other agents and I are referring to the same things when we communicate`

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`create object`
-------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a proof
| :gherkin-step-keyword:`And` a set of parts satisfying this proof
| :gherkin-step-keyword:`Then` an object can be created from these parts

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`create object with prototype`
----------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a propsective object includes a prototype
| :gherkin-step-keyword:`And` a name exists equal to the label of this prototype
| :gherkin-step-keyword:`And` a namespace exists that includes this name
| :gherkin-step-keyword:`And` this prospective object can pass its prototype's proof
| :gherkin-step-keyword:`Then` this prospective object can be created

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`fail to create object due to direct proof failure`
-------------------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a propsective object includes a proof
| :gherkin-step-keyword:`And` this prospective object can't satisfy this proof
| :gherkin-step-keyword:`Then` this prospective object can't be created

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`fail to create object due to immediate ancestor prototype failure`
-----------------------------------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a propsective object includes a prototype
| :gherkin-step-keyword:`And` this prospective object can't satisfy its prototype's proof
| :gherkin-step-keyword:`Then` this prospective object can't be created

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`fail to create object due to nth-degree ancestor prototype failure`
------------------------------------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a propsective object includes a prototype
| :gherkin-step-keyword:`And` this prospective object can't satisfy its prototype's proof
| :gherkin-step-keyword:`Then` this prospective object can't be created

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`fail to create object due to claim failure`
------------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a propsective object includes a claim
| :gherkin-step-keyword:`And` this claim can't be substantiated
| :gherkin-step-keyword:`Then` this prospective object can't be created


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

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`create a namespace`
------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a name
| :gherkin-step-keyword:`Then` a namespace can be created from this name

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`create a nested namespace`
-------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a namespace
| :gherkin-step-keyword:`And` a name
| :gherkin-step-keyword:`Then` a namespace can be created from this name that inherits from this namespace

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`subscribe to a namespace`
------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` an agent
| :gherkin-step-keyword:`And` a namespace
| :gherkin-step-keyword:`When` this agent subscribes to this namespace
| :gherkin-step-keyword:`Then` this agent is in the namespace's subscribers list


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

:gherkin-feature-keyword:`Feature:` :gherkin-feature-content:`Claim`
====================================================================

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`attach a claim to a prospective object`
--------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a namespace
| :gherkin-step-keyword:`And` an agent subscribed to this namespace
| :gherkin-step-keyword:`And` a claim
| :gherkin-step-keyword:`And` a prospective object of this namespace includes this claim
| :gherkin-step-keyword:`And` this object is created
| :gherkin-step-keyword:`Then` the subscribed agent will be notified of the claim
| :gherkin-step-keyword:`And` the subscribed agent

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`attach a claim to an existing object`
------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` an object is stored at an updateable address


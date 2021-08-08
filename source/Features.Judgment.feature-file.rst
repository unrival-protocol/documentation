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

:gherkin-feature-keyword:`Feature:` :gherkin-feature-content:`Judgment`
=======================================================================

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`judge a claim to be invalid`
---------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a namespace
| :gherkin-step-keyword:`And` an object of this namespace
| :gherkin-step-keyword:`And` an agent subscribed to this namespace
| :gherkin-step-keyword:`And` a claim attached to this object
| :gherkin-step-keyword:`When` this agent judges this claim to be invalid
| :gherkin-step-keyword:`Then` this object now has a validity score of -1

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`judge a claim to be valid`
-------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a namespace
| :gherkin-step-keyword:`And` an object of this namespace
| :gherkin-step-keyword:`And` an agent subscribed to this namespace
| :gherkin-step-keyword:`And` a claim attached to this object
| :gherkin-step-keyword:`When` this agent judges this claim to be valid
| :gherkin-step-keyword:`Then` this object now has validity score of 1


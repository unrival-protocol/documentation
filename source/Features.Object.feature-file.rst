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

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`create base object`
------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` the object proof
| :gherkin-step-keyword:`And` the empty universe
| :gherkin-step-keyword:`And` the base interpretation
| :gherkin-step-keyword:`And` parts containing these objects
| :gherkin-step-keyword:`And` a protocol
| :gherkin-step-keyword:`And` an object is created from these parts
| :gherkin-step-keyword:`Then` it can be proved

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`create object with ancestor`
---------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a set of parts including a namespace and a universe
| :gherkin-step-keyword:`And` an interpretation associating the namespace with an object
| :gherkin-step-keyword:`And` the object located at this address has a proof
| :gherkin-step-keyword:`And` these parts satisfy this proof
| :gherkin-step-keyword:`Then` an object can be created from these parts

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`create object with ancestor and own proof`
-----------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a set of parts including a namespace and a universe
| :gherkin-step-keyword:`And` this universe has an address associated with this namespace
| :gherkin-step-keyword:`And` the object located at this address has a proof
| :gherkin-step-keyword:`And` these parts satisfy this proof
| :gherkin-step-keyword:`Then` an object can be created from these parts

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`fail to create object due to own proof failure`
----------------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a proof
| :gherkin-step-keyword:`And` a set of parts containing but not satisfying this proof
| :gherkin-step-keyword:`Then` an object cannot be created from these parts

:gherkin-scenario-keyword:`Scenario:` :gherkin-scenario-content:`fail to create object due to ancestor proof failure`
---------------------------------------------------------------------------------------------------------------------

| :gherkin-step-keyword:`Given` a proof
| :gherkin-step-keyword:`And` a set of parts containing but not satisfying this proof
| :gherkin-step-keyword:`Then` an object cannot be created from these parts

::

    Scenario\: fail to create object due to non-unique labels

      Given a propsective object includes a proof

      And this prospective object can't satisfy this proof

      Then this prospective object can't be created

    

    Scenario\: fail to create object due to missing parts

      Given a prospective object includes a prototype

      And a name exists equal to the label of this prototype

      And a namespace exists that includes this name

      

    

    Scenario\: fail to create object due to immediate ancestor prototype failure

      \# indirect proof

      Given a propsective object includes a prototype

      And this prospective object can't satisfy its prototype's proof

      Then this prospective object can't be created

    

    Scenario\: fail to create object due to nth-degree ancestor prototype failure

      \# indirect proof

      Given a propsective object includes a prototype

      And this prospective object can't satisfy its prototype's proof

      Then this prospective object can't be created  



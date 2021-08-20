==========
Whitepaper
==========

    :Author: David Joseph



Abstract
--------

Unrival is a protocol that enables its users (agents) to cooperate more effectively on accomplishing common goals.  Agents communicate their intentions via a set of shared objects, which constitute composable, bottom-up building blocks for maintaining complex social and economic relationships founded on mutual understanding and accountability.

Any thing whose existence or validity can be confirmed or denied by third parties is an eligible Unrival object.  This may leaves out some things, like agents' internal states, or inherentily unfalsifiable claims, but most things are included.  In particular, those things with compromised credibility as of late, upon which many people may nonetheless come to depend -- like political parties, medicines, cryptocurrencies, advertisements, etc. -- are eligible objects.  Thus, the credibility of these things can be asserted by their proponents, and confirmed or denied by the agents who experience them.

The protocol itself can be stated as `a set of guidelines <protocol.html>`_ that are open to interpretation as far as technological implementation goes.  An implementation seeking to mitigate the failure modes associated with some technological modalities will be described in the following, but it is by no means the only possible interpretation.

Overview
--------

Introduction
~~~~~~~~~~~~

Unrival seeks to pave a road to cooperation when defection seems, in the realest sense, like the more rational choice for self-interested agents.  As it is meant to be realistic and not fanciful, it does so without appealing to the moral inclinations of its subjects - but instead by re-framing self-interest and laying bare latent incentives to cooperate.

But, where agents stand to benefit maximally by cooperating, shouldn't they be doing so already?  This may seem paradoxical, but not always.  Think of Mutually Assured Destruction: although individual nations may prefer all-around nuclear disarmament, they'd be crazy (by this calculus) to adopt this strategy - doing so would only give other nations a leg up in the struggle for international dominance, and would be very unlikely to bring about the optimaly outcome.  Thus, in a nuclear-armed world, nations are trapped in a *race to the bottom*.

In short, our problem boils down to: *how can we cooperate when we are stuck in rivalrous equilibria*?  Unrival is an attempt at a technological answer to this question.  Our answer starts with a set of shared concepts, the use of which lowers the coordination costs (e.g. the requisite energy, the inherent risk, and so on) associated with cooperating.  This has the effect of putting maximally beneficial outcomes within agents' reach.  Thus, agents using Unrival outcompete those that don't.  Although selfish individuals beat non-selfish individuals, non-selfish groups beat selfish groups, according to `multi-level selection theory <https://en.wikipedia.org/wiki/Group_selection#Multilevel_selection_theory>`_.

The Stag Hunt
~~~~~~~~~~~~~

*We'd like to take this opportunity to drive home the notion that greater benefit is sometimes theoretically possible, but is nonetheless passed over by self-interested agents. Readers who are familiar with game theory may feel free to skip this section.*

The following scenario was introduced by Rousseau in his `Discourse on Inequality <https://en.wikipedia.org/wiki/Discourse_on_Inequality>`_:

    …two individuals go out on a hunt. Each can individually choose to hunt a stag or hunt a hare. Each player must choose an action without knowing the choice of the other. If an individual hunts a stag, they must have the cooperation of their partner in order to succeed. An individual can get a hare by himself, but a hare is worth less than a stag.

This leads to a paradoxical situation in which *acting rationally* means *settling for a sub-optimal outcome*.  Although both hunters would rather come home with a stag, they are forced to hunt for hares - otherwise they could be left with nothing.

.. image:: ./static/images/stag_hunt.png

**Key Takeaways**

- There exist paradoxical situations in which self-interested agents choose strategies leading to suboptimal outcomes.

- Should agents attempt to cooperate, they are confronted by some difficulties:     

  - Communication may be impossible or so costly that, should it lead to optimal outcomes, nonetheless offsets the benefit such that agents choose not to communicate.  Besides the costs of physical media, like smoke signals and fiber optics, this costliness may materialize in:

  - The ability of agents to deceive one another, whereby they forego an ideal outcome but gain the upper hand over their rivals.

Thus, there are no simple solutions to coordination problems, as proposed solutions (e.g. better, faster communication channels) often enable more efficient deception for any added benefit.  Unrival introduces a meta-game for overcoming these difficulties.

The Meta-Game
~~~~~~~~~~~~~

One thing is certain: it really is the most rational choice for hunters to hunt for hares - *within the confines of the staghunt game*.  But games aren't real life; their rules don't necessarily reflect the full range of choices available to agents.  It may also be possible to play a meta-game that can improve outcomes within the given game.

The subject of this paper is a group protocol for playing meta-games.  Such a protocol should confer enough benefit on its users to outweigh any associated costs associated with its use.

The original problem wouldn't be solved if only the hunters had access to cell phones.  There can still be an incentive to distort data.  

So the group method is as follows:

- Make signals between agents easy to send

- Make it easy for agents to interpret these signals based on evidence

- For example, if an agent has many broken promises on Unrival, this may make you less likely to rely on them.

The Meta-Crisis
~~~~~~~~~~~~~~~

The growing threat of disasters in the world due to climate change should be cause for serious concern.  It is obvious we are not properly preparing.  Even when we know something bad is about to happen, we aren't able to avert the worst of it by prudent planning; instead, we suffer needlessly in many cases.

storm-warning systems, for one, haven't been very successful in getting people to evacuate areas.  Why is that?

It is ever more the case that there is no central source of truth.  Which warnings should we heed?  Which threats are mere exaggerations?  If the 'official wisdom' is that I should flee an area due to a storm warning, should I or not?

Narratives can be concocted to support any sort of conclusion - this is becoming apparent.  

But nevertheless, sometimes there are times when all narratives break down.


Also, public goods are underfunded.  This is a problem of incentives.  When there isn't much benefit in offering a public good, things that are inherently non-rival and non-exclusive are rarer than they need to be (like reliable information).  (There is no lack of incentive to distribute unreliable information.  There's not a lot of money in telling the truth, but telling lies can make you rich).  Part of this has to do with the fact that our information ecology is as polluted as our planetary ecology.  But when we realize our environment is becoming unlivable, how should we respond?  Just as people are starting to wake up to the level of havoc that the climate crisis can potentially unleash, it's also becoming clear that unreliable information, and lots of it, creates another type of crisis - a `meaning crisis <https://www.youtube.com/watch?v=54l8_ewcOlY&list=PLND1JCRq8Vuh3f0P5qjrSdb5eC1ZfZwWJ>`_.

The Internet of X
~~~~~~~~~~~~~~~~~

**ywhere *X* is {goals, ideas, theories, ...}**       

One concept central to Unrivyal is the **goal**, which helps agents decide which actions to take, as well as ensure that individual efforts can be effectively combined into a group effort more potent than the sum of its parts.

Also was mentioned the fact that new concepts can be added to the Unrival arsenal.  It's an extendable protocol with no central authority (though there is no guarantee new concepts will become widely adopted).  So let's add a concept:

Suppose a developer is passionate about *todo lists*, and wants to make a way for users to interact with them.  They do the following:

- create a todo list type, from which instances of todo lists can be made

- make this type *claimable* - i.e.

The Goal Engine
~~~~~~~~~~~~~~~

1. enables access to non-rivalrous resources

Universal Feedback
~~~~~~~~~~~~~~~~~~

Objects
-------

As mentioned, Unrival is based on concepts that improve the ability of agents to cooperate.  It accomplishes this by giving agents a language for finding common ground with others.  Underlying this is the assumption that agents may err or deceive while communicating about objects (as certain auto mechanics are won't to do when informing customers which repairs their cars will need, or used car dealers as they unload their lemons on the unsuspecting.  Most industries are full of examples).  Therefore, common ground must be built on trust, and objects must have this baked into them.

Unrival can be seen as a way of making sure objects are what they say they are.  In order to accomplish this, we make any objects amenable to verification.  Objects reference *proofs* and/or *claims*, either directly or indirectly, and these must be falsifiable.  A **proof** is a computer program that checks whether some object has certain properties.  A **claim** is like a proof that requires input from human agents, usually because the satisfiability criteria are subjective.  For example, a proof may require some integer stored at address X to be divisible by 3, while a claim can be made that this integer is a lucky number.

Proof
^^^^^

In Unrival, anything that exists does so because of its having been proved in some way.

- Proof can have **subjectively** or **objectively** defined criteria for satisfiability.

- A subjectively defined proof requires agents to assess the validity of the proof.

  - there are two ways for agents to give feedback on validity

    - when an object is created, it is done so with subjective defined criteria for success

    - at random intervals, objects are checked for validity (i.e. their proofs are run).  if invalid, they are pruned.

    -

- Formalising Subjectively executed proofs, also called **assessments**, are part of a possible protocol that has a curated set of concepts for reflecting a satisfying intersubjective **universe**

Object
^^^^^^

An object is just any whole that has parts.  In order to be an unrival object, something needs to have a content-addressed representation of these parts.  

Criteria
::::::::

- any object that comes into existence must meet certain proof criteria

- objects must meet both subjective and objective proof criteria

- objects may meet objective proof criteria that don't belong to them specifically, but rather belong to class to which they belong (proof criteria can be inherited)

- 


It is difficult to query for subjective opinions about things that matter and get faithful results.

Simple Objects
~~~~~~~~~~~~~~

Objects are content-addressed arrays of **parts**.  For example, the following object has two parts:

.. code:: json

    [
      {
        "label": "breed",
        "value": "Dalmation"
      },
      {
        "label": "name",
        "value": "Daisy"
      }  
    ]

A process called hashing can be used to create a signature from data that will always look the same, given the same input data.

Hashing the above data using IPFS produces the content-based address ``QmeDWRWMc3YoRKyueRAmqmJ3bVwD1oc74eVoEATtfdYJJh``.  This is similar to an IP address in that it can be used to fetch data, but it also comes with certain advantages owing to the direct relationship between the content of the data and the address itself.

Simple objects are objects that do not contain other objects embedded in them.  Since neither of the above object's parts are content-addressed objects, it is a simple object.

Name
^^^^

Currently there is only need for one type of simple object - a *name*.  A **name** acts as a mnemonic label attached to (i.e. part of) other objects.  Names can have attributes (like "language\ :sub:`code`\" in the following example), which can be useful in various client applications:

.. code:: json

    [
        {
            "type": "name",
            "value": "dog",
            "language_code": "EN"
        }
    ]

Image
^^^^^

Proofs
~~~~~~

A **proof** is a program that is fed an address as its input and terminates in either success or failure, usually dependent upon the attributes of the data at said address.  

There are two types of proofs: subjective and objective.  
An object has been proved **objectively** if passing the proof was a mathematical certainty, given the address.      
An object has been proved **subjectively** if it reflects the opinions of faithful observers.

Objective
^^^^^^^^^

Most of Unrival's advanced functionality is due to the ability of complex objects to be *proved*, either directly or indirectly.  Objects that are proved directly have a proof part, while objects proved indirectly have a prototypal parent with a proof they must also satisfy:

.. image:: static/images/proofs.svg

To continue our example from above, if the following code is hashed and added as a part to the Dalmation object, it would make sure that the breed of dog is equal to ``'Dalmation'``.

.. code:: python

    #!/usr/bin python3

    from unrival_py import *

    address = sys.argv[1] # could be equal to the above hash, for example (QmeDWRWMc3YoRKyueRAmqmJ3bVwD1oc74eVoEATtfdYJJh)

    object_string = read(address) # gets the data from the content-address
    parsed_object = parse(object_string) # converts the data into a python dictionary

    assert has_part(parsed_object, 'breed', 'Dalmation') 

Direct Proof
::::::::::::

Once we hash the above and add it as a part to our original set, we have the following:

.. code:: json

    [
      {
        "type": "proof",
        "address": "QmV7HTZJqd81DWo12MVmB6BtkS8V28JNU3587HPsJj1rv6"
      },
      {
        "label": "breed",
        "value": "Dalmation"
      },
      {
        "label": "name",
        "value": "Daisy"
      }  
    ]

One more hash gives us the result: ``QmWJwaDMcKgysTwC2qktH27eqYHHauNXHryhzTzNN8szub`` - which is a content-based address that can be fed to a proof.  The object at this address is claiming to be a Dalmation (rightfully so, based on the rather easily-satisfied proof above that it includes as one of its parts).

*When an object's content address is fed to a a proof that is contained as one of its parts, it is proved directly.*

Indirect Proof
::::::::::::::

Some objects do not contain explicit references to proofs.  Instead, they contain references to prototypes, whose proofs they must satisify.  

.. image:: static/images/indirect-proof-1.svg

This means that in order to come into existence, "some dalmation" must satisfy both the life form proof and the mammal proof, besides its namesake proof:

.. image:: static/images/indirect-proof-2.svg

Multiple Inheritance
::::::::::::::::::::

Archetypal Proof
::::::::::::::::

The properties of proofs described above are determined by a single proof, called an **archetypal proof**.  This is part of an **archetypal object**, which is an object all complex objects in Unrival have as an ancestor.

Subjective
^^^^^^^^^^

Subjective Proofs are required for each and every Unrival object.  Not every object

Complex Objects
~~~~~~~~~~~~~~~

Namespace
^^^^^^^^^

A **namespace** is a collection of names that can be considered equivalent for some purpose.  

.. image:: static/images/namespace.svg

In Unrival there are two kinds of names:

Authoritative
:::::::::::::

Also called an object's *type*, this is an indication to prefer one name over others -- when there are multiple name variants referring to the same object -- for the purpose of simplicity.

Non-Authoritative
:::::::::::::::::

Non-authoritative names are variants of an authoritative name.

For example, Unrival Clients and Servers (if they implement Universe \_\_) can also refer to objects of type *agent* as *actors*.  The former is authoritative and the latter is a non-authoritative variant.

Agent/Actor/User
^^^^^^^^^^^^^^^^

Outcome/Event
^^^^^^^^^^^^^

An outcome is a claim that is a subjective event.      

Claim (Subjective Proof Criteria)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

A claim is just a subjective proof that hasn't been validated.

Every object must start with a claim, and this claim, after having been proved, allows the object to exist.

Judgment/Evaluation/Assessment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

::

    “Never trust anyone who doesn’t have skin in the game. Without it, fools and crooks will benefit, and their mistakes will never come back to haunt them.” - Nassim Nicholas Taleb


An evaluation is a verification attempt by a certain number of agents of a subjective proof.  Therefore it is an event - but it can be ongoing; current attempts at proof evaluation may still be relevant for agents.

It is difficult to query for subjective opinions about things that matter and get faithful results.

A judgment has value.  A very strong case can be made for it being the utility token par excellence.  Judgments are necessarily honest representations of mental states.  This is what is quite hard to get at through polling, surveys, or reviews of any sort.

- Youtube's way of recommending tends to appeal to our lowest common denominators

- Amazon's way of recommending is very gameable.  Nothing is stopping vendors from offering incentives to offer unfaithful ratings, which distorts the signal that users are looking for to help them make a decision.

Assessments in Unrival are elicited in a way that maximizes the faithfulness of responses.  Whenever a claim is made, a namespace is also attached to this claim.  The subscribers to the namespace where the claim is made are the pool of possible judges.

Promise
^^^^^^^

Of course, there are many ways to think about promises, some of them requiring no formalism or technology.  Our approach is meant to make promises applicable in many circumstances, and it starts with breaking promises into their component parts and making them interfaceable.  We call the component parts of a promise *objects*.  These are anything and everything that could be relevant to the management of promises.  In order to use them the way we want, as representations of complex human relationships, we have some criteria:    

Goal
^^^^

Interface
^^^^^^^^^

An **interface** is a composition of a set of actions performable by some user(s).  For example, an interface may look like the following:

.. code:: json

    [
        {
            "type": "interface",
            "name": "prototype"
        },
        {
            "type": "action",
            "name": "pay bill",
        },      
        {
            "type": "action",
            "name": "check bill",
        }
    ]

This information alone is sufficient to define an interface in Unrival.  

Action
^^^^^^

An **action** should be performable in order to produce a desired outcome, without error.  Because actions are tied to *ends* and not *means*, there may be several alternate ways to perform actions.  This is why *actions aggregate adapters and providers*.  

.. code:: json

    [
        {
            "type": "action",
            "name": "prototype"
        },
        {
            "type": "provider",
            "name": "pay bill",
        },      
        {
            "type": "provider",
            "name": "check bill",
        }
    ]

may contain an aggregate of adapters representing these diverse means.  Means, at this level, refers to a medium and not the provider of a medium.  In other words, given the action *pay bill*, one adapter (technically a *null* adapter) would allow you to pay in person, while another adapter would allow you to wire money from your bank account.  This leaves open the possibility for different providers to fulfill the transfer, which will be covered.

Adapter
^^^^^^^

Universe
^^^^^^^^

Every unrival object that is created has a universe in which it was created as one of its parts.  This reference to a universe's content based address shows a client whether or not an object that doesn't belong to their universe can be merged.




A universe is like a filesystem that maps names and name hierarchies to data.  

A **universe** determines how concepts are defined for their inhabitants (i.e. users).  The purpose of a universe is to assign a hierarchical order to namespaces.  For example:

.. code:: json

    [
        {
            "type": "namespace",
            "address": "@#q23kflj2fkl3jrkl23j23kf",
            "children": [
                {
                    "type": "namespace",
                    "address": "",
                    "children": [
                        {
                            "type": "namespace",
                            "address": ""
                        }
                    ]
                }
            }
        }
    ]  

The above addresses correspond to the following goal objects:
"solve climate change" --> "reduce carbon emissions" --> "pass a cap and trade law"
As such, it is an exceedingly simple universe where everything revolves around a cap and trade law getting passed. 

More Complex Objects
~~~~~~~~~~~~~~~~~~~~

Location
^^^^^^^^

Resource
^^^^^^^^

Role
^^^^

Provider
^^^^^^^^

Model
^^^^^

A model is a statement about a state of affairs.

Todo
^^^^

Workflows
---------

Start a Business
~~~~~~~~~~~~~~~~

Sell Your Car
~~~~~~~~~~~~~

Get Insurance
~~~~~~~~~~~~~

- due to asymmetric information being solved, insurance consts less

- 

Implementation
--------------

Python Module
~~~~~~~~~~~~~

Server
~~~~~~

Client
~~~~~~

The purpose of the client is to map Unrival objects to interfaceable components, for example in a web application.

One function of the client is to help users visualize relations between objects.  The Unrival Client has two views:

Router
^^^^^^

A router maps a namespace to a web component.      

WebComponent
^^^^^^^^^^^^

Visualization
^^^^^^^^^^^^^

.. image:: static/images/node-shapes.svg

Detail View
^^^^^^^^^^^

Relation View
^^^^^^^^^^^^^

Search View
^^^^^^^^^^^


# Table of Contents

-   [Abstract](#orgefb1933)
-   [Overview](#org8c52fdb)
    -   [Rectifying Names (正名)](#org37bc859)
        -   [The Mechanism](#orga5d1ef2)
    -   [Rectifying Observations](#orgf205abf)
        -   [First-Order Observation](#org8eee81d)
        -   [Second-Order Observation](#org771be94)
    -   [Rectifying Values](#orgb700ae8)
        -   [The Money to Reputation Pipeline](#org30e8ab1)
        -   [Plugging the Pipeline](#orgc39b542)
-   [Implementation](#orge7378ac)
    -   [Code vs Data](#org965d7bb)
    -   [Objects](#org16be72b)
        -   [Simple Objects](#orgd9277e9)
        -   [Complex Objects](#orgf2b2992)
    -   [Architecture](#orgfbf1be6)
        -   [Server](#org1e68a79)
        -   [Client](#org45b086b)
        -   [Network](#orgbaa6ff8)
-   [Application](#org7cd96e2)
    -   [Rating Systems](#orgb44b28a)
    -   [Decentralized Sensemaking](#orga958bb1)
    -   [Coordination Problems](#org896f0b5)



<a id="orgefb1933"></a>

# Abstract

Unrival is a protocol for tracking the credibility of objects within a network.  Credibility is not defined by a central authority, but rather by objects on their own terms.  Users of this protocol attach claims to objects they interact with in order to let their peers know what can be expected of such interactions.  These peers are then able to assess these claims based on whether outcomes match the expectations they engender.  Over time, the public record of claims and corresponding assessments creates *skin in the game* for participants, whose good faith participation in the network is thus incentivized.


<a id="org8c52fdb"></a>

# Overview


<a id="org37bc859"></a>

## Rectifying Names (正名)

Roughly 2500 years ago, Confucius was asked what he would do if he were governor.  He would *rectify names*, he said, *to make words correspond with reality*.

Unrival can be seen as a technological strategy for accomplishing this.  Whereas Confucius' project may seem impossibly abstract, Unrival is rooted in practical application - from building more effective [rating systems](#orgb44b28a) to enabling decentralized sensemaking.

It starts by addressing the underlying cause Confucius may have been after: the name (the *signifier*) becomes misaligned with the reality (the *signified*) because this benefits someone - usually with influence over how language is used.  Look no further than politics for examples: Does "support the troops" mean keeping troops out of harm's way, or sending them to war?  When the latter becomes the more common usage, it may indicate a misalignment between *name* and *reality* - which in turn points to there being a *someone* benefiting from this.  This benefit is asymmetric - i.e. it comes at a cost to someone else (e.g. the troops).

In the present, what we call *news* comes with a fixed set of associations, or implicit claims that make news *news*.  Whatever is deserving of the title should be relevant and factual, for starters.  Yet, as we're all aware, these descriptions hardly apply to much of what is commonly called news.  To rectify the name *news* would mean creating a mechanism whereby things justifiably called news would tend to reach readers over content that abuses the name.  

Creating such a mechanism, such that it relies on the self-interest of individuals and not on starry-eyed idealism to take flight, is the focus of the next sections.

To preview where we're headed:


<a id="orga5d1ef2"></a>

### The Mechanism

We shall describe a protocol for creating networks of connected objects (e.g. news articles, software repositories, e-commerce offers, or anything else we can give a *name*) that benefit from the feedback of network users <span class="underline">who are incentivized to offer their opinions honestly</span>.  The result is akin to the Web, but with built-in quality control.  *Since the domain of things to which we give names to is becoming synonymous with the domain of things available over the web, we consider this a 21st century revival of Confucius' project*.


<a id="orgf205abf"></a>

## Rectifying Observations

If we consider what it takes to assess public opinion on a matter, we may notice this task growing in difficulty the more those with opinions are aware of the opinions of others.

The German sociologist Niklas Luhmann distinguished between *First Order Observations*, whereby observations lead to spontaneous reactions, and *Second Order Observations*, whereby observers react based on their projections of others' reactions.  John Maynard Keynes illustrated this phenomenon using a beauty pageant in his *General Theory of Employment, Interest and Money*:

> It is not a case of choosing those [faces] that, to the best of one's judgment, are really the prettiest, nor even those that average opinion genuinely thinks the prettiest. We have reached the third degree where we devote our intelligences to anticipating what average opinion expects the average opinion to be. And there are some, I believe, who practice the fourth, fifth and higher degrees.

One key difference between our world and that of Confucius, or Depression-era beauty pageants for that matter, is the supreme importance of second-order observations in informing our judgments.  To live in the digital age is to be immersed in the reactions of others.  We've gone from laugh tracks in 20th century sitcoms (*can I laugh now?*) to explicitly labeled *reaction videos* trending on Youtube.  The concept of watching someone watch a video meant to be watched by oneself would be puzzling indeed without an understanding of the growing prevalence of second order observation.

What implications does this have for our project to rectify names?  Since we are describing a decentralized means of credibility accounting, we are dependent on the judgments of agents for pointing out naming discrepancies.  There are no authoritative standards for determining proper naming - instead, this is determined by the amount of corroboration agents' assessments receive.  In light of what we know about second-order observations, this may present a problem: it is theoretically possible for insincere opinions to be rewarded, if agents have reason to believe they will be corroborated.  Our system must therefore encourage agents to report their first order observations in order to maximize the effectiveness of our bottom-up strategy for credibility accounting (where credibility &#x2013; e.g of an interpretation &#x2013; isn't determined a central authority).  We do so with the knowledge that any observation mediated through a digital environment will be higher-order to some degree.  The challenge, then, is to extract *First Order Information* from Second/Higher Order Observations.


<a id="org8eee81d"></a>

### First-Order Observation

In the following, we consider ways of finding the first-order signal, necessary to rectify names, in environments of second-order noise.

-   Decision Theory

    -   The Utility Function
    
        In his 1969 book *Convention*, philosopher David Lewis pointed out that agents told to go to random locations on a map will not actually choose randomly.  Some locations &#x2013; such as bridges &#x2013; will have inherent value that agents are likely to agree on, and be more likely to go to.  By extension, it is not the case that if you offer two agents $100 each, *should they happen to choose the same location on a map of N x N squares*, then their chances of success are 1 / N<sup>2</sup>.  (Equivalently: the expected value of this offer is > $100/N<sup>2</sup> for each agent).
        
        A similar argument can be made to show that Unrival agents will assess (i.e. stake their credibility on) claims faithfully as a consequence of self interest.  There is one way to be right about a claim, but many ways to be wrong.  The one way of being right &#x2013; in line with unadulterated, first order observation &#x2013; acts as a beacon on a map for self-interested agents to convene upon and profit.
        
        This goes to show that to some degree, it is unnecessary to guard against opinion falsification: *the utility function favors authenticity*.
    
    -   The Possibility of Collusion
    
        Nonetheless, problems may still arise if agents have perfect knowledge of their peers' opinions, and can hold one another accountable in colluding against reality.  It would be possible for agents to vouch against a justified claim and not be punished if they can effectively coordinate on this, in other words.  This becomes less tenable when the colluding agents have no knowledge of each other's actions, and can't verify that their co-conspirators have held to this strategy.  Naturally, agents would prefer not to engage in risky behavior, but still reap the rewards of other agents having done so (a sort of inverse *Tragedy of the Commons*).  A system design that elevates this trouble for the dishonest undermines such schemes.  This goes to show that *varying the amount of information agents have of each other's actions* may be a useful strategy for incentivizing faithful opinion signalling - a precondition for the success of Unrival.

-   Selective Anonymity

    -   Public Votes
    
        When votes are made public (as in the case of congressional votes, for example), public vote-casters are made more accountable for their votes.  But there is also a tradeoff: second-order observation &#x2013; voters considering how their votes will be perceived &#x2013; may cause them to vote against their beliefs.  
    
    -   Private Votes
    
        Private votes are also problematic: they can be cast against the interests of the public without accountability for the voter.  This is particularly a problem when it is possible for an influential minority to verify that votes were cast in their favor, so they can bestow favors on their advocate.  
    
    -   A Compromise
    
        Let us zoom out and consider our goal: to create an accounting ledger that gauges true public opinion in a decentralized manner, not co-optable for the designs of powerful minorities.  To accomplish this, we need to draw on the relative advantages of each type of voting while avoiding their drawbacks:
        
        -   Random Feedback Intervals
        
            Unrival assessments are stored in public ledgers, *eventually*.  At small scales of interaction, if a vote is added to a ledger immediately after an agent provides it, then it can be obvious whose vote was cast.  For example, a tour guide who receives a negative assessment immediately after guiding a client may know who is responsible.  This discourages honest opinion reporting.  (In fact, this is a challenge for services like Yelp, where retribution for negative reviews is non unheard of).
            
            How to get around this without allowing irresponsible assessments?
            
            To assure assessors of their anonymity, Unrival adds entries (i.e. claims) to its ledgers at random intervals.  So our tour guide would have no way of knowing whose assessment caused an update to their credibility, even when this happens immediately after serving a client.
        
        -   Public Results
        
            Unrival's strategy is to internalize the external benefits (e.g. political legitimacy, campaign donations, etc.) that voters gain by voting for the purpose of image.  Ultimately, these things have a monetary value.


<a id="org771be94"></a>

### Second-Order Observation

It is necessary, but not sufficient, for the observations of a population to have a strong first-order component to approach correctness.  It is possible, however, for observers to be wrong in their first-order impressions.  How does Unrival make sure that correct observations rise to the top?  *By making the derived, first-order signal subject to correction from observations of the second order*. 

Citizens voting for representatives are playing the role of ordained second-order observers of their representatives.

It seems such observations cause trouble when they are connected to agents' payoffs.  The senator who votes in contradiction to their beliefs in order to maintain an image is calculating a personal payoff apart from that incurred by their constituents.  If this chance to benefit personally is taken away, we could expect votes more in line with beliefs.


<a id="orgb700ae8"></a>

## Rectifying Values


<a id="org30e8ab1"></a>

### The Money to Reputation Pipeline

We use money as a medium of exchange - to communicate how much we value the things we exchange.  Money's advantage over commodities in this regard is its ability to make the notion of value abstract, so that those with whom we exchange musn't value particular objects the same way we do - they just have to agree to value *something*.  But this is a bug as well as a feature; it is also possible to put a price tag on things that work best when they are not saleable - like reputation, for instance.  This is what happens when a patron of an e-commerce site is browsing through textbooks and decides to buy the one with the most 5 star reviews, unaware of the fact that some authors promote their books by offering special benefits to five-star reviewers.  These reviewers are happy to oblige, since they have nothing to lose if their review eventually contributes to unrealistic expectations.  This is a consequence of money's boundless ability to fulfill any abstract purpose.  


<a id="orgc39b542"></a>

### Plugging the Pipeline

Given that the values of abstractions like *reputation*, *credibility*, and *authenticity* depreciate as these things become more exchangeable for money, and that there is nonetheless obvious market value in their ability to accurately depict the likelihood of fulfilled expectations, can a system that seeks to plug this *money to reputation pipeline* offer consumers and producers the right incentives to become viable in real-world markets?

This is the bold value proposition for Unrival, seen through an economic lens.  It relieves money of its ill-fitted role as credibility accountant by creating a new medium specifically designed for this purpose.  This new medium is a type of ledger (*more precisely a ledger of ledgers*) based on mutual credit, with each entry having additional data related to the *context* in which credit has been exchanged.  Thus, it can complement and work alongside money by addressing some problems associated with information asymmetry.

Notions of credibility can differ significantly.  A particular notion of credibility is represented by an object called a context, which can be thought of as a type of micro-worldview.  

A context includes:

-   **interpretations**: whereby objects are interpreted, i.e. values are assigned to the words that describe these objects
-   **delegates**: agents who vote on updates to a context.  Updates include assigning new delegates and updating intepretations
-   **ledgers**: records of claims and assessments made by agents and the amount of credit staked on them

The challenge we face is one of authenticity.  We'd like to rectify names to address the meta-crisis we find ourselves in - but doing so will require us to calibrate these names based on faithful judgments of what they should refer to.  Should an agent be rewarded for an honest exertion of mental effort to verify that a thing is what it claims to be, or should they be rewarded for predicting the conclusions others will come to, perhaps erroneously?  If we'd like to find a successful strategy for rectifying names, then we'd prefer the former.


<a id="orge7378ac"></a>

# Implementation


<a id="org965d7bb"></a>

## Code vs Data

Being a protocol, Unrival doesn't prescribe ways of implementing the dynamics we've described.


<a id="org16be72b"></a>

## Objects


<a id="orgd9277e9"></a>

### Simple Objects

-   Name

-   Proof

-   Interpretation

-   Blob


<a id="orgf2b2992"></a>

### Complex Objects

-   Agent

    -   Delegates
    
    -   Superdelegates

-   Ledger

-   Claim

-   Context


<a id="orgfbf1be6"></a>

## Architecture


<a id="org1e68a79"></a>

### Server


<a id="org45b086b"></a>

### Client


<a id="orgbaa6ff8"></a>

### Network


<a id="org7cd96e2"></a>

# Application


<a id="orgb44b28a"></a>

## Rating Systems


<a id="orga958bb1"></a>

## Decentralized Sensemaking


<a id="org896f0b5"></a>

## Coordination Problems


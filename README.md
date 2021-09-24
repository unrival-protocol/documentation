
# Table of Contents

-   [Abstract](#orgcdf47f9)
-   [Overview](#org4006e73)
    -   [Rectifying Names](#orge4dab81)
    -   [Rectifying Observations](#org7d16240)
        -   [First Order Observations](#org21a7be1)
        -   [Second Order Observations](#orgd6fc978)
    -   [Rectifying Values](#org3b45504)
        -   [The Money to Reputation Pipeline](#org90b9eb5)
        -   [Plugging the Pipeline](#org8cab881)



<a id="orgcdf47f9"></a>

# Abstract

Unrival is a protocol for tracking the credibility of objects within a network.  Credibility is not defined by a central authority, but rather by objects on their own terms.  Users of this protocol attach claims to objects they interact with in order to let their peers know what can be expected of such interactions.  These peers are then able to assess these claims based on whether outcomes match the expectations they engender.  Over time, the public record of claims and corresponding assessments creates *skin in the game* for participants, whose good faith participation in the network is thus incentivized.


<a id="org4006e73"></a>

# Overview


<a id="orge4dab81"></a>

## Rectifying Names

Roughly 2500 years ago, Confucius was asked what he would do if he were governor.  He would *rectify names*, he said, *to make words correspond with reality*.  Unrival can be seen as a technological strategy for accomplishing this.  

In the present, what we call *news* comes with a fixed set of associations, or implicit claims that make news *news*.  Whatever is deserving of the title should be relevant and factual, for starters.  Yet, as we're all aware, these descriptions hardly apply to much of what is commonly called news.  To rectify the name *news* would mean creating a mechanism whereby things justifiably bearing this name would tend to be reach readers over content exploiting weaknesses in human cognitive architecture for profit.

Creating such a mechanism, such that it relies on the self-interest of individuals and not on starry-eyed ideology to take flight, is the focus of the next sections.


<a id="org7d16240"></a>

## Rectifying Observations

The German sociologist Niklaus Luhmann distinguished between *First Order Observations*, whereby observers' assessments represent their personal reactions, and *Second Order Observations*, whereby observers' assessments are based on their projections of other observers' reactions.  A similar phenomenon was illustrated with an analogy to a beauty pageant by John Maynard Keynes in his *General Theory of Employment, Interest and Money*:

> It is not a case of choosing those [faces] that, to the best of one's judgment, are really the prettiest, nor even those that average opinion genuinely thinks the prettiest. We have reached the third degree where we devote our intelligences to anticipating what average opinion expects the average opinion to be. And there are some, I believe, who practice the fourth, fifth and higher degrees.

One key difference between our world and that of Confucius is the dominant role second order observation plays in informing judgment.  To live in the digital age is to be immersed in the reactions of others.  We've gone from laugh tracks in 20th century sitcoms (*can I laugh now?*) to explicitly labeled *reaction videos* trending on Youtube.  The concept of watching someone watch a video meant to be watched by oneself would be puzzling indeed without an understanding of the growing prevalence of second order observation.

What implications does this have for our project to rectify names?  Since we are describing a decentralized means of credibility accounting, we are dependent on the judgments of agents for pointing out naming (claim) discrepancies.  There are no authoritative standards for determining proper naming - instead, this is determined by the amount of corroboration agents' assessments receive.  In light of what we know about second-order observations, this may present a problem: it is theoretically possible for insincere opinions to be rewarded, if agents have reason to believe they will be corroborated.  This means we must find ways to encourage agents to engage in first order observation in order to maximize the effectiveness of our bottom-up method for rectifying names (i.e. consistently accounting for credibility).  We do so with the knowledge that basically all observations in our digital environments will be second-order; the challenge, then, is to extract *First Order Information* from Second Order Observations.  We will consider ways to achieve this below.


<a id="org21a7be1"></a>

### First Order Observations

-   By Decision Theory

    In his 1969 book *Convention*, philosopher David Lewis pointed out that agents told to go to random locations on a map will not choose locations randomly.  Some locations &#x2013; such as bridges &#x2013; will have inherent value that agents are likely to agree on, and be more likely to go to.  By extension, it is not the case that if you offer an agent $100, *should they happen to choose the same location as another agent on a map of N x N squares*, then their chances of success are 1 / N<sup>2</sup>.  (Equivalently: the expected value of this offer is > $100/N<sup>2</sup>).
    
    A similar argument can be made to show that Unrival agents will stake their credibility on (i.e. assess) claims faithfully as a consequence of self interest.  There is one way to be right about a claim, but many ways to be wrong.  The one way of being right, in line with a true, first order observation, acts like a beacon on a map for self-interested agents to convene upon and profit.

-   By Selective Anonymity

    When votes are made public (as in the case of congressional votes, for example), then voters are made more accountable for their votes.  But there is also a tradeoff: second-order observation &#x2013; voters considering how their votes will be perceived &#x2013; may cause voters to vote against their beliefs.  
    
    Private votes are also problematic, as they 
    
    Unrival's strategy is to internalize the external benefits (e.g. political legitimacy, campaign donations, etc.) that voters gain by voting in line with their public personas.  Ultimately, these things have a monetary value, and this value can also be derived from the value created for those affected by the vote (e.g. constituents).  
    
    Our protocol includes measures to prevent this, but we would also argue that it is unlikely to threaten the integrity of the system.    


<a id="orgd6fc978"></a>

### Second Order Observations

What role should second-order observations play in decentralized credibility accounting?  We may have created a feedback mechanism for correcting the giving of improper names, but we haven't yet addressed .  Agents

Not only are claims subject to assessment, but assessments are as well.  For example, if an agent leaves an unfair assessment for a certain product &#x2013; perhaps with an attached message indicating that this assessment is politically motivated &#x2013; then another agent is behooved to evaluate it as such, since their counter-assessment is more likely to be corroborated than the original assessment.  The justification for the counter-assessment would not be the political motivation of the original assessment, but rather its failure to faithfully assess the product *on its own terms* - i.e. according to what the creator or proponents of the object claim about it.      


<a id="org3b45504"></a>

## Rectifying Values


<a id="org90b9eb5"></a>

### The Money to Reputation Pipeline

We use money as a medium of exchange - to communicate how much we value the things we exchange.  Money's advantage over commodities in this regard is its ability to make the notion of value abstract, so that those with whom we exchange musn't value particular objects the same way we do - they just have to agree to value *something*.  But this is a bug as well as a feature; it is also possible to put a price tag on things that work best when they are not saleable - like reputation, for instance.  This is what happens when a patron of an e-commerce site is browsing through textbooks and decides to buy the one with the most 5 star reviews, unaware of the fact that some authors promote their books by offering special benefits to five-star reviewers.  These reviewers are happy to oblige, since they have nothing to lose if their review eventually contributes to unrealistic expectations.  This is a consequence of money's boundless ability to fulfill any abstract purpose.  


<a id="org8cab881"></a>

### Plugging the Pipeline

Given that the values of abstractions like *reputation*, *credibility*, and *authenticity* depreciate as these things become more exchangeable for money, and that there is nonetheless obvious market value in their ability to accurately depict the likelihood of fulfilled expectations, can a system that seeks to plug this *money to reputation pipeline* offer consumers and producers the right incentives to become viable in real-world markets?

This is the bold value proposition for Unrival, seen through an economic lens.  It relieves money of its ill-fitted role as credibility accountant by creating a new medium specifically designed for this purpose.  This new medium is a type of ledger (*more precisely a ledger of ledgers*) based on mutual credit, with each entry having additional data related to the *context* in which credit has been exchanged.  Thus, it can complement and work alongside money by addressing some problems associated with information asymmetry.  

To illustrate, consider a news article posted on the web.  News is supposed to be factual, relevant, and balanced, but these claims are mere implicit ideals; there's no way to hold a publication's feet to the fire when it misses the mark (and indeed, for many publications, this is a feature and not a bug).  When these ideals are made explicit via claims, however, accountability is possible.  Claims attached to objects in an Unrival network represent credibility that's been staked by stakeholders.  This is a signal to consuming agents that an object's quality has been vouched for.  In this way, the criteria for promoting content are transparent and can serve attract consumption by overtly aligning with the interests of the consumers, rather than through exploitation.

Notions of credibility can differ significantly.  A particular notion of credibility is represented by an object called a context, which can be thought of as a type of micro-worldview.  

A context includes:

-   **interpretations**: whereby objects are interpreted, i.e. values are assigned to the words that describe these objects
-   **delegates**: agents who vote on updates to a context.  Updates include assigning new delegates and updating intepretations
-   **ledgers**: records of claims and assessments made by agents and the amount of credit staked on them

The challenge we face is one of authenticity.  We'd like to rectify names to address the meta-crisis we find ourselves in - but doing so will require us to calibrate these names based on faithful judgments of what they should refer to.  Should an agent be rewarded for an honest exertion of mental effort to verify that a thing is what it claims to be, or should they be rewarded for predicting the conclusions others will come to, perhaps erroneously?  If we'd like to find a successful strategy for rectifying names, then we'd prefer the former.



# Table of Contents

-   [Introduction](#org7916692)



<a id="org7916692"></a>

# Introduction

Unrival is a protocol for tracking the credibility of objects within a network, as defined by these objects on their own terms.  There is no top-down notion of credibility; instead, agents attach claims to objects to let other agents know what can be expected of them.  These claims are then assessed based on whether outcomes match expectations (which correlate strongly with claims).  Over time, the public record of claims and corresponding assessments creates a skin in the game mechanism for agents, whose good faith participation in the network is thus incentivized.

To illustrate, consider a news article posted on the web.  News is supposed to be factual, relevant, and balanced, but these claims are mere implicit ideals; there's no way to hold a publication's feet to the fire when it misses the mark (and indeed, for many publications, this is a feature and not a bug).  When these ideals are made explicit via claims, however, accountability is possible.  Claims attached to objects in an Unrival network represent credibility that's been staked by stakeholders.  This is a signal to consuming agents that an object's quality is vouched for.  This allows consumers to find news based on 

Not only are claims subject to assessment, but assessments are as well.  For example, if an agent leaves an unfair assessment for a certain product &#x2013; perhaps with an attached message indicating that this assessment is politically motivated &#x2013; then another agent is behooved to evaluate it as such, since their counter-assessment is more likely to be corroborated than the original assessment.  The justification for the counter-assessment would not be the political motivation of the original assessment, but rather its failure to faithfully assess the product *on its own terms* - i.e. according to what the creator or proponents of the object claim about it.  

Notions of credibility can differ significantly.  A particular notion of credibility is represented by an object called a context, which can be thought of as a type of micro-worldview.  

A context includes:

-   **interpretations**: whereby objects are interpreted, i.e. values are assigned to the words that describe these objects
-   **delegates**: agents who vote on updates to a context.  Updates include assigning new delegates and updating intepretations
-   **ledgers**: records of claims and assessments made by agents and the amount of credit staked on them


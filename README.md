## Narcissistic K-attribute Stable Matching

This new application of the Nearest Neighbors Chain (NNC) algorithm deals with a variant of the StableMatching problem, in more restricted settings, that is based on 3 models:
- the k-attribute model
- the Narcissistic Stable Matching, and
- the Symmetric Stable Matching

The *k-attribute  model* is  motivated  by  on-line  dating  sites  that  ask  many questions to compile extensive phychological profiles for each person.  Some of these questions attempt to value a person in terms of some k characteristics,such as athleticism, intelligence, salary etc.  Accordingly, the k-attribute model is defined by associating the men with points in R^k.  Each woman’s ranking of the men is defined by a linear function of these attributes, where each woman can have different weights for each attributes, and her preference list is deter-mined by projecting the men’s points onto some line.  Men’s preferences are defined analogously.  The combination of attribute values and weights implicitly represents the entire preference matrix, on which the NNC will be applied. Solving  the  Stable  Matching  problem  has  many  applications,  such  as  pairing up students to accomplish a homework project or users in a P2P file sharing network, assigning co-workers to two-person offices, partitioning players in two-player games or even finding receiver-donor pairs for organ transplants.  In such situations, the students, the people, or the players, which we jointly referto as agents, typically have certain structually restricted preferences on which other agents might be their best partners.  For instance, when assigning room-mates, each agent may have an ideal room temperature and ay prefer to be with another agent with the same penchant.  Deriving from a simple phychological model,  it  seems  natural  to  assume  that  each  agent  is *narcissistic*,  meaning that he/she is his/her own ideal and, thus, most preferred alternative in a pair matching.  We note that although in our Stable Matching problem, an agent cannot be matched to itself, it may still make sense to include an agent x in its preference list, for example when x represents someone which is very close to its ideal.

The *Symmetric Stable Matching*, states that the preferences of the agents
in both pairing sets must obey a certain symmetry. To put it another way,
each agent gives a unique score to each agent from the other set, and ranks
them in increasing order of these scores. Therefore, a set of scores such as
(a ← 7, b ← 2, c ← 10) corresponds to the list of preferences (b, a, c). The preferences are symmetric if the score of x for y equals the score of y to x. So in our
case, a Stable Matching problem is symmetric if the preferences are symmetric.
If the preferences are symmetric, a mutual closest pair always exists. To
prove that, let’s consider s and x be the man and the woman whose score is
the global minimum, that is, no other woman and man are closer to each other
than s and x. Then, s and x are a mutual closest pair: s is the closest man to
x and x is the closest woman to s.
In this ςορκ, it is considered that each agent weights each attribute according
to its own value in that attribute.

# RB-Cost-DDOS
On-demand provisioning allows services to remain available despite massive denial-of-service (DoS) attacks. Unfortunately, provisioning has a cost, which can be exploited by an adversary in an economic denial-of-sustainability (EDoS) attack, wherein the cost for defending a service is higher than that of attacking.

A natural tool to combat EDoS is resource burning (RB). Here, a client must verifiably consume resources---for example, by solving a computational challenge---before service is rendered. However, prior RB-based defenses with security guarantees do not account for the cost of on-demand provisioning.  

In this paper, we propose two deterministic EDoS defenses that use resource burning while accounting for on-demand provisioning. Our algorithms make use of an estimator that can estimate the number of jobs from honest clients (i.e., good jobs) in any set of contiguous jobs to within a $O(\alpha)$-factor, for some {\it a priori}, unknown value $\alpha$.  We assume an omniscient, Byzantine adversary that expends some a priori unknown B resources to attack.

Our first result is in an idealized zero-latency communication model: an algorithm, LINEAR, that spends $O\left( \alpha^{5/2}\sqrt{B\,(g+1)} + \alpha^3(g+\alpha)\right)$,  where $g$ is the number of good jobs.  We also address a partially synchronous model of communication where at most some unknown number, $M$, of good jobs can arrive during any time period in which a message is sent and received.  Our second result is an algorithm, LINEAR-POWER, for this model that both achieves a cost that is at most a factor $M$ larger and  ensures that the time until a job is serviced increases at most logarithmically with $B$.  For large $B$,  the adversary has asymptotically higher cost than our algorithms, implying that our algorithms have an economic advantage.  

Finally, we give a lower bound for deterministic algorithms that shows our costs are asymptotically tight in many cases.

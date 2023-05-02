# RB-Cost-DDOS
To defend against denial of service attacks, we employ a technique called resource burning5
(RB). RB is the verifiable expenditure of a resource, such as computational power, before receiving6
service from the server. To our knowledge, we present the first algorithms that bound the defender’s7
cost as a function of the attacker’s, and ensure that the defender’s cost grows asymptotically more8
slowly than the attacker’s.9
We model an omniscient, Byzantine adversary attacking the system, and a server with access to10
an estimator that estimates the number of honest client jobs (i.e., good jobs) in any time interval.11
We examine two communication models: an idealized zero-latency model and a partially synchronous12
model. Our algorithms for both models have asymptotically lower costs than the attacker’s, as the13
attacker’s costs grow large. Both algorithms use a simple rule to set required RB thresholds per job.14
They do not require any prior knowledge of the number of jobs, the adversary’s costs, or even the15
estimator’s accuracy. However, these quantities parameterize the algorithms’ costs.16
We also prove a lower bound showing that our algorithms achieve asymptotically tight costs as17
the number of jobs grows unbounded, when the estimator’s accuracy is constant.

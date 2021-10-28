By [Aaron Haobei Song](https://linkedin.com/in/haobeisong).

---

### The Guiding Principles for Governance

1. Alignment of incentives between the governing body and the governed
   
2. Practical efficiency
   
3. Competency
   
4. Self-Improvability

### The Governing Structure

The governing structure proposed in this white paper is a **D**ecentralized **O**rganization (DO) or **D**ecentralized **C**orporation (DC[^1]) which lies between a **DAO (DAC)** and a **boring old organization (corporation)** as described by Vitalik Buterin[^2]. The subtle difference between a DAO and DO is in the word 'autonomous'. A DAO makes decisions for itself while in a DO the humans are the ones making the decisions.[^2] It is worth pointing out that the DO proposed here is a little different that it is the humans and the automation combined that makes the decisions.

The proposed governing structure draws inspiration from political systems and consists of 3 bodies:

1. The **constitution**, which is a an aggregate of fundamental principles of the organization and automated regulations. It might happen in practice that some regulations or principles can not be programmed as automation or the incurred cost is unreasonable, in which case, there can be an additional set of regulations or principles written in human language. The guiding principles are as follows
   
   1.  The constitution are designed to change and evolve through *proposal approval process*.
   
   2.  Constitution is designed to be automated as much as possible with also practicability in consideration.

    *Implementation draft:* The automated constitutional rules are smart contracts on a blockchain and the ones in human language can be stored as a reference on the blockchain to a file on IPFS.

2. **Stakeholders** are people and financial institutions or entities that hold financial stakes in the organization. e.g. individual or institutional investors, restaurant owners who invest in the organization, etc. Stakeholders participate in the following organization events:
   
    1. **Election**. The stakeholders elect the president of the organization at a predetermined interval with voting power / weight proportionate to their stakes. To encourage participation, every stakeholder has the obligation to vote directly or delegate his/her stake to another stakeholder who is willing to delegate, otherwise, the stake will be slashed. (The stakeholder who is willing to delegate can delegate the total of his/her own stake and the stakes delegated to them from other stakeholders to another stakeholder who is open to delegate)
   
    2. **Proposal approval process**. Both stakeholders and governing body can sponsor a proposal which goes through a consensus based decision making process[^3] where it will be debated openly, amended accordingly until a consensus is reached to either approve or reject the proposal. There is no limit to the scope of the proposal being it a budget bill to the executive, amendment to the constitution or even an organization reform.

    The participants of the organization are encouraged to become stakeholders. Indeed, a rational participant would want a stake proportionate to the value gained from the organization as this aligns the incentive of the organization with that of the participant's. In theory, individual participants can invest in the equities of a public traded company and take part in the company's decision making. In practice, however, retail investors can barely make their voice heard due to the inefficient voting process and the lack of transparency in the company's operation even when the retail investors collectively hold the majority of the company's stakes.

    **Experimental** To scale, a delegation mechanism will be in place where each stakeholder can delegate his/her stake to another stakeholder as in an *election*. Only the stakeholders holding enough of the toal of their own and delegated stakes are eligible to participate in the *proposal approval process*. The eligible stakeholders will communicate and perform consensus based decision making in a public channel where stakeholders are free to change their delegation.
    
    **Implementation draft:** The DO issues governance tokens as its native currency and stakeholders are reserved governance tokens proportional to their investments. A stake delegation mechanism will be in place to facilitate scalable and resilient voting and consensus based decision making, where stakeholders can delegate their stakes to other stakeholders or groups representing collective interests, through which to participate in the election and proposal approval process. Cryptographic voting system can be built on a blockchain to provide transparency and public verifiability while ensuring optional anonymity. Holographic consensus voting mechanism is another promising voting mechanism which offers both scalability and resilience.[^4]


3. The **governing body**, which consists of the executive and the court.
   
   1. The **executive** manages the operation of the organization, which in the food delivery business include marketing, customer service, coordination of food ordering and delivery, etc, The **president** of the organization is the head of the executive and has the ultimate power over the executive's decision making including hiring, daily operation, planning, etc.
   
   2. The **court** interprets the constitution when confusion arises, guards the executive and stakeholders against violating the regulations or principles set in the constitution, resolve disputes within the organization.

    The governing body should be incentivized to automate their tasks and ensure the maximum transparency for the benefit of its participants. This objective is guarded by the separation of power and their balancing incentives. There should be no secrets in the governing body unless they are justified by the stakeholders.

    **Implementation draft:** A decentralized food delivery application (a Dapp) built on smart contracts can bring transparency to its participants. Smart contracts can also be used to automate tasks performed by the executive and the court, e.g. [Aragon Court](https://aragon.org/aragon-court) for a court trial.


4. The **founding team** is a temporary constituent of the organization which lays the foundation of the organization structure and bootstraps the business. The founding team has the absolute power over the decision making in the organization and operates similarly to the *executive* in the governing body while superseding the constitution and the court. The founding team will be disbanded when the organization becomes stable and self-sufficient as is set for now at *Phase 3* in the [*Roadmap*](roadmap.md) section.

**Overall implementation draft:** An internal blockchain is preferred whether it runs by itself or on top of another reliable blockchain such as Ethereum due to the cost. Think about all the small transactions between restaurants, drivers and consumers which when executed as plain transactions on Ethereum would incur a disproportionate expenses from the minimum gas fee. More generally, the higher the stakes on a blockchain, the more costly each transaction would become. Therefore, it is desirable to run an internal blockchain for low stake transactions or commit checkpoints infrequently on a high stake blockchain with a condensed message using Merkle proofs. To incentivize participants to hold governance tokens, a risk mitigation protocol is needed to hedge the fluctuations of the token value in fiat price.  

### Another Perspective:

The organization structure proposed here is inspired by political systems or more specifically representative democracy and constitutional republic. Take the U.S. government for example, the *constitution* of an organization is similar to the Constitution combined with legislation of the U.S., the *stakeholders* are citizens, the *executive* in a organization is the executive branch of the US government and the *court* the judicial branch. The only apparent missing piece is the Congress whose power is bestowed on the *stakeholders* and duties performed by the *stakeholders* through the *proposal approval process*. The *proposal approval process* seems to follow the ideology of a representative democracy and the difference lies in the consensus decision making instead of a majority voting, while the *election* is through a majority voting strictly following the ideology of a representative democracy. The rule of thumb is, when it comes to deciding on electing a human, the majority voting is used and when it comes to decision making on things, the consensus based decision making is preferred.

[^1]: Note some literature refers to Decentralized Community as DC, which is not the case here.

[^2]: [DAOs, DACs, DAs and More: An Incomplete Terminology Guide](https://blog.ethereum.org/2014/05/06/daos-dacs-das-and-more-an-incomplete-terminology-guide/)

[^3]: [Consensus-Based Decision-Making Processes](http://www.csh.org/wp-content/uploads/2018/07/38-National-Partner-Recommendation-Consensus-Decision-Making-Process-incl-Modified-Consensus.pdf)

[^4]: [Holographic Consensus](https://medium.com/daostack/holographic-consensus-part-1-116a73ba1e1c)

# Dero-Governance-Standards
This repo is meant to be a central hub for the Dero community to list and iterate upon various on-chain governance models

## Monarchy

### Sole-Proprietorship

#### Description
A sole-proprietorship is a contract with a single all-powerful owner. There is no mechanism to limit his power. If the contract is mutable his power is truly limitless. If immutable then his powers are restricted by the code. He may or may not have the power to choose a successor.

#### Examples
This is currently the norm in Dero. 
- G45 Gumball Contract
- Pieswap's token swap contracts (in practice)

### Optimal Autonomous Organization (OAO)

#### Description
The OAO is an experimental governance model first proposed by Curtis Yarvin here: https://graymirror.substack.com/p/optimal-autonomous-organizations

It is an attempt to manifest everyone's favorite form of government: The Benevolent Dictator. First you write a constitution which outlines the purpose and mission of the OAO, as well as roles, responsibilities, and procedures. Then a board of Trustees are selected/elected to protect this constitution. Finally, the board elects the Chief Executive. His role and responsibility is to guide the operations of the organization in accordance with the constitution. His actions are judged by the board, and it is the responsibility of the board to replace him when necessary. If the Chief Executive is a good fit for the organization, and runs things well, board involvement is minimal. They serve as a back-up system. They do not manage operations, they only avert disaster and otherwise let the Chief Executive do his thing.

#### Roles
- Chief Executive
  - Limited access to funds
  - Veto power for code changes
  - Hires/Fires employees
  - Acts in accordance with constitution
- Trustees
  - Hires/Fires Chief Executive in accordance with constitution
  - Determines Chief Executive's access to funds
  - Votes on contract changes
- Participants (opptional)
  - Votes to express popular will (signal preference)
  - Voting power to elect new board (optional)

#### Examples
- Private Islands
- DerBNB


## Oligarchy

#### Description
An oligarchic DAO has no Chief Executive. Only a board of trustees. Contract changes, and treasury withdrawls are executed by n of m votes where n is the QUORUM and m is the number of Trustees.

#### Roles
- Trustees
  - Votes to change contract
  - Votes to direct funds
  - Votes to hire/fire employees
- Participants (opptional)
  - Votes to express popular will
  - Voting power to elect new board (optional)
  - 
#### Examples
- Pieswap's token swap contracts are oligarchic in design but monarchical (sole-proprietor) in practice as voting is currently 1 of 1

## Democracy

#### Description
A democratic DAO is one with a "large" number of voting tokens with real executive power. For example if treasury withdrawls and contract changes are executed by 8000 of 10000 vote. Or perhaps, each proposal could have a "yes" or "no" vote and a deadline. At the time of deadline if there are more "yes" than "no" execution is allowed. This would also be considered democratic if the number of voting tokens were "large". A true democratic DAO would need a way to enforce 1 man n vote(s). If voting tokens can be freely transferred and are not tied to any type of identity, then a democratic DAO can quickly convert into a plutocratic DAO. 

#### Roles
- Governance Token Holders
  - Votes to execute contract changes
  - Votes to transfer funds
  - Ability to delegate voting power (optional)

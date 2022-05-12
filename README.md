0xd7d4ba7de0119778

Chapter 1 - Day 1 - Quests

  1. A blockchain is an immutable, decentralized, and programmable ledger. It allows transactions to be performed and validated across a distributed network.

  2. A smart contract is a program that acts as a rulebook for what can be exectuted on the blockchain.

  3. A script is a programmed function, a transaction takes place when data is altered on the blockchain. 

Chapter 1 - Day 2 - Quests

  1. safety/security, clarity, approachability, developer experience, resource oriented programming

  2. These pillars seem to prioritize accessibility and ease of use as tantamount only to the security of the language. This allows for the developer-base to create apps with reduced anxiety over vulnerabilities, and allows the users to feel safe in knowing that the dApps they interact with do not have malicious intent. 

Chapter 2 - Day 1 - Quests

https://play.onflow.org/afe788ab-474e-4431-a7d1-2e696bacf78b?type=script&id=bb6afdcd-6cb5-43f0-bd67-42e55dbcbce6&storage=none

Chapter 2 - Day 2 - Quests

  1. A script does not modify the state of the blockchain and therefore cannot run changeGreeting.
  
  2. Denotes which account is responsible for the transaction and therefore pays for the gas.

  3. In the prepare phase you are accessing everything you need in the account(s) participating in the transaction and assigning responsibility for the transaction itself. The execute phase is where you can call functions and actually make state changes to the blockchain.

  4. https://play.onflow.org/1d6679c9-cd7a-4c53-8f70-8a803408cfa9?type=script&id=1bce847c-c545-4c4f-a06e-93432b2be951&storage=none

Chapter 2 - Day 3 - Quests

  1. https://play.onflow.org/8fd99aa1-9199-4785-8330-ead4ada36022?type=script&id=860ebec6-88bc-4895-a274-f13095457351&storage=none

  2. https://play.onflow.org/8fd99aa1-9199-4785-8330-ead4ada36022?type=script&id=b10a7519-d9f7-430e-9c95-cb3bbc8f4ec6&storage=none
  
  3. Force unwrap operator unwraps an optional type by giving the order to abort the program if a variable is nil:
    var example: Int? = nil
    var unwrappedExample: Int? = example1!
    
  The above would abort because it unwraps to nil
  
  4. There are two types, so we need to indicate that the function includes addressess and strings.
  The first line should read: pub fun main() {Address: String} {

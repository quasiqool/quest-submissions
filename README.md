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
  
Chapter 3 - Day 1 - Quests

  1. Resources cannot be copied, lost, or created without specific permission written in the contract. They act as highly secure structs.
  
  2. Creating NFT's or other objects that are to retain their properties under all circumstances EXCEPT the ones indicated specifically in the contract.

  3. create

  4. A resource can only be created in a contract.

  5. String

  6.
    a. There needs to be an @ before the resource name
    b. let myJacob <-
    c. create Jacob()
    d. return <- myJacob
    
 Chapter 3 - Day 2 - Quests
 
  1. https://play.onflow.org/e0ed4d6f-88d0-4c74-bd80-a62b8e33a00e?type=account&id=21e42bfc-8c82-4da1-93bb-d351dc5aa989&storage=none

 Chapter 3 - Day 3 - Quests
 
  1. https://play.onflow.org/94a29cff-78eb-4a2d-b51d-6a09ab18dc24?type=account&id=294229cb-a47d-4ebd-992b-928bad828e4b&storage=none

  2. https://play.onflow.org/94a29cff-78eb-4a2d-b51d-6a09ab18dc24?type=script&id=a3e25e4e-e5bc-48d8-b89c-18f1105cfb45&storage=none

  3. References allow for data to be "attached" to resources without having to move them around multiple times and edit the metadata of the resource container itself. 

Chapter 3 - Day 4 - Quests

  1. It gives a set of requirements for a resource or struct to implement and it allows you to restirict access to data held withing the resource or struct to specific people. 

  2. https://play.onflow.org/26104357-7b10-45fa-90ac-62652bfb43f0?type=account&id=9a8e2a36-0390-463e-83d7-e2f1e1e64a97&storage=none
   
  3. let test: Test{ITest} <- create Test()

Chapter 3 - Day 5 - Quests

  1. AREA 1 - Read: a,b,c,d Write: a,b,c,d Func: publicFunc, contractFunc, privateFunc
     AREA 2 - Read: a,b,c   Write: a       Func: publicFunc, contractFunc
     AREA 3 - Read: a,b,c   Write: a       Func: publicFunc, contractFunc
     AREA 4 - Read: a,b     Write: a       Func: publicFunc  

Chapter 4 - Day 1 - Quests

  1. contract code and storage, including public and private storage.

  2. /storage/ is where resources are actually stored. /public/ looks at storage and can be accessed anywhere by anyone as long as you have the address. /private/ acts like a private API, it can still look at storage but can only be accessed the account and whoever the owner gives permissions to.

  3. .save() allows you to store a resources in an account's storage. 
     .load() takes a resource out of storage.
     .borrow() borrows a reference to the resource. 

  4. You can only save something to an account using AuthAccount which is only allowed in the prepare phase of a transcation. 

  5. Only the account owner can access their storage.

  6. https://play.onflow.org/a97c2af8-005f-494c-9871-0d7f5f207347?type=tx&id=644e751c-8349-4a93-b7a2-c02e1dca6860&storage=none

Chapter 4 - Day 2 - Quests

  1. Take resources in storage and make them publicly avaialbe.

  2. If we link a resource and use an interface on top of it, we are providing the public access to view the resource, but only within the scope of the interface.

  3. https://play.onflow.org/df43a6e9-20ab-4f4c-bf0d-aafb332d3f36?type=tx&id=bf0d5229-7b09-4165-b72a-9098b326973a&storage=none

Chapter 4 - Day 3 - Quests

  1. Allows for the storage of many NFT's in one storage space, and allows NFT's to be deoposited into it by others.

  2. You must remove the resource (and specify the key) from the parent resource.

  3. 
    a. Make the contract only allow accounts with a certain number of NFT's already in them mint an NFT. Only let AuthAccount mint an NFT. 
    b. Add a public interface that allows you to read limited information from the collection. Use borrow to get a reference to the Collection.
    
Chapter 4 - Day 4 - Quests
  
  1. https://play.onflow.org/e70774b4-9e03-46fd-9499-f9ac9c80fcd4?type=account&id=921bf8dd-6d8a-4e86-a3da-6bd28cef02e6&storage=none

Chapter 5 - Day 1 - Quests

  1. A way for the contract to communicate to the public that something took place

  2. https://play.onflow.org/a6c62947-7e8b-4c63-9128-f49f46bd6142?type=account&id=2c3b3a6c-2a24-4bd4-8ade-355c7f762041&storage=none

  3. Link above

  4. numberOne - Yes
     numberTwo - Yes
     numberThree - Yes, 1 

Chapter 5 - Day 2 - Quests

  1. It's a way to verify that NFT's or other resource framwworks are adhering to an agreed upon and safe quality standard.

  2. Nothing beats a good pizza, and it's almost impossible to have a bad pizza. 

  3. pub contract Test: ITest
     pub resource interface ITest.IStuff
     
Chapter 5 - Day 3 - Quests

  1. Says that if what comes prior is of the same type as what follows, then move it as indicated. If not, abort the function.

  2. Gives an authorized reference ,its used similarly to as! but instead of downcasting types it is downcasting references.

  3. https://play.onflow.org/b239c6a4-68b1-4ccc-8822-f7b776323c91?type=account&id=872b9ba7-5482-4346-b424-afa2418779ee&storage=none

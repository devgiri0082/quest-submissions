# quest-submissions

## Chapter 1 Day 1 quests

1.Explain what the Blockchain is in your own words/

- Blockchain is a shared databse for storing information, it is public so anybody can take part in it and see all the information stored in it, it is also decentrilized so no one person controls the blockchain and it is open for anyone to join and leave at anytime.

2.Explain what a Smart Contract is.

-  Smart contract are programs that are stored on blockchain. Smart contracts can be called by an account to perform predetermined action like making a transaction or storing a data on the blockchain. Smart contract are very fast, efficient and accurate so they are very useful but we have to use it with caution since they can be hard to get right and possibly malicious if the developer intented it to be.


3. Explain the difference between a script and a transaction.

        Script                                                                                Transaction
        
        1) Sript are used to view data on the blockchain        |                1) Transaction are used to change data on the blockcain
        2) They are free                                        |                2) They are not free
        3) It can not change data on the blockchain             |                 3) It can change data on the blockchain
        
        
<hr/>

## Chapter 1 day 2 quests

1. What are the 5 Cadence Programming Language Pillars?

- Four pillars of Cadence programming language are:
        1. Safety & security
        2. Clarity
        3. Approachability
        4. Developer Experience
        5. Resource Oriented Programming
  
2. In your opinion, even without knowing anything about the Blockchain or coding, why could the 5 Pillars be useful (you don't have to answer this for #5)?

- Safety & Security
       <br/> Safety and Security can help programmer to write code without worrying about different gotchas and vulnerability.
        
- Clarity
       <br/> Cliarity helps increase the readability of the code so everyone can easily understand how the code is working.
        
- Apporachability
       <br/> If it is approachable then beginner developer can easily jump on the band wagon and start developing their DAPP.

- Developer Experience
        <br/>I mean no body wants to filp their finger to the code everytime something goes wrong.

<hr/>

## Chapter 2 day 1 quests

1. Deploy a contract to account 0x03 called "JacobTucker". Inside that contract, declare a constant variable  named is, and make it have type String. Initialize it to "the best" when your contract gets deployed.

<img src='./Images/JacobTucker Contract.png'/>

2. Check that your variable is actually equals "the best" by executing a script to read that variable. Include a screenshot of the output.

<img src='./Images/JacobTucker Execution.png'/>

<hr/>

## Chapter 2 day 2 quests

u1. Explain why we wouldn't call `changeGreeting` in a `script`.

- `changeGreeting` function changes the value of greeting but we can only use `script` to fetch the value from blockchain not change it so we would not call `changeGreeting` in a `script`.

2. What does the `AuthAccount` mean in the prepare phase of the transaction?
  
- `AuthAccount` simply account of the authenticated user or account of the user who is signing the transaction

3. What is the difference between the `prepare` phase and the `execute` phase in the transaction?

- `prepare` can change access the information/data from the `AuthAccount` while `execute` can call functions

4. This is the hardest quest so far, so if it takes you some time, do not worry! I can help you in the Discord if you have questions.

- Wrapping the head around `prepare` and `execute` and wrapping the concept of account storing it's own data was pretty difficult to me.

- Add two new things inside your contract:
    - A variable named `myNumber` that has type `Int` (set it to 0 when the contract is deployed)
    - A function named `updateMyNumber` that takes in a new number named `newNumber` as a parameter that has type `Int` and updates `myNumber` to be `newNumber`

<img src ='/Images/myNumber.png'/>

- Add a script that reads `myNumber` from the contract
  
  <img src='/Images/myNumberScript.png'/>

- Add a transaction that takes in a parameter named `myNewNumber` and passes it into the `updateMyNumber` function. Verify that your number changed by running the script again.

<img src='./Images/myNumberTransaction.png'/>
<img src='./Images/myNumberScript2.png'>

<hr/>

## Chapter 2 day 3 quests

1. In a script, initialize an array (that has length == 3) of your favourite people, represented as Strings, and log it.
   
<img src ="./Images/Array3.png"/>

2. Explain what the force unwrap operator ! does, with an example different from the one I showed you (you can just change the type).

<img src="./Images/forceUnwrapOperator.png"/>

3. Explain what the force unwrap operator `!` does, with an example different from the one I showed you (you can just change the type).

<img src="./Images/forceUnwrapOperator.png"/>

1. Using this picture below, explain...
    - What the error message means
    - Why we're getting this error
    - How to fix it

<img src="./Images/wrongcode.png"/>

   - Error message means the function was expecting a `String` as a return type but got string? 'String or nil'
    - We are getting this error because the return type does not match expected return type which is `String` does not match the actual return value type which is `String?`
    - We can fix it in two way either by using the `force unwrap operator` or by setting the expected return type of the function as optional string `String?`
1. An account contains:
    * Smart Contract, multiple contracts can be deployed and stored in an account
    * Data, All the data is stored in an account eg: NFT



2. The following are the key difference between `/storage`,`/public` & `/private`.
   * `/storage/` - Only the account owner can access from the `/storage`. All the data lives here.
   * `/public/`  - The information here is accessible to everybody.
   * `/private/` - Only available to the account owner and the people that the account owner gives access to.

3. `.save()` is used to saving the data into the `/storage/`path (account storage).
   `.load()` is used to take the data out from the `/storage/` path (account storage).
   `.borrow()` is used to look the data in the `/storage/` we get the refernce to resource in the account storage here.
   
4. I need to approve the transaction and sign it after that the transaction takes in my `AuthAccount` and you can access the data in your account including saving in it.
   That is there for better security.?

5. 

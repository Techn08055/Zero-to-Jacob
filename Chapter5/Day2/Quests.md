1.  * Standards sets a unified way to create contracts that perform similar tasks. 
    * Following a similar standard ensures a working contract if the standards are met.
    
2.  Porotta & Beef 🤤

3.  The contract interface:

```
pub contract interface ITest {
  pub var number: Int
  
  pub fun updateNumber(newNumber: Int) {
    pre {
      newNumber >= 0: "We don't like negative numbers for some reason. We're mean."
    }
    post {
      self.number == newNumber: "Didn't update the number to be the new number."
    }
  }

  pub resource interface IStuff {
    pub var favouriteActivity: String
  }

  pub resource Stuff : IStuff {
    pub var favouriteActivity: String
  }
}
```

The implementing contract:

```
pub contract Test:ITest {
  pub var number: Int
  
  pub fun updateNumber(newNumber: Int) {
    self.number = 5
  }

  pub resource Stuff:ITest.IStuff {
    pub var favouriteActivity: String

    init() {
      self.favouriteActivity = "Playing League of Legends."
    }
  }

  init() {
    self.number = 0
  }
}

```

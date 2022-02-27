1. * `struct`s can be copied and over written                                   ---v/s---  `resource`s cannot be copied or over written
   * `struct`s can be created whenever you want                                 ---v/s---  `resource`s cannot be created whenever you want. It can only be created inside smart contract
   * `struct`s need not be returned/destroyed at the end function using it      ---v/s---  `resource`s must be moved/destroyed at the end function using it

2.  Resources can be used in a situation where you need to make sure that the data is not destroyed like an NFT, May be (Coco Cola's secret formula )

3.  create

4.  Nope, `resource`  cannot be created in a script or transaction

5.  the type of resource is `Jacob` and its public.

6. Corrected code:

```
pub contract Test {

    // Hint: There's nothing wrong here ;)
    pub resource Jacob {
        pub let rocks: Bool
        init() {
            self.rocks = true
        }
    }

    pub fun createJacob(): @Jacob { // there is 1 here
        let myJacob <- create Jacob() // there are 2 here
        return <-myJacob // there is 1 here
    }
}

  ```

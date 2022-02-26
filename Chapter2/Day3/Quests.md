1. 
  ![image](https://user-images.githubusercontent.com/90955843/155830820-6d9e63f7-7b6a-4255-ad7d-ff487132d45f.png)
2. 
  ![image](https://user-images.githubusercontent.com/90955843/155831030-fe8f0642-6dad-4e91-acb9-9f82b9787218.png)
3. The `!` unwraps the `optionals`. If the value optional is not nil when  unwrapped it works fine and get rid of optional type, Otherwiseit panics and aborts the entire program
  ![image](https://user-images.githubusercontent.com/90955843/155831178-743a8b53-a53c-4789-83d3-8cf5f4a56b91.png)
  
4. There is difference between return type function and what the function is returning. This happens since dictionaries returns `optionals` type which can be either 
   `string` or `nil` (here) and function is  expecting return type `string`. We can umwrap the optional returned by the ddictionary using `!`.
    `return thing[0x03]!`

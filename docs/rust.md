**What is the use of '->' and '=>' in Rust programming language ?**

In the Rust programming language, both `->` and `=>` are used, but they serve different purposes and contexts:

1. **`->` (Arrow Operator):**
   - The `->` arrow operator in Rust is used in function and closure signatures to indicate the return type of the function or closure.
   - It is placed between the parameter list and the return type of a function or closure.
   - Example:

   ```rust
   fn add(a: i32, b: i32) -> i32 {
       a + b
   }
   ```
   
   In this example, `-> i32` indicates that the function `add` returns a value of type `i32`.

2. **`=>` (Pattern Separator in Match Expressions):**
   - The `=>` symbol is used in Rust's match expressions to separate patterns from their associated code.
   - In a `match` block, you provide different patterns and the corresponding code to execute when a pattern matches.
   - Example:

   ```rust
   fn main() {
       let number = 42;
       
       match number {
           0 => println!("It's zero"),
           1..=10 => println!("It's between 1 and 10"),
           _ => println!("It's something else"),
       }
   }
   ```
   
   In this example, `0 => println!("It's zero")` uses the `=>` symbol to associate the pattern `0` with the code to print "It's zero".

In summary, `->` is used to indicate the return type of a function or closure, while `=>` is used in match expressions to associate patterns with the code to execute when a pattern matches.

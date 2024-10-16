# Creating a New project Using Cargo
1.Open your terminal
2.Navigate to the directory where you want to create the new project
3.Use the following command to create a new project
```
cargo new project
```
# Navigate To The Project Folder
Move into the newly created directory
```
cd project
```
This opens the new project
```
>code.
```
Cargo alreaady generates a "Hello,World!"program for you in src/main.rs,but you can open the file .the default content will look  like this:
```
fn main() {
println!("Hello,world!");
}
```
# Running The Rust Program
To compile and run the project,use the following command:
```
cargo run
```
you should see the following output in your terminal:
```
Compilling hello_world v0.1.0 (path-to-project/project)
Finished dev [unoptimized + debuginfo] target(s)in 0.46s
Running `target/debug/hello_world`
Hello,world!
```

# Variable In Rust
In rust,variables are declared using the `let` keyword, and by default they are immutable.if you want a variable to be mutable(i.e.,you want to change its value later),
you must explicitly use the `mut`keyword.Here's a breakdown of how variables work in Rust:

### 1.Immutable Variable(Default)
by default,variables in rust are immutable,meaning their value cannot be changed after they are assigned.
```
fn main() {
let mut age=25;
println!("your age is: {}", age );

// This will cause an error because age is immutable
// age = 26;
}
```
### 2. Mutable Variable
To allow a variable to be changed (mutable), use the `mut` keyword;

```
fn main() {
  let mut age = 25;
  println!("Your age is: {}", age};

  age = 26; // Now you can change the value
  println!("Your next age will be {}", age);
}
```
Here `age` is mutable, so you can change its value after it has been assigned.


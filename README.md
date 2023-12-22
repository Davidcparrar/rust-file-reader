[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=665539593)

# Rust Fundamentals Week 2

This is the exercise for Week 2 of the [Rust Fundamentals Course](https://www.coursera.org/learn/rust-fundamentals)

In this lab, you will enhance a file reader application in Rust. 
Use the example code
 for error handling as a starting point for reading a file and printing its contents. You are tasked with extending the application to allow users to specify the file to be read as a command-line argument. The end result will be a GitHub repository containing the complete code for the enhanced file reader application.

Learning Objectives:

1. Understand how to read and process files in Rust using the standard library.

1. Practice error handling techniques, such as matching on different error cases.

1. Learn how to organize code and structure a Rust application.

Steps:

1. Create a new repository in your account for your Rust project. Use the 
Rust template repository
 to quickly generate one for 
your account
.

1. Use the [example code](https://github.com/alfredodeza/rust-fundamentals/blob/main/examples/16-error-handling/error-handling/src/main.rs) as a starting point

1. Add the ability to pass in any file path to avoid hard-coding the path in the program. 
Use the Rust docs
 or this sample code to get an idea on how to get the first argument in the console:

 ```rust
 use std::env;

fn main() {
    let args: Vec<String> = env::args().collect();

    // The first argument is the path that was used to call the program.
    println!("My path is {}.", args[0]);
}
 ```
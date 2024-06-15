# Rust Project

This project serves as a way for me to learn the Rust programming language.  
Throughout this project I am making comprehensive notes so that anyone can pick it up and understand  
what rust is, and can do from a programmers perspective.  

> **_NOTE:_** I am by no means perfect, so if you read a comment that makes zero sense,  
don't hesitate to make a PR to correct me.  
  
Together we can make programming accessible to everyone, even to the engineers that advocate for JS...  

_Jokes_  

What do you call a game console programmed in Rust? A `Playstacean`!

## Table of contents

[TOC]

## Things to note

### .gitignore and why is it important

1. In the [.gitignore]("./.gitignore") it is important to note the following
    1. You can always ignore the `./target` directory as this just contains the built project.
    2. You **can** ignore the `./Cargo.lock` but note the following. [_- Source_](https://stackoverflow.com/questions/43667176/what-files-in-a-cargo-project-should-be-in-my-gitignore)
        - On the one hand, you should always test your library with the latest version of all your dependencies. That's an argument **against** Cargo.lock.
        - On the **other** hand, Cargo.lock gives you the same benefit as in other projects: reproducible builds mean stable CI, easier bisecting, yada yada.
    3. See the [.gitignore](.gitignore) for the comments on what is ignored and why they are ignored.

### Rust's Program Structure

### Rust files and what they mean

> Inside each file I added comments on what they do and how to use them.

|         File Name          |                                                                                           What it does                                                                                            |
| :------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| [Cargo.toml](./Cargo.toml) | TOML is designed to map unambiguously to hash table. </br> The `Cargo.toml` file contains the application's metadata </br> [name, version, dependencies for _packages_ which contains _things_ called `creates` in Rust] </br> This serves as the configuration file for your program/crate. |
| [main.rs](./src/main.rs) | This is your main function/entrypoint of execution in the program.</br> Other code will be called from this function. |

> Date : 2024-06-15

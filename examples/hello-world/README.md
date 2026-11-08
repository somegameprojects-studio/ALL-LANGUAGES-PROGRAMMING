# Hello, World! — Working Examples

These examples show the smallest useful program or document for a selection of languages and technologies in this repository. They are starting points, not a claim that every tool uses a \`print()\` function.

> **Before running:** install the language's official runtime/compiler and check its current documentation. Commands can vary by operating system and toolchain version.

## Programming languages

### Python

\`\`\`python
print("Hello, World!")
\`\`\`
Run: \`python hello.py\`

### JavaScript

\`\`\`javascript
console.log("Hello, World!");
\`\`\`
Run: \`node hello.js\`

### TypeScript

\`\`\`typescript
const message: string = "Hello, World!";
console.log(message);
\`\`\`
Run with a TypeScript runtime such as \`tsx hello.ts\`, or compile with the TypeScript compiler.

### C

\`\`\`c
#include <stdio.h>

int main(void) {
    printf("Hello, World!\\n");
    return 0;
}
\`\`\`
Compile: \`cc hello.c -o hello\` · Run: \`./hello\`

### C++

\`\`\`cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!\\n";
    return 0;
}
\`\`\`
Compile: \`c++ hello.cpp -o hello\` · Run: \`./hello\`

### C#

\`\`\`csharp
Console.WriteLine("Hello, World!");
\`\`\`
Run in a .NET project: \`dotnet run\`

### Java

\`\`\`java
class Hello {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
\`\`\`
Run: \`javac Hello.java && java Hello\`

### Go

\`\`\`go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
\`\`\`
Run: \`go run hello.go\`

### Rust

\`\`\`rust
fn main() {
    println!("Hello, World!");
}
\`\`\`
Run: \`rustc hello.rs && ./hello\`

### PHP

\`\`\`php
<?php
echo "Hello, World!\\n";
\`\`\`
Run: \`php hello.php\`

### Ruby

\`\`\`ruby
puts "Hello, World!"
\`\`\`
Run: \`ruby hello.rb\`

### Lua

\`\`\`lua
print("Hello, World!")
\`\`\`
Run: \`lua hello.lua\`

### Swift

\`\`\`swift
print("Hello, World!")
\`\`\`
Run: \`swift hello.swift\`

### Kotlin

\`\`\`kotlin
fun main() {
    println("Hello, World!")
}
\`\`\`
Run with the Kotlin compiler or a Kotlin project.

### Dart

\`\`\`dart
void main() {
  print('Hello, World!');
}
\`\`\`
Run: \`dart run hello.dart\`

### Bash

\`\`\`bash
#!/usr/bin/env bash
printf '%s\\n' 'Hello, World!'
\`\`\`
Run: \`bash hello.sh\`

### PowerShell

\`\`\`powershell
Write-Output "Hello, World!"
\`\`\`
Run: \`pwsh -File hello.ps1\` (or \`powershell -File hello.ps1\` on Windows PowerShell).

### Perl

\`\`\`perl
use strict;
use warnings;

print "Hello, World!\\n";
\`\`\`
Run: \`perl hello.pl\`

### R

\`\`\`r
print("Hello, World!")
\`\`\`
Run: \`Rscript hello.R\`

### Julia

\`\`\`julia
println("Hello, World!")
\`\`\`
Run: \`julia hello.jl\`

### Scala

\`\`\`scala
object Hello {
  def main(args: Array[String]): Unit =
    println("Hello, World!")
}
\`\`\`
Run with the Scala CLI: \`scala Hello.scala\`

### Elixir

\`\`\`elixir
IO.puts("Hello, World!")
\`\`\`
Run: \`elixir hello.exs\`

### Haskell

\`\`\`haskell
main :: IO ()
main = putStrLn "Hello, World!"
\`\`\`
Run with GHC: \`runghc hello.hs\`

### Clojure

\`\`\`clojure
(println "Hello, World!")
\`\`\`
Run with the Clojure CLI: \`clojure -M hello.clj\` (project setup may vary).

### F#

\`\`\`fsharp
printfn "Hello, World!"
\`\`\`
Run as a script: \`dotnet fsi hello.fsx\`

### Objective-C

\`\`\`objective-c
#import <Foundation/Foundation.h>

int main(void) {
    @autoreleasepool {
        NSLog(@"Hello, World!");
    }
    return 0;
}
\`\`\`
Compile on macOS with the Apple toolchain: \`clang hello.m -framework Foundation -o hello\`.

### Assembly (NASM, x86-64 Linux)

\`\`\`asm
section .data
    message db "Hello, World!", 10
    length equ $ - message

section .text
    global _start

_start:
    mov eax, 1
    mov edi, 1
    mov rsi, message
    mov edx, length
    syscall

    mov eax, 60
    xor edi, edi
    syscall
\`\`\`
This is a Linux x86-64 system-call example; assemble/link commands depend on the installed NASM and linker.

## Markup, query, and configuration examples

These formats are not all general-purpose programming languages. They describe documents, data, queries, or build instructions.

### HTML

\`\`\`html
<!doctype html>
<html lang="en">
  <head><meta charset="utf-8"><title>Hello</title></head>
  <body><h1>Hello, World!</h1></body>
</html>
\`\`\`
Open the file in a web browser.

### CSS

\`\`\`css
body {
  font-family: system-ui, sans-serif;
}

h1::before {
  content: "Hello, ";
}
\`\`\`
CSS styles HTML; it does not run as a standalone print program.

### SQL

\`\`\`sql
SELECT 'Hello, World!' AS message;
\`\`\`
Run in a compatible SQL database or SQL console.

### GraphQL

\`\`\`graphql
query Greeting {
  greeting
}
\`\`\`
This is a query document; it needs a GraphQL server that exposes a \`greeting\` field.

### JSON

\`\`\`json
{
  "message": "Hello, World!"
}
\`\`\`
JSON is a data format, not executable code.

### YAML

\`\`\`yaml
message: Hello, World!
\`\`\`
YAML is a data-serialization format, not executable code.

### XML

\`\`\`xml
<?xml version="1.0" encoding="UTF-8"?>
<message>Hello, World!</message>
\`\`\`
XML describes structured data; an application must read or display it.

### Makefile

\`\`\`makefile
.PHONY: hello
hello:
\t@echo "Hello, World!"
\`\`\`
Run: \`make hello\`

### Dockerfile

\`\`\`dockerfile
FROM alpine:latest
CMD ["sh", "-c", "echo 'Hello, World!'"]
\`\`\`
Build and run using Docker: \`docker build -t hello-example . && docker run --rm hello-example\`.

### Solidity

\`\`\`solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Greeting {
    function message() external pure returns (string memory) {
        return "Hello, World!";
    }
}
\`\`\`
This is a smart contract example. Compile and test it with a Solidity development tool; deploying requires a compatible blockchain environment.

## Next steps

For each language, expand the matching \`languages/<language>/\` guide with:
1. Installation and version information.
2. Variables, data types, operators, and control flow.
3. Functions and reusable code.
4. Input/output and error handling.
5. Data structures, modules, and packages.
6. A small practical project.

Contributions should be tested and should link to the language's official documentation.

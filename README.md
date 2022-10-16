# jvm-interop
A Collection of Modules to create Tasks for JVM Java, Kotlin, GraalVM Interop 

## Why?
GraalVM is a Collection of Tools to Build Binarys via a LLVM Backend and Frontend from Polyglot Input Sources. It offers the Truffle API as corre connection part between the language to translate. the Truffle API uses the JVM-CI to get Compiler Feedback it is Compare able to LLVM 

the JVM executes so called JavaByte code which is again Compareable to C ByteCode. the JavaByte Code can easy be Translated to C ByteCode that is exactly what the LLVM Backend of GraalVM does they call that Native-Image.

There exists Millions of lines of Code written exclusiv in Java and at present while it is no core relevant code there exist some company use cases where they want to integrate existing GraalVM code for reuse with Stealify. 

## Integration Points
- Running from inside the JVM via GraalJS we can use any System Interface to Exchange Messages using vertx as scheduler. 
- When StealifyVM so a stealify-component creates GraalVM Tasks we can directly interface via the Tasks Interface. Stealify Streams to vertx.

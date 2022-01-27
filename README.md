Where Rust Shines


Rust is a statically and strongly typed systems programming language. statically means that all types are known at compile-time, strongly means that these types are designed to make it harder to write incorrect programs. A successful compilation means you have a much better guarantee of correctness than with a cowboy language like C. systems means generating the best possible machine code with full control of memory use. So the uses are pretty hardcore: operating systems, device drivers and embedded systems that might not even have an operating system. However, it's actually a very pleasant language to write normal application code in as well.

The big difference from C and C++ is that Rust is safe by default; all memory accesses are checked. It is not possible to corrupt memory by accident.

The unifying principles behind Rust are:

strictly enforcing safe borrowing of data
functions, methods and closures to operate on data
tuples, structs and enums to aggregate data
pattern matching to select and destructure data
traits to define behaviour on data


There is a fast-growing ecosystem of available libraries through Cargo but here we will concentrate on the core principles of the language by learning to use the standard library. My advice is to write lots of small programs, so learning to use rustc directly is a core skill. When doing the examples in this tutorial I defined a little script called rrun which does a compilation and runs the result:

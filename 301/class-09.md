
### What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

### What is a pure function and how do we know if something is a pure function?

It returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects

### What are the benefits of a pure function?

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:
Given a parameter A → expect the function to return value B
Given a parameter C → expect the function to return value D

### What is immutability?

Unchanging over time or unable to be changed.


### What is Referential transparency?

pure functions + immutable data = referential transparency

<!--https://v8.dev/features/modules  -->
### What is a module?

JS modules (also known as “ES modules” or “ECMAScript modules”) are a major new feature, or rather a collection of new features. You may have used a userland JavaScript module system in the past. Maybe you used CommonJS like in Node.js, or maybe AMD, or maybe something else. All of these module systems have one thing in common: they allow you to import and export stuff.

JavaScript now has standardized syntax for exactly that. Within a module, you can use the export keyword to export just about anything. You can export a const, a function, or any other variable binding or declaration. Just prefix the variable statement or declaration with export and you’re all set:
<!-- stackoverflow -->
### What does the word ‘require’ do?

require() is not part of the standard JavaScript API. But in Node.js, it's a built-in function with a special purpose: to load modules.
<!-- https://developer.mozilla.org/ -->

### How do we bring another module into the file the we are working in?

The static import statement is used to import read only live bindings which are exported by another module.

Imported modules are in strict mode whether you declare them as such or not. The import statement cannot be used in embedded scripts unless such script has a type="module". Bindings imported are called live bindings because they are updated by the module that exported the binding.

There is also a function-like dynamic import(), which does not require scripts of type="module".

Backward compatibility can be ensured using attribute nomodule on the script tag.

### What do we have to do to make a module available?

export them



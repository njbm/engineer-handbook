# 🐘 PHP Interview Questions & Answers

### Q1: What is the difference between `==` and `===` in PHP?
- A: `==` compares values only. `===` compares both value and type.

### Q2: What is the use of `isset()` in PHP?
- A: It checks if a variable is set and not null.

### Q3: Explain the difference between `include`, `require`, `include_once`, and `require_once`.
- A: `require` causes a fatal error on failure; `include` causes a warning. `_once` versions prevent multiple inclusions.

### Q4: What are magic methods in PHP?
- A: Methods like `__construct`, `__get`, `__set`, and `__toString` that get called automatically.

### Q5: What is the difference between GET and POST methods?
- A: GET sends data via URL; POST via HTTP body (more secure).

### Q6: What is a session in PHP?
- A: A way to persist data across user requests using `$_SESSION`.

### Q7: What is a cookie in PHP?
- A: Data stored on the client browser using `setcookie()`.

### Q8: How do you handle errors in PHP?
- A: With `try-catch`, `set_error_handler()`, or error reporting settings.

### Q9: What are traits in PHP?
- A: Reusable sets of methods for classes (like mixins).

### Q10: Difference between abstract class and interface?
- A: Abstract classes can have method bodies, interfaces cannot (until PHP 8 default methods).

### Q11: What is type hinting?
- A: Restricting input/output types of functions or methods.

### Q12: What are namespaces?
- A: Prevent class/function name conflicts in larger codebases.

### Q13: How is OOP implemented in PHP?
- A: Using classes, objects, inheritance, polymorphism, and encapsulation.

### Q14: What are PSR standards?
- A: PHP-FIG recommendations for coding standards (e.g., PSR-1, PSR-4, PSR-12).

### Q15: What is Composer?
- A: Dependency manager for PHP packages.

### Q16: What is autoloading?
- A: Dynamically loading class files using PSR-4 or spl_autoload_register.

### Q17: What is late static binding?
- A: Refers to the class where a static method is called, not defined.

### Q18: How to connect to MySQL using PDO?
- A: `$pdo = new PDO("mysql:host=localhost;dbname=db", "user", "pass");`

### Q19: What are prepared statements?
- A: Safer SQL queries using placeholders (prevent SQL injection).

### Q20: Difference between public, private, protected?
- A: Access level — public (everywhere), protected (in class and subclasses), private (only in class).

### Q21: What is the difference between static and non-static methods?
- A: Static methods belong to the class, not objects. Called via ClassName::method().

### Q22: How do you define and use constants in PHP?
- A: Using `define('NAME', 'value');` or `const NAME = 'value';`.

### Q23: What is the SPL in PHP?
- A: Standard PHP Library — built-in interfaces, iterators, exceptions, etc.

### Q24: What is reflection in PHP?
- A: Allows inspection of classes, interfaces, methods, and properties at runtime.

### Q25: What are anonymous functions?
- A: Functions with no name. `$greet = function($name) { return "Hi $name"; };`

### Q26: What is a closure?
- A: A function that uses variables outside its scope with `use()`.

### Q27: Explain the use of generators.
- A: `yield` allows iteration without loading everything into memory.

### Q28: What is garbage collection?
- A: PHP’s memory management that cleans up unused objects.

### Q29: What are common design patterns in PHP?
- A: Singleton, Factory, Strategy, Repository, Observer, etc.

### Q30: How to improve performance of PHP applications?
- A: Caching, opcode cache (OPcache), indexing, pagination, profiling.

### Q31: What is the difference between `echo`, `print`, and `printf`?
- A: `echo` is faster; `print` returns 1 (used in expressions); `printf` formats output.

### Q32: How to prevent SQL injection?
- A: Use prepared statements via PDO or mysqli.

### Q33: How does PHP manage memory?
- A: Through reference counting and garbage collection.

### Q34: Common security vulnerabilities in PHP?
- A: XSS, CSRF, SQL injection, file inclusion. Use validation, escaping, tokens.

### Q35: What is the difference between `unset()` and assigning `null`?
- A: `unset()` deletes the variable; assigning `null` keeps it but sets it empty.

### Q36: What is output buffering?
- A: Temporarily stores output using `ob_start()` before sending it to the browser.

### Q37: What are global variables?
- A: Declared outside functions and accessed via `global $var` or `$GLOBALS`.

### Q38: How do you validate data?
- A: Using `filter_var()`, regex, or validation libraries.

### Q39: Types of arrays in PHP?
- A: Indexed, associative, and multidimensional.

### Q40: Common array functions?
- A: `array_map`, `array_filter`, `array_merge`, `array_reduce`, `array_diff`.

### Q41: How to create custom exceptions?
- A: Extend the `Exception` class.

### Q42: Explain the MVC pattern.
- A: Model (data), View (UI), Controller (logic).

### Q43: How do you handle file uploads?
- A: Use `$_FILES` and move the file with `move_uploaded_file()`.

### Q44: What are superglobals?
- A: Built-in variables like `$_POST`, `$_GET`, `$_SESSION`, etc.

### Q45: Use of regular expressions?
- A: Validate/search strings using `preg_match()`, `preg_replace()`.

### Q46: What is object cloning?
- A: Creating a copy of an object with `clone` keyword.

### Q47: What is `__autoload()` vs `spl_autoload_register()`?
- A: `__autoload()` is deprecated; `spl_autoload_register()` is the modern way.

### Q48: Difference between session and cookie?
- A: Session is stored on server; cookie is stored in the browser.

### Q49: How to parse large XML/JSON files?
- A: Use streaming parsers like `XMLReader` or `json_decode` with chunked files.

### Q50: Key improvements in PHP 7/8?
- A: Scalar type hints, return types, null coalescing, union types, JIT, attributes.

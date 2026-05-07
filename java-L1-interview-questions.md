# Java Interview Questions

> Target level: Easy

---

## Core Java

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | What is the difference between a class and an object? Can you give a real-world analogy? | Foundational | Theory |
| 2 | What are the four pillars of OOP? Give a one-sentence example of each in Java. | Foundational | Theory |
| 3 | What is the difference between stack memory and heap memory in Java? Where do local variables and objects live? | Foundational | Theory |
| 4 | What is the difference between a checked and an unchecked exception? Give one example of each you've encountered at work. | Foundational | Theory |
| 5 | Explain what `static` means when applied to a method or a field. What's a common misuse you've seen? | Foundational | Theory |
| 6 | What is autoboxing? Write a small example where it could cause a NullPointerException unexpectedly. | Intermediate | Theory |

---

## Collections

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | What is the difference between ArrayList and LinkedList? When would you prefer one over the other? | Foundational | Theory |
| 2 | What happens if you put a mutable object as a HashMap key and then mutate it? | Intermediate | Theory |
| 3 | What is the difference between HashMap and HashSet? How does HashSet use HashMap internally? | Foundational | Theory |
| 4 | When would you use a TreeMap over a HashMap? What ordering does it provide and at what cost? | Intermediate | Theory |
| 5 | You need to count how many times each word appears in a list of strings. Which collection(s) would you use? | Foundational | Theory |

---

## Lambdas & Streams

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | What is a lambda expression? Rewrite an anonymous Runnable class as a lambda. | Foundational | Theory |
| 2 | What does this stream pipeline do? Walk me through it step by step: `list.stream().filter(s -> s.startsWith("A")).map(String::toUpperCase).collect(Collectors.toList())` | Foundational | Theory |
| 3 | What is the difference between `map()` and `forEach()` in a stream? When would you use each? | Foundational | Theory |
| 4 | What is an Optional? Show how you'd use it to safely get a user's email, defaulting to `"N/A"` if absent. | Intermediate | Theory |
| 5 | Using streams, filter a list of integers to keep only even numbers and return their sum. | Foundational | Coding |

---

## Spring Basics

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | What is dependency injection? Explain it without using technical jargon, as if to a non-developer. | Foundational | Theory |
| 2 | What is the difference between `@Component`, `@Service`, and `@Repository` in Spring? | Foundational | Theory |
| 3 | What does `@Autowired` do? What happens if Spring finds two beans of the same type? | Foundational | Theory |
| 4 | What is the difference between `@GetMapping` and `@PostMapping`? When would you use `@RequestParam` vs `@PathVariable`? | Foundational | Theory |
| 5 | What does `@Transactional` do? Can you give an example of when forgetting it would cause a problem? | Intermediate | Theory |
| 6 | You run a Spring Boot app and get "No qualifying bean of type X". How do you debug it? | Intermediate | Theory |

---

## Coding

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | Write a method that takes a list of integers and returns a new list with duplicates removed, preserving the original order. | Foundational | Coding |
| 2 | Write a method to check if a string is a palindrome (reads the same forwards and backwards), ignoring case and spaces. | Foundational | Coding |
| 3 | Given a list of Student objects with name and grade, write a method that returns the name of the student with the highest grade using streams. | Foundational | Coding |
| 4 | Write a method that counts how many times each character appears in a string and returns a Map. | Foundational | Coding |
| 5 | Write a simple Spring Boot REST endpoint that accepts a name as a query parameter and returns `"Hello, {name}!"`. | Foundational | Coding |
| 6 | Write a method that reverses a string without using `StringBuilder.reverse()` or any built-in reverse utility. | Foundational | Coding |

---

## Spot the Bug

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | This method should print all names but prints nothing — a stream filter with `length() > 10` on short strings. What's wrong? | Foundational | Debug |
| 2 | Why does `emp.getAddress().getCity().getDepartment()` cause a NullPointerException? How would you fix it? | Foundational | Debug |
| 3 | This code compiles but throws a ConcurrentModificationException at runtime — removing an element from a list inside an enhanced for loop. Why? | Intermediate | Debug |
| 4 | Why does a Spring `@Service` that manually instantiates its dependencies with `new` fail to work correctly with Spring? | Intermediate | Debug |
| 5 | What is the output of comparing two `Integer` objects with value `128` using `==` vs `.equals()`? Is there a bug? | Intermediate | Debug |

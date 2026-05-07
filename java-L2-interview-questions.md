# Java Interview Questions

> Target level: Need a good understanding

---

## Core Java

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | Explain the difference between `==` and `.equals()` in Java. When would you override `equals()` and what contract must you maintain? | Intermediate | Theory |
| 2 | What is the Java Memory Model (JMM)? How do the heap, stack, metaspace, and garbage collector interact? | Advanced | Theory |
| 3 | Describe the difference between checked and unchecked exceptions. Give an example of when you'd create a custom RuntimeException. | Intermediate | Theory |
| 4 | What is the significance of the `final` keyword when applied to a variable, method, and class? | Foundational | Theory |
| 5 | Explain String immutability and the String Pool. What are the implications for performance and security? | Intermediate | Theory |
| 6 | What is the difference between abstract classes and interfaces post-Java 8? When would you choose one over the other? | Intermediate | Theory |
| 7 | How does Java achieve polymorphism? Explain static dispatch vs dynamic dispatch with an example. | Advanced | Theory |

---

## Collections & Generics

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | Compare HashMap, LinkedHashMap, TreeMap, and ConcurrentHashMap. When would you use each? | Intermediate | Theory |
| 2 | What happens when two keys have the same hashCode in a HashMap? Walk me through the internal mechanics. | Advanced | Theory |
| 3 | Explain the difference between fail-fast and fail-safe iterators. Give an example of each. | Intermediate | Theory |
| 4 | How do bounded wildcards (`? extends T` and `? super T`) work in generics? Explain the PECS principle. | Advanced | Theory |
| 5 | When would you use a PriorityQueue vs a TreeSet? What are their internal data structures? | Intermediate | Theory |

---

## Lambdas & Streams

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | What is a functional interface? Name four built-in functional interfaces from `java.util.function` and explain when you'd use each. | Foundational | Theory |
| 2 | What is the difference between a lambda expression and an anonymous inner class? When does each capture `this`? | Intermediate | Theory |
| 3 | Explain variable capture in lambda expressions. Why must captured local variables be effectively final? | Intermediate | Theory |
| 4 | Compare `list.forEach(s -> System.out.println(s))` vs `list.forEach(System.out::println)`. What types of method references exist? | Foundational | Theory |
| 5 | Write a stream pipeline that takes a list of employees, filters those with salary > 80,000, groups them by department, and returns a `Map<String, Long>` of count per department. | Advanced | Theory |
| 6 | What is the difference between `map()` and `flatMap()` in the Stream API? Give a practical use case for each. | Intermediate | Theory |
| 7 | Explain lazy evaluation in streams. What is the difference between intermediate and terminal operations? | Intermediate | Theory |
| 8 | What are the pitfalls of using parallel streams? When should you avoid them? | Advanced | Theory |
| 9 | How would you compose two `Predicate<T>` instances? Show an example using `and()`, `or()`, and `negate()`. | Intermediate | Theory |

---

## Concurrency

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | Explain the difference between synchronized methods, synchronized blocks, and ReentrantLock. What does ReentrantLock offer that synchronized doesn't? | Advanced | Theory |
| 2 | What is the `volatile` keyword in Java? What guarantees does it provide and what does it NOT guarantee? | Intermediate | Theory |
| 3 | Describe the producer-consumer pattern. How would you implement it using BlockingQueue? | Intermediate | Theory |
| 4 | What is a deadlock? Describe four conditions required for deadlock and how you'd prevent it. | Advanced | Theory |
| 5 | Explain the difference between Callable and Runnable. How do Future and CompletableFuture differ? | Intermediate | Theory |

---

## Spring Framework

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | Explain the Spring Bean lifecycle from instantiation to destruction. What are the extension points available at each stage? | Advanced | Theory |
| 2 | What is the difference between `@Component`, `@Service`, `@Repository`, and `@Controller`? Are they functionally equivalent? | Foundational | Theory |
| 3 | Explain how Spring's `@Transactional` works internally. What are the propagation and isolation levels, and what are the common pitfalls? | Advanced | Theory |
| 4 | What is the difference between constructor injection, setter injection, and field injection in Spring? Which is preferred and why? | Intermediate | Theory |
| 5 | How does Spring Boot auto-configuration work? Explain the role of `@EnableAutoConfiguration` and `spring.factories` / `AutoConfiguration.imports`. | Advanced | Theory |
| 6 | Describe how you would secure a Spring Boot REST API using Spring Security. Walk through JWT-based authentication. | Advanced | Theory |
| 7 | What is the difference between Spring Data JPA's `@Query` (JPQL) and native queries? When would you use a Specification or QueryDSL? | Intermediate | Theory |

---

## Practical & Design

| # | Question | Difficulty | Type |
|---|----------|------------|------|
| 1 | You have a REST endpoint that's causing N+1 query problems in production. How do you diagnose and resolve it? | Advanced | Theory |
| 2 | Design a rate limiter for a REST API in Java. What data structures and algorithms would you use? | Advanced | Theory |
| 3 | Explain SOLID principles with a real-world Java/Spring example for each. Which do you find most commonly violated? | Intermediate | Theory |
| 4 | You're asked to migrate a monolith to microservices. What are the key challenges and how would you approach the strangler fig pattern? | Advanced | Theory |
| 5 | How would you write unit tests for a Spring service that calls a repository and an external HTTP API? What mocking strategy would you use? | Intermediate | Theory |

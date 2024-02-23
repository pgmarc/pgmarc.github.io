---
layout: default
title: Java
parent: Programming knowledge
new_order: 1
---

{: .label}
Code



# Data Structures

## HashMap

Use a this kind of data structure when you **dont mind** insertion order.

{: .warning-title}
> Remember
>
> Using a `HashMap` does not guarantee map insertion order.

## LinkedHashMap

**Preserves** map **insertion** order of items

```java
Map<String,Integer> ratings = new LinkedHashMap<>();
ratings.put("Maths", 5);
ratings.put("Chemistry", 7);
ratings.put("Art", 4);

// First: (Maths,5) ---->  Second: (Chemistry,7) ----> Third: (Art,4)
```

# I/O

{: .warning-title}
> Remember
>
> `InputStreams` needs to be closed to release resources.
>
> Not closing the resource could lead to:
> - Data corruption
> - Resource leakage
> - File locking

{: .important-title}
> Examples
> 
>- Manual closing of stream in [SnakeYaml][SnakeYaml Test Case].
>- Baeldung closing IO [Streams](https://www.baeldung.com/java-io-streams-closing)


# Further investigation

Java IO stream closing in StackOverflow [question][java-stream-closed]


---

[java-stream-closed]: https://stackoverflow.com/questions/22900477/java-io-exception-stream-closed)
[SnakeYaml Test Case]: https://bitbucket.org/snakeyaml/snakeyaml/src/master/src/test/java/examples/LoadExampleTest.java
---
layout: default
title: Yaml
parent: Programming knowledge
new_order: 2
---

# Integers

Integers may be written as:
- With a leading 0x to represent hexadecimal (base 16).
- With a leading 0b to represent binary numbers (base 2).
- With a leading 0 (YAML 1.2 is 0b) to represent octal (base 8).

{: .important-title}
> Examples
>
> Number 143 can be represented as:
> ```yaml
> dec: 143
> bin: [0b10001111, 0b1000_1111]
> oct: 0217
> hex: 0x8F
> ```

Integers can be separated by `_`

```yaml
- 10000
- 10_000
# This is nasty don't do this
- 1_0_0_0_0
# This is fine
- 0x12_AB_C3
```

{: .warning-title}
> Remember
>
> - You cannot put `.inf` in an integer field, this keyword is reserved for floats.
> - Integers are finite.

```yaml
# Wrong
pets: .inf
# Correct is finite
pets: 100
```
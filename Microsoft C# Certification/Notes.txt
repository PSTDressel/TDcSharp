# C# Basics

## Console Output

### `Console.WriteLine()`
Prints text and automatically starts a new line afterward.

```csharp
Console.WriteLine("My Text!");
Console.WriteLine("Another Line!");
```

**Output:**

```text
My Text!
Another Line!
```

### `Console.Write()`
Prints text without adding a new line.

```csharp
Console.Write("My ");
Console.Write("Text!");
```

**Output:**

```text
My Text!
```

---

## Case Sensitivity

C# is **case-sensitive**.

✅ Works:

```csharp
Console.WriteLine("My Text!");
```

❌ Does not work:

```csharp
console.WriteLine("My Text!");
```

---

## Comments

Comments are created using two forward slashes (`//`).

```csharp
// This is a comment
Console.WriteLine("Hello!");
```

---

## Data Types and Literals

### Character (`char`)

Use **single quotes** (`'`) for a single character.

```csharp
Console.WriteLine('b');
```

### String (`string`)

Use **double quotes** (`"`) for one or more characters.

```csharp
Console.WriteLine("Hello!");
```

### Integer (`int`)

No quotes are required.

```csharp
Console.WriteLine(123);
```

### Float (`float`)

Append `F` to create a float literal.

```csharp
Console.WriteLine(0.25F);
```

### Decimal (`decimal`)

Append `m` (or `M`) to create a decimal literal.

```csharp
Console.WriteLine(12.39816m);
```

---

## Floating-Point Types

| Type | Approximate Precision |
|--------|----------------------|
| `float` | ~6–9 digits |
| `double` | ~15–17 digits *(default for decimal numbers)* |
| `decimal` | ~28–29 digits |

---

## Boolean Values

```csharp
Console.WriteLine(true);
Console.WriteLine(false);
```

**Output:**

```text
True
False
```

---

## Variables

### Rules

- No `#` or `$` prefixes.
- Variable names must start with:
  - A letter (`A-Z`, `a-z`), or
  - An underscore (`_`)
- Variable names cannot start with a number.
- Variable names are case-sensitive.

### Declaration Syntax

```csharp
<datatype> <variableName>;
```

### Examples

```csharp
char userOption;
int gameScore;
decimal particlesPerMillion;
bool processedCustomer;
```

### Using `var`

The `var` keyword allows the compiler to infer the data type from the assigned value.

```csharp
var firstName = "Tim";
```

In this example, `firstName` is automatically treated as a `string`.

❌ Not allowed:

```csharp
var firstName = "Tim";
firstName = 123;
```

Once the type is inferred, it cannot be changed.

---

## Quick Reference

| Example | Data Type |
|----------|-----------|
| `'A'` | `char` |
| `"Hello"` | `string` |
| `123` | `int` |
| `0.25F` | `float` |
| `0.25` | `double` |
| `12.39816m` | `decimal` |
| `true` / `false` | `bool` |

> **Tip:** If you write a decimal number without a suffix (`F`, `m`, etc.), C# treats it as a `double` by default.
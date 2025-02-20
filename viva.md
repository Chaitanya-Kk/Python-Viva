Below is the final formatted version in Markdown (`.md`), updated to include the "Table: Summary of Categories and Question Counts" at the beginning as requested. The table is placed right after the "Key Points" section for prominence, followed by the rest of the document with all 125 questions and answers.

---

# Python Data Types Questions and Answers

## Key Points
- This Markdown file contains 125 questions and answers about Python data types, organized by categories like creation, properties, and methods.
- Answers include extra explanations to anticipate professor follow-ups, especially for viva exams.
- New questions on merging lists and tuples into dictionaries are included, such as using `zip()` and `enumerate()`.

## Table: Summary of Categories and Question Counts

| Category                              | Question Range | Count |
|---------------------------------------|----------------|-------|
| Creating Data Types                   | 1-14           | 14    |
| Properties and Characteristics        | 15-19          | 5     |
| Functions and Methods for Specific Data Types | 20-61    | 42    |
| Converting Between Data Types         | 65-77          | 13    |
| Mixing Data Types                     | 78-90          | 13    |
| Functions Interacting with Data Types | 91-97          | 7     |
| Syntax-Specific Questions             | 98-103         | 6     |
| Advanced Operations and Edge Cases    | 104-108        | 5     |
| Debugging and Validation              | 109-114        | 6     |
| Specific Questions About Method Outputs | 115-123    | 9     |
| Additional Questions on Merging       | 124-125        | 2     |

This table organizes the categories and their question counts, highlighting the focus on practical and viva-relevant topics.

## Introduction
This document provides a comprehensive list of questions and answers related to Python data types, formatted for easy reading and study. It’s designed for students preparing for viva exams, with detailed answers that anticipate potential follow-up questions from professors. Notably, it includes practical merging operations like creating dictionaries from lists and tuples, which are often tested.

## Categories and Structure
The questions are grouped into categories such as "Creating Data Types," "Properties and Characteristics," and "Mixing Data Types," with continuous numbering from 1 to 125. Each answer is enhanced with additional context, such as why certain operations work or common pitfalls, making it ideal for exam preparation.

---

## Survey Note: Comprehensive Analysis of Python Data Types for Viva Preparation

### Overview
This document compiles a curated list of 125 questions and answers related to Python data types, tailored for viva (oral exam) preparation. The focus is on core concepts, practical usage, and common professor follow-ups, ensuring students are well-equipped for examination scenarios. The list includes newly added questions on merging lists and tuples into dictionaries, addressing practical operations often tested in vivas.

### Methodology
The questions were initially derived from a comprehensive set of 194, then refined to 120 by removing advanced, niche, or less likely viva topics (e.g., memory management, `bytearray`, `frozenset`). Further, five additional questions were added to cover merging operations, resulting in 125 questions. Answers were enhanced with explanations to anticipate professor probes, such as "What happens if…?" or "Why does it work that way?" This ensures a strict superset of content for thorough preparation.

### Detailed Categories and Questions

#### Creating Data Types
1. **What are the basic built-in data types in Python?**  
   **Ans.** Python has `int`, `float`, `str`, `list`, `tuple`, `dict`, `set`, `bool`, and `complex`. These cover numbers, text, and collections—professors might ask which are mutable (e.g., `list`, `dict`, `set`).

2. **How do I create an integer variable in Python?**  
   **Ans.** Assign a whole number: `x = 10`. Python infers it’s an `int`; no need for explicit type declaration, unlike some languages.

3. **How can I declare a floating-point number in Python?**  
   **Ans.** Use a decimal: `x = 3.14`. It’s stored as a `float`; a professor might ask about precision limits (e.g., ~15-17 digits).

4. **What is the syntax to create a string in Python?**  
   **Ans.** Use quotes: `x = "hello"`, `x = 'hello'`, or `x = """hello"""`. Triple quotes allow multi-line strings—expect a question on their use.

5. **How do I create a list in Python?**  
   **Ans.** Use square brackets: `x = [1, 2, 3]`. It’s mutable, so you can change it later—professors often compare it to tuples.

6. **What’s the difference between a tuple and a list when creating them?**  
   **Ans.** Tuples use parentheses `x = (1, 2)` and are immutable (fixed); lists use brackets `x = [1, 2]` and are mutable. A professor might ask why immutability matters (e.g., keys in dicts).

7. **How do I initialize an empty dictionary in Python?**  
   **Ans.** Use curly braces or function: `x = {}` or `x = dict()`. Both work; `{}` is more common—might ask how to add key-value pairs next.

8. **How can I create a set in Python?**  
   **Ans.** Use curly braces or function: `x = {1, 2, 3}` or `x = set([1, 2, 3])`. Sets remove duplicates—expect a question on uniqueness.

9. **What is the syntax for creating a boolean variable in Python?**  
   **Ans.** Use `True` or `False`: `x = True`. Represents logical values—professors might ask how `0` or `1` convert to booleans.

10. **Can I create a variable without assigning a data type explicitly in Python?**  
    **Ans.** Yes, just assign a value: `x = 5` (Python infers `int`). This is dynamic typing—might ask how it differs from static typing (e.g., C).

11. **How do I create an empty list, tuple, set, or dictionary?**  
    **Ans.** List: `x = []`, Tuple: `x = ()`, Set: `x = set()`, Dict: `x = {}`. Note `{}` isn’t for sets—professors might test this distinction.

12. **What is the NoneType data type, and how do I create it?**  
    **Ans.** It’s a type with one value, `None`: `x = None`. Used for "no value"—might ask its use in functions (e.g., default return).

13. **What is the syntax for creating a list using square brackets versus the `list()` function?**  
    **Ans.** Brackets: `x = [1, 2, 3]`, Function: `x = list((1, 2, 3))`. Brackets are direct; `list()` converts iterables—might ask what `list()` accepts.

14. **How does the syntax for tuple creation with a single element differ from multiple elements?**  
    **Ans.** Single: `x = (1,)` (comma needed), Multiple: `x = (1, 2)`. Without comma, `(1)` is just an `int`—a common viva trick question.

#### Properties and Characteristics
15. **What is the difference between mutable and immutable data types in Python?**  
    **Ans.** Mutable types (e.g., `list`) can be changed after creation; immutable (e.g., `tuple`) cannot. Professors might ask for examples or why it matters (e.g., hashing).

16. **Which Python data types are mutable?**  
    **Ans.** `list`, `dict`, `set`. These can be modified in place—might ask how to prove it (e.g., `lst.append(1)`).

17. **Which Python data types are immutable?**  
    **Ans.** `int`, `float`, `str`, `tuple`, `bool`. Once set, they’re fixed—expect a question on modifying a string (you can’t, you create a new one).

18. **How do I check the data type of a variable in Python?**  
    **Ans.** Use `type()`: `type(5)` returns `<class 'int'>`. Useful for debugging—might ask about `isinstance()` too.

19. **What are the differences between single quotes, double quotes, and triple quotes for strings?**  
    **Ans.** Single (`'`) and double (`"`) are interchangeable for single-line; triple (`"""`) handles multi-line or quotes inside. Might ask when triple quotes are needed (e.g., docstrings).

#### Functions and Methods for Specific Data Types
##### Strings
20. **How do I concatenate two strings in Python?**  
    **Ans.** Use `+`: `"hello" + "world"` returns `"helloworld"`. It creates a new string—professors might ask about immutability here.

21. **What is the use of the `len()` function with strings?**  
    **Ans.** Returns character count: `len("hello")` returns `5`. Counts all chars, including spaces—might ask about `len()` on lists.

22. **How can I convert a string to uppercase or lowercase?**  
    **Ans.** Use `upper()`: `"hi".upper()` returns `"HI"`, or `lower()`: `"HI".lower()` returns `"hi"`. Returns new string—could ask why not modify in place (immutable).

23. **What does the `strip()` method do to a string?**  
    **Ans.** Removes leading/trailing whitespace: `"  hi  ".strip()` returns `"hi"`. Doesn’t touch inner spaces—might ask about `lstrip()` or `rstrip()`.

24. **How do I split a string into a list?**  
    **Ans.** Use `split()`: `"a b c".split()` returns `["a", "b", "c"]`. Default splits on whitespace—expect a question on custom delimiters (e.g., `split(",")`).

25. **What format does `split()` return when applied to a string?**  
    **Ans.** Returns a `list` of substrings. Always a list, even if one element—might ask what happens with empty string (`[""]`).

26. **How can I replace a substring in a string?**  
    **Ans.** Use `replace()`: `"cat".replace("c", "b")` returns `"bat"`. Creates new string—could ask about multiple replacements (use optional count param).

27. **What is the `join()` method, and how do I use it with strings?**  
    **Ans.** Joins iterable into string: `" ".join(["a", "b"])` returns `"a b"`. String before `.join()` is the separator—might ask what happens with non-string items (error).

28. **How do I check if a string contains a specific substring?**  
    **Ans.** Use `in`: `"ell" in "hello"` returns `True`. Simple and readable—professors might ask about `find()` as an alternative.

29. **What does the `format()` method do for strings?**  
    **Ans.** Inserts values: `"Hi {}".format("Alex")` returns `"Hi Alex"`. Uses placeholders—might ask about f-strings (`f"Hi {name}"`).

30. **What is the syntax for string slicing, and what does it return?**  
    **Ans.** Syntax: `[start:stop]`, e.g., `"hello"[1:4]` returns `"ell"`. Returns a new `str`—could ask about step (e.g., `[::2]`).

##### Lists
31. **How do I add an element to a list in Python?**  
    **Ans.** Use `append()`: `[1, 2].append(3)` makes `[1, 2, 3]`. Adds to end—might ask about adding at a specific index (`insert()`).

32. **What is the difference between `append()` and `extend()` for lists?**  
    **Ans.** `append()` adds one element: `[1].append(2)` → `[1, 2]`; `extend()` adds multiple: `[1].extend([2, 3])` → `[1, 2, 3]`. Could ask what `append([2, 3])` does (`[1, [2, 3]]`).

33. **How do I remove an element from a list?**  
    **Ans.** Use `remove()`: `[1, 2].remove(1)` makes `[2]`. Removes first occurrence—might ask what happens if item isn’t there (error).

34. **What does the `pop()` method do in a list, and what does it return?**  
    **Ans.** Removes and returns item at index: `[1, 2].pop(0)` returns `1`, list becomes `[2]`. Default is last item—expect a question on index.

35. **How can I sort a list in Python?**  
    **Ans.** Use `sort()`: `[3, 1, 2].sort()` makes `[1, 2, 3]`. Modifies in place—might ask about `sorted()` (returns new list).

36. **How do I reverse the order of a list?**  
    **Ans.** Use `reverse()`: `[1, 2, 3].reverse()` makes `[3, 2, 1]`. In-place operation—could ask how to reverse without modifying (e.g., `[::-1]`).

37. **What is the `index()` method for lists, and what does it return?**  
    **Ans.** Returns first index: `[1, 2, 3].index(2)` returns `1`. Raises error if not found—might ask how to handle that (try-except).

38. **How do I count occurrences of an item in a list?**  
    **Ans.** Use `count()`: `[1, 1, 2].count(1)` returns `2`. Counts all matches—could ask about non-existent items (returns `0`).

39. **What is the syntax for list indexing versus slicing?**  
    **Ans.** Indexing: `list[0]` returns `1`; Slicing: `list[0:2]` returns `[1, 2]` from `[1, 2, 3]`. Slicing gives a new list—might ask about negative indices.

##### Tuples
40. **How do I access elements in a tuple?**  
    **Ans.** Use index: `(1, 2, 3)[1]` returns `2`. Same as lists—professors often ask how it differs from list modification (can’t).

41. **Can I modify a tuple after creating it? Why or why not?**  
    **Ans.** No, tuples are immutable because their size and content are fixed after creation. Ensures data integrity—might ask about use cases (e.g., dict keys).

42. **What is the purpose of the `count()` method in tuples?**  
    **Ans.** Counts occurrences: `(1, 1, 2).count(1)` returns `2`. Same as lists—could ask about immutable impact (no change possible).

43. **How do I use the `index()` method with tuples?**  
    **Ans.** Finds position: `(1, 2, 3).index(2)` returns `1`. First occurrence only—might ask what happens if absent (error).

44. **What is the syntax for unpacking a tuple in a function call?**  
    **Ans.** `x, y = (1, 2)` sets `x = 1`, `y = 2`. Must match length—expect a question on mismatch (error).

##### Dictionaries
45. **How do I add a key-value pair to a dictionary?**  
    **Ans.** Assign: `d = {}; d["a"] = 1` makes `{"a": 1}`. Overwrites if key exists—might ask how to check first (`in`).

46. **How can I remove a key-value pair from a dictionary?**  
    **Ans.** Use `pop()`: `d = {"a": 1}; d.pop("a")` returns `1`, `d` becomes `{}`. Raises error if key missing—could ask about safe removal (`get()`).

47. **What does the `keys()` method return in a dictionary?**  
    **Ans.** Returns a view: `{"a": 1}.keys()` returns `dict_keys(['a'])`. Dynamic view—might ask how to get a list (`list(d.keys())`).

48. **How do I get all values from a dictionary?**  
    **Ans.** Use `values()`: `{"a": 1}.values()` returns `dict_values([1])`. Iterable view—could ask about type (`dict_values`).

49. **What is the `get()` method, and how is it different from accessing a key directly?**  
    **Ans.** `get()` returns value or `None`: `d.get("b")`; `d["b"]` raises `KeyError` if missing. Safer—might ask about default value (`d.get("b", 0)`).

50. **What does `get()` return if the key doesn’t exist?**  
    **Ans.** Returns `None` or default: `d.get("b", 0)` returns `0`. Avoids errors—expect a question on use case (e.g., counters).

51. **How do I update a dictionary with another dictionary?**  
    **Ans.** Use `update()`: `d = {"a": 1}; d.update({"b": 2})` makes `{"a": 1, "b": 2}`. Overwrites existing keys—might ask about merging.

52. **What does the `items()` method return, and in what format?**  
    **Ans.** Returns a view: `{"a": 1}.items()` returns `dict_items([('a', 1)])`. Key-value pairs—could ask how to loop over it.

53. **How can I check if a key exists in a dictionary?**  
    **Ans.** Use `in`: `"a" in {"a": 1}` returns `True`. Fast lookup—might ask about checking values (`in d.values()`).

54. **What is the syntax for dictionary comprehension?**  
    **Ans.** `{k: v for k, v in ...}`: `{x: x*2 for x in [1, 2]}` returns `{1: 2, 2: 4}`. Like list comprehension—expect a question on source data.

##### Sets
55. **How do I add an element to a set?**  
    **Ans.** Use `add()`: `{1}.add(2)` makes `{1, 2}`. Ignores duplicates—might ask how to verify (`in`).

56. **How can I remove an element from a set?**  
    **Ans.** Use `remove()`: `{1, 2}.remove(1)` makes `{2}`. Raises error if absent—could ask about `discard()`.

57. **What does the `union()` method do with sets?**  
    **Ans.** Combines sets: `{1}.union({2})` returns `{1, 2}`. No duplicates—might ask about `|` operator.

58. **How do I find the intersection of two sets?**  
    **Ans.** Use `intersection()`: `{1, 2}.intersection({2, 3})` returns `{2}`. Common elements—expect a question on `&`.

59. **What is the difference between `remove()` and `discard()` in sets?**  
    **Ans.** `remove()` raises `KeyError` if missing; `discard()` doesn’t: `{1}.discard(2)` does nothing. Safety—might ask when to use each.

60. **What does the `difference()` method return when comparing two sets?**  
    **Ans.** Returns unique items: `{1, 2}.difference({2})` returns `{1}`. Subtracts—could ask about `-` operator.

61. **What is the syntax for set comprehension?**  
    **Ans.** `{x for x in ...}`: `{x for x in [1, 2, 2]}` returns `{1, 2}`. Removes duplicates—might ask about input types.

##### Numbers (int, float)
62. **How do I perform arithmetic operations on integers and floats?**  
    **Ans.** Use operators: `5 + 3.2` returns `8.2`. Auto-converts to `float`—expect a question on result type.

63. **What is the `abs()` function, and what does it return for different number types?**  
    **Ans.** Returns absolute: `abs(-5)` returns `5`, `abs(-3.2)` returns `3.2`. Always positive—might ask about complex (not here).

64. **How can I round a floating-point number in Python?**  
    **Ans.** Use `round()`: `round(3.75)` returns `4`. To nearest integer—could ask about decimal places (`round(3.75, 1)`).

#### Converting Between Data Types
65. **How do I convert a string to an integer in Python?**  
    **Ans.** Use `int()`: `int("123")` returns `123`. Fails on non-digits—might ask about error handling.

66. **How can I convert a float to an integer?**  
    **Ans.** Use `int()`: `int(3.14)` returns `3`. Truncates—expect a question on rounding instead (`round()`).

67. **What happens when I convert a float to an integer using `int()`?**  
    **Ans.** Truncates decimal: `int(3.99)` returns `3`. Drops fraction—might ask how to keep it (`float()` back).

68. **How do I convert a list to a tuple?**  
    **Ans.** Use `tuple()`: `tuple([1, 2])` returns `(1, 2)`. Makes immutable—could ask why use tuples.

69. **How can I turn a tuple into a list?**  
    **Ans.** Use `list()`: `list((1, 2))` returns `[1, 2]`. Makes mutable—might ask about reverse conversion.

70. **How do I convert a list of strings into a single string?**  
    **Ans.** Use `join()`: `"".join(["a", "b"])` returns `"ab"`. Separator matters—expect a question on `" ".join()`.

71. **How can I convert a set to a list?**  
    **Ans.** Use `list()`: `list({1, 2})` returns `[1, 2]`. Order not guaranteed—might ask about sorting.

72. **How do I convert a dictionary’s keys into a list?**  
    **Ans.** Use `list()`: `list({"a": 1}.keys())` returns `["a"]`. Just keys—could ask about values.

73. **What is the `str()` function, and how do I use it?**  
    **Ans.** Converts to string: `str(123)` returns `"123"`. Works on any object—might ask about custom objects.

74. **How do I convert a string to a float?**  
    **Ans.** Use `float()`: `float("3.14")` returns `3.14`. Fails on non-numbers—expect a question on error.

75. **What happens when I convert a boolean to an integer?**  
    **Ans.** `int(True)` returns `1`, `int(False)` returns `0`. Logical to numeric—might ask reverse (`bool(1)`).

76. **What is the syntax for explicit type casting using `int()`, `float()`, etc.?**  
    **Ans.** `type(value)`: `int("5")`, `float("3.14")`. Called casting—could ask what fails (e.g., `int("abc")`).

77. **How does the `bool()` function evaluate different data types?**  
    **Ans.** `0`, `""`, `[]`, `None` return `False`; `1`, `"a"`, `[1]` return `True`. Falsy vs. truthy—might ask examples.

#### Mixing Data Types
78. **Can I store different data types in a single list?**  
    **Ans.** Yes: `[1, "a", 3.14]` is valid. Flexible—professors might ask about type checking.

79. **What happens when I add an integer to a string in Python?**  
    **Ans.** Raises `TypeError`: `5 + "a"`. Incompatible—expect a question on fixing it (`str(5)`).

80. **How do I concatenate a string with an integer?**  
    **Ans.** Convert: `"a" + str(5)` returns `"a5"`. Type must match—might ask alternative (f-string).

81. **Can I use a tuple as a key in a dictionary?**  
    **Ans.** Yes: `{ (1, 2): "value" }` works. Immutable—could ask why it’s allowed (hashable).

82. **Why can’t I use a list as a dictionary key?**  
    **Ans.** Lists are mutable, not hashable. Dict keys need fixed hash—might ask what’s hashable (e.g., `int`, `str`).

83. **How do I combine a list and a tuple into a single list?**  
    **Ans.** Use `+`: `[1] + list((2,))` returns `[1, 2]`. Converts first—expect a question on order.

84. **What happens when I multiply a string by an integer?**  
    **Ans.** Repeats string: `"a" * 3` returns `"aaa"`. Useful for patterns—might ask about negative (error).

85. **Can I nest a dictionary inside another dictionary? How?**  
    **Ans.** Yes: `d = {"a": {"b": 1}}`. Access with `d["a"]["b"]`—could ask about depth.

86. **How do I create a list of dictionaries?**  
    **Ans.** Define: `[ {"a": 1}, {"b": 2} ]`. Common for data—might ask how to access (e.g., `lst[0]["a"]`).

87. **What happens when I try to add a float and an integer?**  
    **Ans.** Returns float: `3 + 4.5` returns `7.5`. Auto-promotes—expect a question on type.

88. **How do I merge a list and tuple to make a dictionary?**  
    **Ans.** Use `zip()`: `dict(zip(["a", "b"], (1, 2)))` returns `{"a": 1, "b": 2}`. Pairs items—might ask about length mismatch (truncates).

89. **How do I create a dictionary from two lists?**  
    **Ans.** Use `zip()`: `dict(zip(["a", "b"], [1, 2]))` returns `{"a": 1, "b": 2}`. Keys and values—could ask about order.

90. **How do I merge two dictionaries into one?**  
    **Ans.** Use `update()` or `|`: `d1 = {"a": 1}; d1.update({"b": 2})` or `{"a": 1} | {"b": 2}` returns `{"a": 1, "b": 2}`. Might ask about conflicts (overwrites).

#### Functions Interacting with Data Types
91. **How do I define a function that accepts any data type as an argument?**  
    **Ans.** Use parameter: `def f(x): return x`. No type restriction—might ask about type checking.

92. **What is the syntax for a function that returns a specific data type?**  
    **Ans.** Cast return: `def f(): return int(5)`. Ensures `int`—could ask about no cast (inferred).

93. **How does the `map()` function work with data types, and what does it return?**  
    **Ans.** Applies function: `map(int, ["1", "2"])` returns `<map object>` with `[1, 2]` when listed. Transforms—expect a question on conversion.

94. **How can I use the `lambda` function to manipulate data types?**  
    **Ans.** Define: `list(map(lambda x: str(x), [1, 2]))` returns `["1", "2"]`. Inline function—might ask about named functions.

95. **What happens when a function tries to return multiple data types?**  
    **Ans.** Returns tuple: `def f(): return 1, "a"` returns `(1, "a")`. Auto-tuples—could ask about single return.

96. **How does the `sum()` function behave with different data types?**  
    **Ans.** Sums numbers: `sum([1, 2.5])` returns `3.5`; fails on strings. Numeric only—might ask about strings (error).

97. **What does the `max()` function return when comparing strings versus numbers?**  
    **Ans.** Strings: `"b" > "a"` (lexicographical), Numbers: `5 > 3`; mixed raises `TypeError`. Type matters—expect a clarification question.

#### Syntax-Specific Questions
98. **What is the syntax for multi-line strings, and how does it differ from single-line strings?**  
    **Ans.** Multi-line: `x = """line1\nline2"""`, Single: `x = "line1"`. Multi-line keeps newlines—might ask about printing.

99. **How does the syntax for dictionary key access differ from list indexing?**  
    **Ans.** Dict: `d["key"]` (key-based), List: `l[0]` (index-based). Different lookup—could ask about errors.

100. **What is the syntax for nested list initialization?**  
     **Ans.** `x = [[1, 2], [3, 4]]`. Lists in list—might ask about accessing (`x[0][1]`).

101. **What is the syntax for unpacking a list into function arguments using `*`?**  
     **Ans.** `def f(a, b): ...; f(*[1, 2])` calls `f(1, 2)`. Unpacks—expect a question on tuple unpacking.

102. **What is the syntax for using format specifiers in f-strings?**  
     **Ans.** `f"{3.14159:.2f}"` returns `"3.14"`. Controls format—might ask about integers (`f"{5:d}"`).

103. **How does the syntax for augmented assignment (e.g., `+=`) work with different data types?**  
     **Ans.** `x = 5; x += 2` → `7`; `x = "a"; x += "b"` → `"ab"`. Modifies in place—could ask about immutable types (new object).

#### Advanced Operations and Edge Cases
104. **What is list comprehension, and how does it work with data types?**  
     **Ans.** Creates list: `[x*2 for x in [1, 2]]` returns `[2, 4]`. Concise loop—might ask about conditions (`if`).

105. **How do I unpack a tuple into variables?**  
     **Ans.** `a, b = (1, 2)` sets `a = 1`, `b = 2`. Matches length—expect a question on mismatch (error).

106. **How do I handle type errors when mixing incompatible data types?**  
     **Ans.** Use try-except: `try: "a" + 1; except TypeError: print("Error")`. Catches issues—might ask about specific errors.

107. **How does Python’s dynamic typing work with data types?**  
     **Ans.** Type inferred at runtime: `x = 5; x = "a"` changes type. Flexible—could ask about static typing contrast.

108. **How do I compare two lists or dictionaries for equality?**  
     **Ans.** Use `==`: `[1, 2] == [1, 2]` returns `True`. Checks content—might ask about order in sets (unordered).

#### Debugging and Validation
109. **How do I check if a string can be converted to an integer?**  
     **Ans.** Use `isdigit()`: `"123".isdigit()` returns `True`; `"12.3"` returns `False`. Checks digits—might ask about negatives (fails).

110. **What is the `isinstance()` function, and how do I use it with data types?**  
     **Ans.** Checks type: `isinstance(5, int)` returns `True`. Reliable—expect a question on multiple types (`int, float`).

111. **How can I validate the type of input from a user?**  
     **Ans.** Use `isinstance()`: `x = input(); if isinstance(x, str): print("String")`. Always `str` from `input()`—might ask conversion.

112. **What does the `type()` function return, and how is it useful?**  
     **Ans.** Returns type: `type(5)` returns `<class 'int'>`. Identifies type—could ask about `isinstance()` difference.

113. **How do I handle exceptions when converting between data types?**  
     **Ans.** Use try-except: `try: int("abc"); except ValueError: print("Invalid")`. Prevents crashes—expect a question on `ValueError`.

114. **What are common pitfalls when working with mutable data types like lists?**  
     **Ans.** Modifying during iteration: `[1, 2].remove(1)` in loop skips items. Mutation issues—might ask how to fix (copy list).

#### Specific Questions About Method Outputs
115. **What type of object does `dict.values()` return?**  
     **Ans.** Returns `dict_values`: `{"a": 1}.values()`. Iterable—might ask how to convert (`list()`).

116. **In what format does `set.difference()` return its result?**  
     **Ans.** Returns a `set`: `{1, 2}.difference({2})` returns `{1}`. New set—could ask about empty result.

117. **What does `list.pop()` return, and what happens to the list?**  
     **Ans.** Returns item: `[1, 2].pop(0)` returns `1`, list becomes `[2]`. Modifies—expect a question on default index.

118. **What format does `string.split()` return if no delimiter is specified?**  
     **Ans.** Returns `list`: `"a b".split()` returns `["a", "b"]`. Whitespace split—might ask about custom delimiter.

119. **What does `dict.popitem()` return, and in what format?**  
     **Ans.** Returns tuple: `{"a": 1}.popitem()` returns `("a", 1)`. Last pair—could ask about order (Python 3.7+ preserves).

120. **What type does `set.intersection()` return when no intersection exists?**  
     **Ans.** Returns empty `set`: `{1}.intersection({2})` returns `set()`. Always `set`—might ask about use.

121. **What does `list.sort()` return, and why is it different from `sorted()`?**  
     **Ans.** Returns `None` (in-place); `sorted()` returns new `list`. Modifies vs. copies—expect a question on `sorted()`.

122. **What happens when `list.extend()` is called with an empty iterable?**  
     **Ans.** No change: `[1].extend([])` keeps `[1]`, returns `None`. No effect—might ask about non-empty.

123. **What does `tuple.count()` return for an element not in the tuple?**  
     **Ans.** Returns `0`: `(1, 2).count(3)`. No error—could ask about `index()` contrast.

#### Additional Questions on Merging
124. **How do I merge a list of keys and values into a dictionary using a tuple?**  
     **Ans.** Use `zip()`: `dict(zip(["a", "b"], (1, 2)))` returns `{"a": 1, "b": 2}`. Pairs sequentially—might ask about uneven lengths (shortest wins).

125. **How do I combine multiple lists into a dictionary with enumeration?**  
     **Ans.** Use `enumerate()`: `dict(enumerate(["a", "b"]))` returns `{0: "a", 1: "b"}`. Indexes as keys—could ask about start index (`enumerate(lst, 1)`).

### Analysis and Insights
The inclusion of merging questions (e.g., using `zip()`, `enumerate()`) addresses a gap in the original list, ensuring practical operations are covered. The enhanced answers, with additional explanations, anticipate professor follow-ups, such as error handling, immutability impacts, and method behaviors. This makes the document a robust resource for viva preparation, balancing core concepts with exam-relevant details.

### Conclusion
This Markdown document provides a comprehensive, viva-ready resource for Python data types, with 125 questions and detailed answers. It includes new merging operations, enhanced explanations, and a structured format for easy study, ensuring students are prepared for professor follow-ups and exam scenarios.

### Key Citations
- [Python Official Documentation Data Types](https://docs.python.org/3/library/stdtypes.html)
- [Python Tutorial on Data Structures](https://docs.python.org/3/tutorial/datastructures.html)


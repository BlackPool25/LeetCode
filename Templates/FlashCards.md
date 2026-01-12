## Leetcode Note Template

````markdown
---
tags: leetcode
difficulty: 
topics: 
---

# Problem: {{title}}

## Solution

```python
# your code here
````

## Key Concepts

## Complexity Analysis

- Time:
- Space:

````

---

## How to Use It

- If you use **Templater**, save the template in your Templates folder and bind a hotkey like "Insert template: Leetcode Template".
- Otherwise, manually copy-paste this structure each time.

---

## How to Write Notes for Auto-Generated Flashcards

To make AI plugins extract good Q/A pairs, structure your content like this:

### In **Key Concepts**:

```md
## Key Concepts
- Sliding window to maintain current substring.
- Use hashmap to store last index of each character.
- Move left pointer when duplicate is found.
````

### In **Complexity Analysis**:

```md
## Complexity Analysis
- Time: O(n) because each character is visited at most twice.
- Space: O(k) for hashmap where k is character set size.
```
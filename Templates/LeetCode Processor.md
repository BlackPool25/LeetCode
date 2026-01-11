---
mode: replace
---
**ACT AS:** A Senior Software Engineer and Technical Interview Coach creating high-quality, archival-grade study notes for Data Structures and Algorithms optimized for future review and pattern recognition.

**YOUR GOAL:** Transform the coding problem and solution I provide into a comprehensive, easily revisable study note that emphasizes pattern recognition and technique mastery.

**CRITICAL INSTRUCTIONS:**

- I am pasting a LeetCode problem description and MY solution code
- **DO NOT generate, modify, or rewrite my code** - use my exact solution as provided
- Your job is to **organize, explain, and add context** around my solution
- Create notes that help me **recognize similar problems** and **recall the solution pattern** during future reviews
- Ensure all explanations are clear enough for my future self to understand without external references
- Verify that code blocks, LaTeX expressions, and Markdown formatting are perfect for Obsidian
- **Be precise with pattern identification** - verify the pattern name matches the actual solution approach
- **Avoid redundancy** - each section should add NEW information, don't repeat the same concept in different words
- **Focus on what MY FUTURE SELF needs** to recognize and recall this pattern quickly
- **Do not add meta-commentary** at the end about whether the explanation is clear

---

## OUTPUT FORMAT

# [Problem Number]. [Problem Title]

## 0. Problem Metadata

- **Difficulty:** [Easy/Medium/Hard]
- **Topics/Tags:** [e.g., Array, Two Pointers, Sliding Window, Dynamic Programming]
- **Pattern Category:** [Be SPECIFIC - e.g., "Two Pointers - Same Direction (Fast-Slow)", "Sliding Window - Variable Size", "Two Pointers - Opposite Ends"]
- **LeetCode Link:** [URL if available]

## 1. Problem Statement

> **[Copy the FULL problem description here. Do not summarize.]**
> 
> **Example 1:** Input: [...] Output: [...] Explanation: [...]
> 
> **Example 2:** [Include all provided examples]

## 2. Constraints & Key Observations

- **Constraints:**
    
    - [List all constraints exactly as given, e.g., "1 ≤ nums.length ≤ 10^5"]
    - [Include data type limits, special conditions]
- **What constraints tell us:**
    
    - [e.g., "n ≤ 10^5 means O(n²) might be too slow; aim for O(n) or O(n log n)"]
    - [e.g., "Array is guaranteed non-empty, so no need to check for empty array"]
- **Key observations:**
    
    - [Properties of input that hint at the approach]
    - [Patterns noticed in the examples that lead to the solution]
- **Edge cases to handle (based on actual constraints):**
    
    - [Only list edge cases that are POSSIBLE given the constraints]
    - [e.g., If constraint says "1 ≤ n", don't mention "empty array"]
    - [e.g., Single element, all duplicates, no duplicates, etc.]

## 3. Solution Development

### 3.1 Core Intuition

**Keep this section concise (3-5 sentences max):**

- **The "Aha!" moment:** What is the ONE key insight that unlocks this problem?
- **Algorithm invariant:** What property is maintained throughout execution? [e.g., "At any point, nums[0...i] contains only unique elements"]
- **Why this works:** Brief fundamental reasoning

### 3.2 Algorithm Strategy

**High-level approach (don't repeat Section 3.1):**

1. [First major step with clear purpose]
2. [Second major step with clear purpose]
3. [Continue with logical progression]
4. [Focus on WHAT happens, save the detailed WHY for the walkthrough]

## 4. Example Walkthrough

**Trace through Example 1 step-by-step:**

Input: [...]

**Initial state:**

- [Variable initializations]

**Execution trace:**

- **Step 1:** [State changes, decisions made, WHY]
- **Step 2:** [State changes, decisions made, WHY]
- [...continue for key steps - be thorough here]

**Final result:** [...]

[If helpful, trace a second example to show different behavior]

## 5. Complexity Analysis

- **Time Complexity:** $O(?)$
    - **Why:** [Explain in terms of the operations: "Single pass (n iterations) × constant work per iteration"]
- **Space Complexity:** $O(?)$
    - **Why:** [Explain what data structures are used and their size: "Only constant variables (i, j) regardless of input size"]

## 6. Code Solution (C++)

```cpp
[PASTE MY EXACT CODE HERE - DO NOT MODIFY IT]
[Only add inline comments if they clarify non-obvious logic]
```

## 7. Key Takeaways & Pattern Recognition

### 🎯 Pattern Recognition

- **This pattern applies when:**
    
    - [SPECIFIC criterion 1: e.g., "Array is sorted AND need to modify in-place"]
    - [SPECIFIC criterion 2: e.g., "Need to track 'valid' vs 'exploring' positions"]
    - [SPECIFIC criterion 3: e.g., "Can compare adjacent or nearby elements"]
    - [Avoid generic statements like "need to find subarray with property"]
- **Pattern Structure (reusable template):**
    

```cpp
// [Name of pattern, e.g., "Two Pointers - Same Direction"]
// [Brief description of what pointers represent]

[pointer_type] slow = [initial_value];  // [what this tracks]

for([pointer_type] fast = [initial_value]; [condition]; [increment]) {
    if([some_condition]) {
        // [what happens when condition is true]
        slow++;
        [operation]
    }
}

return [final_result];  // [what this represents]
```

### 💡 Key Insights

- [Most important technical insight - avoid repeating intuition from Section 3]
- [Specific technique or optimization used in MY solution]
- [Common mistake to avoid - be specific]

### 🔗 Related Problems

- **Practice these similar problems:**
    - LC [Number]: [Title] - [Specific reason it's similar, e.g., "Same fast-slow pointer pattern but with different condition"]
    - LC [Number]: [Title] - [Specific reason it's similar]

### 📝 Review Checklist

- [ ] Can I identify this pattern from the problem description alone?
- [ ] Do I understand the invariant maintained by the algorithm?
- [ ] Can I explain why this approach works to someone else?
- [ ] Can I handle the edge cases?
- [ ] Can I code this from memory in 15 minutes?

---

## Your Input:

{{selection}}

---

**FORMATTING REQUIREMENTS:**

1. ✅ Ensure all code blocks use proper ```cpp syntax with closing tags
2. ✅ Use LaTeX for all mathematical expressions: $O(n)$, $O(n \log n)$, etc.
3. ✅ Use **bold** for emphasis, _italics_ for secondary emphasis
4. ✅ Ensure headers follow proper Markdown hierarchy (no skipping levels)
5. ✅ Keep explanations clear and self-contained (future me should understand without googling)
6. ✅ **CRITICAL: Use my exact code in Section 6 - do not generate or modify it**
7. ✅ Verify the pattern category name accurately describes MY solution's approach

**QUALITY CHECKS:**

- Is the pattern name precise and matches the actual implementation?
- Does each section add unique information without repetition?
- Are edge cases based on actual constraints (not impossible scenarios)?
- Is the "Pattern Recognition" section specific enough to identify similar problems?
- Does the template/framework show the reusable structure?
- Are explanations clear for someone reviewing months later?
- Did you use MY CODE exactly as provided?
- Did you avoid adding meta-commentary about the quality of explanations?
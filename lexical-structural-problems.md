#  Anagram Cheat Sheet

## 🔹 What is an Anagram?
An **anagram** is a word or phrase formed by rearranging the letters of another word while keeping the same character frequency.  
For example:  
- `"listen"` → `"silent"`  
- `"race"` → `"care"`  
- `"rat"`  `"car"` (Not an anagram, different character frequency)

---

##  How to Check for Anagrams?

###  1. Sorting Approach (O(n log n))
Sort both words and compare.
```python
def is_anagram(s: str, t: str) -> bool:
    return sorted(s) == sorted(t)

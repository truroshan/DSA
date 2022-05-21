
### Leetcode

<details>
    <summary>9. Palindrome Number</summary>

```python
class Solution:
    def isPalindrome(self, x: int) -> bool:
        
        if (x<0) or ( x>0 and x%10 == 0):
            return False
        
        number = x
        store = 0
        
        while number > 0:
            
            store = store * 10 + (number % 10)
            
            number = number//10
            
        return store == x
```
</details>
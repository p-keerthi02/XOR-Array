class Solution:
    def decode(self, encoded: List[int], first: int) -> List[int]:
        x = [first]
        for i in encoded:
            x.append(x[-1]^i)
        return x

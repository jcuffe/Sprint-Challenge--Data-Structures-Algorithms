Exercise I:
a) O(n) -- (n^3 / n^2 = n)
b) O(logn) -- (halving each step)
c) O(64 n^(1/2) / 2) or O(sqrtn / 2)
d) O(n logn) -- out loop logn, inner loop n
e) O(n^3)
f) O(n) -- bunnyEars is called once for every number n..0
g) O(n) -- search is called for every arraySize from n..0

Exercise II:
a) findMaxDiff(arr) {
  let diffs = []
  let min = arr[0]
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] < min) {
      min = arr[i]
    } else {
      diffs.push(arr[i] - min)
    }
  }

  let maxDiff = 0
  for (let i = 0; i < diffs.length; i++) {
    if (arr[i] > maxDiff) {
      maxDiff = arr[i]
    }
  }

  return maxDiff
}

b) Use binary sectioning. Start at f' = n/2. If egg breaks, set f' = f'/2. If egg does not break, set f' = 3f'/2

Exercise III:
a) O(n^2). Each time a pivot is selected, the entire array must be inspected for partitioning. If the pivot is always the smallest remaining element, there will be n pivot inspections which must compare roughly n nodes per iteration.

b) O(nlogn). Each time a pivot is selected, half the array is seen to be smaller than the pivot, and half larger. There will be n pivot selections, which must each compare against an array half as large as the previous iteration
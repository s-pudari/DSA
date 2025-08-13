📌 Sorting Algorithms – Stability, Usage, and Purpose
🧩 What is Stability in Sorting?
  A stable sorting algorithm keeps the relative order of elements with equal keys (values).

Example:
  If we sort [(4, 'C'), (2, 'B'), (4, 'A')] by the first number:

  Stable sort → [(2, 'B'), (4, 'C'), (4, 'A')] ✅ (A comes before C because it was before in the original list)
           

  Unstable sort → [(2, 'B'), (4, 'A'), (4, 'C')] ❌ (Order of equal elements changed)

When stability matters:

  Sorting records by multiple keys (e.g., sort by Name, then by Age).

   When preserving the original order for same-value items is important.

<img width="1227" height="750" alt="image" src="https://github.com/user-attachments/assets/79189bb1-e7fe-44b7-896f-a05a4c585391" />

💡 Quick Guidelines – Which One Should You Pick?

   For small datasets: Insertion Sort or Bubble Sort (easy to implement, readable for learning).

   For large datasets: Merge Sort or Quick Sort (fast, well-balanced).

  When stability is crucial: Merge Sort, Insertion Sort, Counting Sort, or Radix Sort.

  When memory is limited: Heap Sort or Selection Sort (in-place sorting).

  For integers with a known range: Counting Sort or Radix Sort (super fast).

🎯 Interview Tip
  If the interviewer asks:

  “Why choose one algorithm over another?”
You can say:
 “It depends on dataset size, whether stability matters, memory limits, and data distribution. For example, I’d choose Merge Sort for large, 
 stable sorting; Quick Sort for general-purpose fast in-memory sorting; and Counting Sort for small-range integers.”

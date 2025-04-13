Project Report

Course Name: Algorithm Design and Analysis Lab
Course Code: CSE 132
        
 Submitted to:
Nasif Istiak Remon
Lecturer
Department of  Computer Science &  Engineering,
 Metropolitan University, Sylhet.


 Submitted by:
Mehedi Hasan
ID: 232-115-005
&
Md.Mehrab Hasan Akhanjee
ID: 232-115-006

  Department of  Computer Science & Engineering
Metropolitan University, Sylhet.



Date of submission: 13.04.2025





1.	Introduction

This report describes an interactive visualizer for the Heap Sort algorithm, implemented in C++. The program demonstrates how a min-heap is constructed from user input and then visualizes the sorting process step by step in the terminal. The tool is designed to enhance understanding of heap construction, the min-heapify operation, and the extraction phase during sorting.
This visualization can help students understand sorting algorithms better, particularly how a binary heap works behind the scenes.

2.Problem Description

Heap Sort is a comparison-based sorting algorithm that utilizes a binary heap data structure. This project focuses on implementing Heap Sort using a Min Heap, where the smallest element is always at the root.
The algorithm involves two main phases:
•	Heap Construction: The input array is transformed into a min heap.
•	Heap Extraction: The root is extracted, and the heap is restructured repeatedly.

3.Solution Approach

The program’s approach includes:
•	Manual Input: The user inputs the number of elements and their values.
•	Min Heap Construction: A bottom-up approach is used to heapify the array.
•	Visualization: Each operation (heapify, swap, extraction) is visualized with a delay and a tree-like structure using indentation and levels.
•	Customization: The user sets the delay time in milliseconds.
•	Statistics: The total number of comparisons and swaps is shown at the end.

4. Code Structure and Design
The program is divided into logical components:

4.1 Input Handling
•	The user is prompted to input the number of elements.
•	Then, the elements of the array are input manually.
•	Finally, the delay time is taken as input.
4.2 Heap Construction and Update
•	A bottom-up approach is used for heapifying the array.
•	Each heapify operation and swap is logged.
•	The heap structure is printed visually in each step.
4.3 Display Functions
•	Tree Printing: The heap is printed as a tree, using recursive formatting and indentation.
•	Clear Screen: The screen is cleared between steps using platform-specific commands.
•	Delay: std::this_thread::sleep_for is used for visual delay between steps.
4.4 Decision Messages
•	When an element is compared or swapped, a message is printed.
•	Highlighting helps users understand the logic of heapify decisions.
4.5 Final Output
•	The final sorted array is displayed.
•	Total comparisons and swaps are printed for analysis.


5. Time Complexity

•	Heap Construction: O(n)
•	Heap Sort (Extraction): O(n log n)
•	Total Complexity: O(n log n)
•	Space Complexity: O(1), in-place sorting is performed.




6. Additional Considerations

•	Platform Compatibility: Works on both Windows and Linux-based systems.
•	Educational Value: Useful for learning tree-based sorting and visual debugging.
•	Potential Enhancements:
o	Graphical UI using a library like SFML or Qt.
o	Toggle between Min Heap and Max Heap mode.
o	Step-back functionality.


7. Future Scope

•	GUI Integration: Use libraries like SFML or Qt for a more intuitive graphical interface.
•	Step Controls: Add next/back options to let users control the sorting steps.
•	Max Heap Support: Allow switching between Min Heap and Max Heap.
•	Better Visualization: Highlight active elements during comparisons and swaps.
•	Export Feature: Save logs or stats for analysis.
•	Web/Mobile Version: Expand accessibility by making it platform-independent.
•	Multi-Algorithm Support: Include other sorting algorithms for comparison.

8. Limitations

•	Terminal-Based View: Tree layout may become unclear with large heaps.
•	No Step Navigation: Users can't pause or rewind the process.
•	Basic Input Handling: No validation for incorrect inputs.
•	Platform Dependent: system("cls"/"clear") may not work in all environments.
•	Performance Drops: Slows down for larger arrays due to frequent screen updates.



9. Conclusion

This interactive Heap Sort visualizer offers a step-by-step breakdown of heap construction and the sorting process. Through its terminal-based visualization and decision tracking, it serves as a helpful educational tool for understanding heap operations. The visual feedback reinforces the conceptual workings of comparison-based sorting and binary trees.

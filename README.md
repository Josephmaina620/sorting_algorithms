In this project, I have implemented various sorting algorithms.

Tests:

Tests: Contains a folder of test files.
Helper Files:

print_array.c: A C function designed to print an array of integers.
print_list.c: A C function developed to print a doubly-linked list of integers (listint_t).

Header Files:

sort.h: A header file that encompasses definitions and prototypes for all types and functions crafted for the project.

Data Structure:

typedef struct listint_s
{
	const int n;
	struct listint_s *prev;
	struct listint_s *next;
} listint_t;

Function Prototypes:


File	Prototype
print_array.c	void print_array(const int *array, size_t size)
print_list.c	void print_list(const listint_t *list)
0-bubble_sort.c	void bubble_sort(int *array, size_t size);
1-insertion_sort_list.c	void insertion_sort_list(listint_t **list);
2-selection-sort.c	void selection_sort(int *array, size_t size);
3-quick_sort.c	void quick_sort(int *array, size_t size);
100-shell_sort.c	void shell_sort(int *array, size_t size);
101-cocktail_sort_list.c	void cocktail_sort_list(listint_t **list);
102-counting_sort.c	void counting_sort(int *array, size_t size);
103-merge_sort.c	void merge_sort(int *array, size_t size);
104-heap_sort.c	void heap_sort(int *array, size_t size);
105-radix_sort.c	void radix_sort(int *array, size_t size);
106-bitonic_sort.c	void bitonic_sort(int *array, size_t size);
107-quick_sort_hoare.c	void quick_sort_hoare(int *array, size_t size);
deck.h	Header file containing definitions and prototypes for all types and functions written for the task 1000-sort_deck.c.

Data Structures:

typedef enum kind_e
{
	SPADE = 0,
	HEART,
	CLUB,
	DIAMOND
} kind_t;

typedef struct card_s
{
	const char *value;
	const kind_t kind;
} card_t;

typedef struct deck_node_s
{
	const card_t *card;
	struct deck_node_s *prev;
	struct deck_node_s *next;
} deck_node_t;


Function Prototype:

File	Prototype
1000-deck_node.c	void sort_deck(deck_node_t **deck);


Tasks:


Bubble sort:
0-bubble_sort.c: Sorts an array of integers in ascending order using the Bubble Sort algorithm.
0-O: Text file containing the best, average, and worst-case time complexities of the Bubble Sort algorithm, each on one line.
Insertion sort:
1-insertion_sort_list.c: Sorts a doubly-linked list of integers in ascending order using the Insertion Sort algorithm.
1-O: Text file containing the best, average, and worst-case time complexities of the Insertion Sort algorithm, each on one line.
Selection sort:
2-selection_sort.c: Sorts an array of integers in ascending order using the Selection Sort algorithm.
2-O: Text file containing the best, average, and worst-case time complexities of the Selection Sort algorithm, each on one line.
Quick sort:
3-quick_sort.c: Sorts an array of integers in ascending order using the Quick Sort algorithm (Lomuto partition scheme).
3-O: Text file containing the best, average, and worst-case time complexities of the Quick Sort Lomuto Partition scheme algorithm, each on one line.
Shell sort - Knuth Sequence:
100-shell_sort.c: Sorts an array of integers in ascending order using the Shell sort algorithm.
Cocktail shaker sort:
101-cocktail_sort_list.c: Sorts a doubly-linked list of integers in ascending order using the Cocktail Shaker Sort algorithm.
101-O: Text file containing the best, average, and worst-case time complexities of the Cocktail Shaker Sort algorithm, each on one line.
Counting sort:
102-counting_sort.c: Sorts an array of integers in ascending order using the Counting Sort algorithm.
102-O: Text file containing the best, average, and worst-case time complexities of the Counting Sort algorithm, each on one line.
Merge sort:
103-merge_sort.c: Sorts an array of integers in ascending order using the Merge Sort algorithm.
103-O: Text file containing the best, average, and worst-case time complexities of the Merge Sort algorithm, each on one line.
Heap sort:
104-heap_sort.c: Sorts an array of integers in ascending order using the Heap Sort algorithm.
104-O: Text file containing the best, average, and worst-case time complexities of the Heap Sort algorithm, each on one line.
Radix sort:
105-radix_sort.c: Sorts an array of integers in ascending order using the Radix Sort algorithm.
105-O: Text file containing the best, average, and worst-case time complexities of the Radix Sort algorithm, each on one line.
Bitonic sort:
106-bitonic_sort.c: Sorts an array of integers in ascending order using the Bitonic Sort algorithm.
106-O: Text file containing the best, average, and worst-case time complexities of the Bitonic Sort algorithm, each on one line.
Quick Sort - Hoare Partition scheme:
107-quick_sort_hoare.c: Sorts an array of integers in ascending order using the Quick Sort algorithm (Hoare partition scheme).
107-O: Text file containing the best, average, and worst-case time complexities of the Quick Sort Hoare Partition scheme algorithm, each on one line.
Dealer:
1000-sort_deck.c: Sorts a doubly-linked list deck of cards from spades to diamonds and from aces to kings.

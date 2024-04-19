<h2>C- List Library</h2>

<h2>Description</h2>
This project was done to gain a better understanding in C and create a list data strcuture that will help in deepning the underrstanding of pointers.

<pre>
  /* Below is the design plan and things like 
pre-conditions, post-conditions for this list lib*/

/*
* Creates a new, empty list and returns a 
pointer to it if successuful or null if list creation failed.
* Pre-condition: None
* Post-condition: returns reference to the list 
structure if, it is created or null if not
*/
List *ListCreate() {}

/*
* Returns number of items in list.
* pre-condition: list: a List data structure.
* post-condition: number of items in the list passed as an argument.
*/
int ListCount(list) {}

/*
* returns a pointer to the first item in list 
and makes the first item the current item.
* pre-condition: list should not be empty.
* post-condition: first item is set as the current 
item and a pointer to first item is returned.
*/
void *ListFirst(list) {}


/*
* returns a pointer to the last item in list 
and makes the last item the current one.
* pre-condition: List should not be empty
* post-condition: last item is set as the 
current item and a pointer to last item is returned
*/
void *ListLast(list) {}

/*int ListAppend(list, item) adds item to the end of list, 
and makes the new item the current one. Returns 0 on success, -1 on failure.

* Advance the pointer to next item in the list
* pre-condition: list should not be empty
* post-condition: moves the cursor to the next item, and returns a 
pointer to the next item or null if there is no next item.
*/
void *ListNext(list) {}


/*
* sets the cursor to previous node and returns a pointer to it
* pre-condition: list not empty
* post-condition: sets cursor to the previous item and returns a 
pointer to it or null if there is no prev item
*/
void *ListPrev(list) {}


/*
* returns a pointer to current item
* pre-condition: None
* post-condition: a pointer tu current item is returned
*/
void *ListCurr(list) {}

/*
* adds a new item to the list after the current 
item and return 0 on success or -1 on failure
* pre-condition: None
* post-condition: item is added to the list after the current 
item and current item cursor is set to the new item
*/
int ListAdd(list, item) {}

/*
* adds a new item to the list after the 
current item and return 0 on success or -1 on failure
* pre-condition: None
* post-condition: item is added to the list before the current 
item and current item cursor is set to the new item
*/
int ListInsert(list, item) {}



/*
* adds a new item to the end of the list returns 0 on success or -1 on failure
* pre-condition: None
* post-condition: new item is added to the list 
and current item cursor is set on the new item
*/int ListAppend(list, item) {}



/*
* adds a new item to the begining of 
the list returns 0 on success or -1 on failure
* pre-condition: None
* post-condition: new item is added to the 
list and current item cursor is set on the new item
*/
int ListPrepend(list, item) {}



/*
* returns the current item and deletes it from the list
* pre-condition: List non-empty
* post-condition: current item cursor is changed to 
the next item and a pointer to current item is returned
*/
void *ListRemove(list) {}


/*
* adds list2 to the end of list 1
* pre-condition: list1, list2
* post-condition: List 2 is added to the end of list 1, 
list1's cursor is the cursor for the whole new list and list 2 is destroyed
*/
void ListConcat(list1, list2) {}


/*
* deletes list
* pre-condition: list, itemFree: a routine to free an item
* post-condition: list and all the items in it are deallocated or freed
*/
void ListFree(list, itemFree) {}


/*
* returns last item in the last and deletes it
* pre-condition: list is not empty
* post-condition: last item is deleted from the list and curssor 
points to the new last item
*/
void *ListTrim(list) {}


/*
* searches for comparator in list starting at the current item 
till the end of the list
* pre-condition: comparisonArg is not null
* post-condition: cursor set to the item that matches comparisonArg
(checked by comparator routine) if it is in the list or left 
at the end of the list
*/

</pre>

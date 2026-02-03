#include <stdio.h>
#define MAX 100 // Maximum capacity of the stack

int stack[MAX];
int top = -1;

// 1. Push: Add a page ID to the stack
void push(int pageID) {
    if (top >= MAX - 1) {
        printf("Stack Overflow! Cannot add more pages.\n");
    } else {
        stack[++top] = pageID;
        printf("Opened page: %d\n", pageID);
    }
}

// 2. Pop: Remove the current page
int pop() {
    if (top == -1) {
        printf("Stack Underflow! No pages to go back to.\n");
        return -1;
    } else {
        return stack[top--];
    }
}

// 3. Peek: View the current page
int peek() {
    if (top == -1) return -1;
    return stack[top];
}

// 4. isEmpty: Check if history is empty
int isEmpty() {
    return top == -1;
}

// 5. Size: Get total pages
int size() {
    return top + 1;
}

int main() {
    // Sample Use Case
    push(101);
    push(102);
    push(103);

    printf("Back pressed -> removed %d\n", pop());
    printf("Current page -> %d\n", peek());
    printf("Total pages in history: %d\n", size());

    return 0;
}
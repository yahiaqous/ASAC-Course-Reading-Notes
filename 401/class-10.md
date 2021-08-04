# Stacks and Queues

## Stacks

**A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack but does not reference its previous.**

Common terminology for a stack:

- **_Push_** - Nodes or items that are put into the stack are pushed.
- **_Pop_** - Nodes or items that are removed from the stack are popped
- **_Top_** - This is the top of the stack.
- **_Peek_** - When you peek you will view the value of the top Node in the stack.
- **_IsEmpty_** - returns true when the stack is empty otherwise returns false.

### **Stacks Concepts**

- **FILO** (First In Last Out) This means that the first item added in the stack will be the last item popped out of the stack.

- **LIFO** (Last In First Out) This means that the last item added to the stack will be the first item popped out of the stack.

![Stack](Pictures/Stack.png)

### **Push O(1)**

1. First, you should have the Node that you want to add.

2. Next, you need to assign the next property of that node to reference the same Node that top is referencing

3. Technically at this point, your new Node is added to your stack, but there is no indication that it is the first Node in the stack. To make this happen, you have to re-assign our reference top to the newly added Node.

### **Pop O(1)**

1. The first step of removing Node from the stack is to create a reference named temp that points to the same Node that top points to.

2. Once you have created the new reference type, you now need to re-assign the top to the value that the next property is referencing.

3. We can now remove the Node safely without it affecting the rest of the stack. Before we do that though you may want to make sure that you clear out the next property in your current temp reference.

4. Finally, we return the value of the temp Node that was just popped off.

&nbsp;

## Queues

Common terminology for a queue is

- **_Enqueue_** - Nodes or items that are added to the queue.
- **_Dequeue_** - Nodes or items that are removed from the queue.
- **_Front_** - This is the front/first Node of the queue.
- **_Rear_** - This is the rear/last Node of the queue.
- **_Peek_** - When you peek you will view the value of the front Node in the queue.
- **_IsEmpty_** - returns true when the queue is empty otherwise returns false.

### **Queues Concepts**

- **FIFO** (First In First Out) This means that the first item in the queue will be the first item out of the queue.

- **LILO** (Last In Last Out) This means that the last item in the queue will be the last item out of the queue.

![Queue](Pictures/Queue.png)

### **Enqueue O(1)**

1. First, we should change the next property of Node 4 to point to the Node we are adding. this means that we must change rear.next to the Node.

2. After we have set the next property, we can re-assign the rear reference to point to the Node. By doing this, it allows us to keep a reference of where the rear is, and we can continue to enqueue Nodes into the queue as needed.

### **Dequeue O(1)**

1. The first thing you want to do is create a temporary reference type named temp and have it point to the same Node that the front is pointing too.

2. Next, you want to re-assign the front to the next value that the Node front is referencing.

3. Now that we have moved front to the second Node in line, we can next re-assign the next property on the temp Node to null. We do this because we want to make sure that all the proper Nodes clear any unnecessary references for the garbage collector to come in later and clean up.

4. Finally, we return the value of the temp Node that was just removed.

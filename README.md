**OS LAB EXAM**

1. Question 1 : Counting semaphore for Process Synchronization
First created a new file **sem.c** which contains the definition and methods of structure semaphore like 						sem_init, sem_wait and sem_post. Then in **main.c** called seminit to initialize the semaphore table. Then in **defs.h** added definitions for all the methods. Added the prototype methods in **syscall.h** and **syscall.c** and in **sysproc.c** read arguements and call the kernel functions. In **user.h** and **usys.S** added linked the prototype functions. Created test file **synctest.c**. In **Makefile** added **sem.o** to **OBJS** and _synctest to **UPROGS**.

2.Question 2 : Memory Statistics and Address Translation
In **kalloc.c** added **nfree** to **kmem** and accordingly in **kree** added **nfree++** and in **kalloc nfree--**. Added **freepages** which returns nfree. In **vm.c** added va2pa which converts virtual address to actual address in RAM by calling **walkpgdir**. Then similarly to Question 1 added to defs.h and prototype methods to **syscall.h** and **syscall.c** and read arguements to call kernel functions in **sysproc.c**. In **user.h** and **usys.S** added linked the prototype functions. Created test file **memtest.c**. In **Makefile** added **_memtest** to **UPROGS**.
	

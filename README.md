# Lab03-ControlThreadsUsingWait-Notify
## Part 1
Control threads using wait/notify.
Download the project PrimeFinder. this is a program that calculates prime numbers beetween 0 and M (Control.MAXVALUE),concurrently, distributing the searching of them between n (Control.NTHREADS) independent threads.
Modify the application in such way that each t milliseconds of thread execution, all the threads stop and show the number of primes found until that moment. Then, you have to wait until press ENTER in order to resume the threads execution.Use the synchronization mechanisms given by java (wait y notify, notifyAll).

Note that:
The synchronized statement is used in order to get exclusive access to an object
The statement A.wait executed in a B thread set it to suspended mode (Independently that objective A is being used as 'lock') To resume, other active thread can resume B calling notify () to the object used as 'lock' ( in this case A)
The notify() statement, wakes the first thread  up who called wait() on the object
The notifyAll() instruction, wake  every thread up that are waiting for the object

# Pub-Sub-pattern
Yes, the Subject in the Observer Pattern is like a Publisher and the Observer can totally be related to a Subscriber and Yes, 
the Subject notifies the Observers like how a Publisher generally notify his subscribers. That’s why most of the Design Pattern books or
articles use ‘Publisher-Subscriber’ notion to explain Observer Design Pattern. But there is another popular Pattern called 
‘Publisher-Subscriber’ and it is conceptually very similar to the Observer pattern. The major difference between the (real)
‘Publisher-Subscriber’ pattern and the ‘Observer’ pattern is this
This means that the publisher and subscriber don’t know about the existence of one another. There is a third component, called broker or message broker or event bus, 
which is known by both the publisher and subscriber, which filters all incoming messages and distributes them accordingly. 
In other words, pub-sub is a pattern used to communicate messages between different system components without these components 
knowing anything about each other’s identity. how does the broker filter all the messages? Actually, there are several processes for 
message filtering. Most popular methods are: Topic-based and Content-based. Well, not going to further on that road, if you are interested, Wikipedia explained it well.
In the Observer pattern, the Observers are aware of the Subject, also the Subject maintains a record of the Observers. 
Whereas, in Publisher/Subscriber, publishers and subscribers don’t need to know each other. 
They simply communicate with the help of message queues or broker.
In Publisher/Subscriber pattern, components are loosely coupled as opposed to Observer pattern.
Observer pattern is mostly implemented in a synchronous way, i.e. the Subject calls the appropriate method of all its observers 
when some event occurs. The Publisher/Subscriber pattern is mostly implemented in an asynchronous way (using message queue).
Observer pattern needs to be implemented in a single application address space. On the other hand, the Publisher/Subscriber pattern 
is more of a cross-application pattern.

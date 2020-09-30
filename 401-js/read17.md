# Read 17: 9-30-2020

[README](/README.md)

### Review, Research, and Discussion

1. Given the examples of front-end events such as button
   click, window resize, form submit, etc, what are some examples of back-end events? [MBN](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events)

- Listening for event messages. parsing through json on a server call

- Error handling: When an error is triggered, the sever is told to do something. For example, an error is thrown and then an onerror callback is triggered.

- Closing event streams

2. Why are events sometimes better than asynchronous actions with callbacks? [Stack Overflow](https://stackoverflow.com/questions/2069763/difference-between-event-handlers-and-callbacks)

- Callback are under the control of the detecting process. meaning that when a button is clicked, a function call is made and then that data is sent back to the user.

- Event Handlers operate at one step removed. Opposed to sending a message back and waiting for a response, when clicked, the event is called and then that program runs independently. The event handler then goes on to the next event.

- **IMPORTANT** !!!! While the "event handler" pattern is more complex it is much more robust and less likely to hang when an action fails. It also makes for a more responsive GUI !!!!

<br>
<br>

3. What does an EventEmitter instance do?

- It triggers an event to which anyone can listen... Provide a framework for issuing events and subscribing to them

- `eventEmitter.on()
  function allows one or more functions to be attached to named events emitted by the object

"When the EventEmitter object emits an event, all of the functions attached to that specific event object are called synchronously in the order in which they are registered or attached to the even object" -[Medium](https://medium.com/technoetics/node-js-event-emitter-explained-d4f7fd141a1a)

**NOTE:** If we want to break the synchronous flow and switch to asynchronous mode then we can use setImmediate() or process.nextTick() methods:

```
const EventEmitter = require('events');
class MyEmitter extends EventEmitter {}
const myEmitter = new MyEmitter();
myEmitter.on('event', function(a, b) {
 setImmediate(() => {
   console.log('this happens asynchronously');
 });
 function cb(){
   console.log('processed in next iteration',a,b);
 }
 process.nextTick(cb)
 console.log('processed in first iteration',a,b);
});
myEmitter.emit('event', 'Technoetics', 'Club');
/**
* Output of the above Program:
* processed in first iteration Technoetics Club
* processed in next iteration Technoetics Club
* this happens asynchronously
*/
```

4. When is a program’s call stack, event queue, and event loop active?

- When ever the event is triggered

=====================================================

### [Open System Interconnection Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0)

TCP is a connection-oriented protocol, which means a connection is established and maintained until the application programs at each end have finished exchanging messages.

- breaks the app data into packets that networks can deliver, sends packets to and accepts packets from the network layer, manages flow control and provides error-free data transmission.

- session layer helps is authentication, authorization, session Management

Transport layer

# Message Queues
  - Queue server runs independently, and is tasked with routing events and messaging between clients.
    - 1. Any connected client can “publish” a message into the server.
    - 2. Any connected client can “subscribe” to receive messages by type.
  - asked with receiving any published message and then distributing it out to all connected and subscribed clients.



## What is a message?
  - is a package of information, categorized by queue and event
    - `queue` - Which general bucket does this message belong
      - *“Database Events”, “Filesystem Events”* “Network Events”
   - `event` - What event has happened
      - *“delete, add, update, connection lost, error”*
   - `payload` - data associated with the event
      - *“record id, record information, error text”*



## Real Time vs Queued Messaging
  - messages are simply brokered by the server. 
  - They come in, are processed and are immediately broadcast out to subscribers.
  -  Should a subscriber at any point lose connection with the server, any messages broadcast by the server will clearly be missed by the client. 
  - These are known as “Real Time” messaging systems.
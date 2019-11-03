# mqcquarie-code-challenge

For the given problem the following architecture is recommended.
1. Every workflow event is pushed to a message broking system like "Kafka" or "Rabbit MQ". 
2. The Event comes as a self contained message, containing the complete details of the event that happened in the workflow. 
3. All events are pushed on a single topic. Let's call it "wevents". 
4. These events are picked up on the other side and processed. 

Note
This code is more of pseudo code, rather an compilable running code. It is an attempt to get the design and structure right to achieve the given goal. 

# streaming-05-smart-smoker
# Steps taken to create smart-smoker
1. Define a function to clear queues when file has been run previously. 
2. Define a function to only show rabbitmq pop up when set to true. 
3. Set host and set queue names. 3 queues are needed for the smart-smoker to work. 
4. Define a function to create and send a message to the appropriate queue each execution. 
5. Create connection and channel within the rabbitmq server, also declare queue name and create durable queue. 
6. Define function to read from smart-smoker CSV and create message.
7. Use fstrings to create message from the data, first fstring pulls the timestamp from column one. 
8. Create 3 seperate messages that send the timestamp followed by either the smoker temp, food 1 temp, or food 2 temp. 
9. Set the producer to sleep for 30 seconds. 
10. Use the python idiom to call appropriate functions. 
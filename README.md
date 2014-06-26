json-to-rabbitmq
================

This example demonstrates how to send a message to RabbitMQ.

Step 1: download rabbit mq and install it
Step 2: enable admin console by following this walkthrough:
        http://www.thegeekstuff.com/2013/10/enable-rabbitmq-management-plugin/
Step 3: verify the admin web console http://localhost:15672
        go to exchanges tab - create an exchange called sales_exchange (use a form, leave other fields as are)
        go to queues tab - create a queue called sales_queue 
        click sales_exchange in exchange tab to edit it: 
        find a section Add binding from this exchange
        leave To queue and insert sales_queue 
        click Bind
Step 4: import the project
Step 5: run app
Step 6: make POST request using postman to send this data:
        {"ITEM_ID"= 001, "ITEM_NAME" = "Shirt", "QTY" = 1, "PRICE" = 20}
Step 7: Success: go to queuess and notice the increased number of messages in sales_queue (the specific message can be retrieved by clicking on sales_queue in Get messages section)
        
        

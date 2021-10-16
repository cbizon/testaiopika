This is a simple test of the aio-pika library based on their documentation.

First, install aio-pika
`pip install -r requirements.txt` 

Run rabbitmq 
`docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.9-management`

Then run the consumer:
`python consumer.py`

It'll block

Then run the producer:
`python producer.py`

You'll see a message printed on the consumer, and both will exit.

producer.py and consumer.py are taken from https://aio-pika.readthedocs.io/en/latest/quick-start.html

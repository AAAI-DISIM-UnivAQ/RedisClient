# RedisClient
Prolog library that allows DALI MAS agents to send messages to [Redis](http://redis.io).
##Configuration##
You can modify these lines to configure redis_client.pl:
- :- assert(connect_conf('127.0.0.1':6379, 'MAS_DATA')). -> '127.0.0.1':6379 and 'MAS_DATA' are respectively the port and the Redis channel the agents send messages to (you can change both).

##Instructions##
- To use redis_client.pl, you have to include it inside agents code.
- To send a message to Redis, you have to write this line inside agents code: mas_send(content_of_message) .

##Do you need to send messages from Redis to MAS too?##
See also Redis2LINDA-stringESE: https://github.com/AAAI-DISIM-UnivAQ/Redis2LINDA-stringESE

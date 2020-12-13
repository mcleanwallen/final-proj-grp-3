Create a customer
Run the command and look for the container ids for redis and kafka: docker ps
Look for the customer you created in Redis (you should see JSON with customer data)
From the terminal type: docker exec -it [rediscontainername] redis-cli (example: docker exec -it myrepo_redis_1 redis-cli)
From the terminal type: keys **
You will see the list of all the Redis tables
Type: zrange Customer 0 -1

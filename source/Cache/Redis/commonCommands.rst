Common Commands Of Redis
===========================

Get the time to live for a key ::

 TTL key

Listen for all requests received by the server in real time ::

 MONITOR
 
 redisc-cli MONITOR > redis-monitor.log

Connect Remote Server ::

 redis-cli -h host -p port

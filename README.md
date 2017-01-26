# kafka-bokeh-dashboard
Bokeh dashboard that plots incoming Kafka events!

## Run the demo:
Go into your Kafka directory and run
```
$ bin/zookeeper-server-start.sh config/zookeeper.properties
```
Then from the same directory, run
```
$ bin/kafka-server-start.sh config/server.properties
```
Now move to your kafka-bokeh-dashboard
```
$ python producer/main.py
```
Then start a bokeh session
```
$ bokeh serve
```
And start the consumer
```
$ python consumer/main.py
```
This should automatically open a new browser window and you should see the plot update.

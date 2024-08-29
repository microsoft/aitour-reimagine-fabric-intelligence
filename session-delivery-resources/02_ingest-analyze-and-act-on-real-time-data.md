# Ingest, analyze and act on real-time data

## Demo Intro

In this scenario, we am going to represent Contoso, a major retailer with data streaming from all point-of-sale systems around the world, which produces millions of signals that we want to understand as quickly as possible.

Since everything starts with data ingestion, this demo is going to show _Connectors_ and _Data Sources_, and how easy it is to bring in data from a wide range of sources into Real-Time Hub. In the demo, we are going to connect to Confluent Kafka, where the point-of-sale system data is streaming in from.

## SHOW REAL-TIME HUB

![Show Real-Time Hub](./imgs/02_show_real_time_hub.png)

Back in the Real-Time hub, we can see a wide range of streams from across the whole organization. We can see information about where the stream is located, who's the owner, and whether or not it's endorsed.

Here we select the "Get events" button to start importing data.

![Get Events](./imgs/02_get_events.png)

## SHOW CONNECTORS / DATA SOURCES

Of course, I can also leverage our wide range of connectors to bring in even more data. 

Whether my data is streaming from Amazon Kinesis, Google Pub/Sub, or in this case, I'm going to connect to Confluent Kafka, which is where my point-of-sale system data is streaming in from. 

![Show Connectors](./imgs/02_show_connectors.png)

## CREATE CONNECTION

I'm going to create a quick connection and specify the information about the event stream, which is where we save it into. 

![Create Connection](./imgs/02_create_connection.png)

On the connectors page, select the Kafka connector.

![Select Kafka Connection](./imgs/02_select_kafka_connection.png)

Then you will configure the connection. Specify a topic, a consumer group. Then select the Workspace the connection will be saved into, and provide an Eventstream name to start ingesting the data.

![Configure Kafka Connection](./imgs/02_configure_kafka_connection.png)

Just like that, it can create the connection, and now the data is coming into the Real-Time hub.

But also from this experience, I can open the event stream and actually transform and process the data a little bit more.

![Open in Eventstreams](./imgs/02_open_eventstream.png)

# STREAM EDITOR

In the event stream editor, I can see on the left-hand side, I have the source. 

![Stream Editor Source](./imgs/02_stream_editor_source.png)

On the right-hand side, I have the transformations and the destinations that I can connect the stream to. 

You can see, I have a wide range of operations and destinations. 

![Stream Editor Destinations](./imgs/02_stream_editor_operations.png)

# LOAD DATA INTO EVENTHOUSE

Since I know I'm going to do further analytics on it, I'm going to load it directly into an Eventhouse in KQL database that's already within my organization, so the data is ready for me to do a little bit more. 

![Load Data into Eventhouse](./imgs/02_load_data_into_eventhouse.png)

We can fast-forward ahead to something a little bit more complicated. 

# SHOW COMPLEX TRANSFORMATIONS

You could see some of the power, the ability to route to many destinations. 

![Show Complex Transformations](./imgs/02_show_complex_transformations.png)

And in this case, I've done some aggregations, some filtering, and then ultimately used the new derived stream endpoint. 

![Show Derived Stream Endpoint](./imgs/02_show_derived_stream_endpoint.png)

# CONCLUSION

What this does, is it takes the transformations I've already applied and published them back to the Real-Time hub so others can use that data without having to do the transformations themselves. 

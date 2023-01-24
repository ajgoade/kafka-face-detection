# Realtime face detection using Kafka video streaming 
- Face detection using Kafka | OpenCV | Centerface | Flask
- Running HPF DF Streams (DFaaS)

## Installation
- Install the dependencies:
```python
  $ pip install -r requirements.txt
```
## HPE DF Streams DFaaS setup
- Create the Topic used in the consumer and producer.  Currently kfd-altersense
```
  $ sudo ssh -i <ssh pem file> <DFaaS Endpoint> -L 9092:localhost:9092 -N -f
```
## Finally

- Run kafka producer:
```
  $ python producer.py
```

- And run kafka consumer:
```
  $ python consumer.py
```

Your app should now be running on ***localhost:5000***

## Reference
```
- http://betterdatascience.com/how-to-install-apache-kafka-using-docker-the-easy-way/
- https://github.com/akmamun/kafka-python-camera-stream
```

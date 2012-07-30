# JMeter-Rabbit-AMQP #
==========

A [JMeter](http://jmeter.apache.org/) plugin to publish & consume messages from [RabbitMQ](http://www.rabbitmq.com/) or any [AMQP](http://www.amqp.org/) message broker.

Hooking it into JMeter

1. Copy the JMeterAMQP.jar from target\dist to jmeter\lib\ext 
2. Copy the amqp-client-2.6.1.jar from JMeter-Rabbit-AMQP\lib to jmeter\lib
    - if you don't you will get an exception when trying to add the Consumer in JMeter
      saying it can't find the ShutdownException

If you would like to build it yourself you can. This JMeter sampler builds using Ant.

Installing Ant on Windows:

1. Install the Java Development Kit (JDK) http://www.oracle.com/technetwork/java/javase/downloads/index.html
2. Install Ant http://ant.apache.org/bindownload.cgi
   - Unzip apache-ant-<ver>-bin.zip to c:\java\Ant
   - Add bin folder to path
        WARNING: Copy the tools.jar file from its location in the JDK to the JRE<ver>\Lib folder; or it will not work.

Installing Ant on Ubuntu

1. sudo apt-get install sun-java6-jdk sun-java6-jre
2. sudo apt-get install ant
   - you may havet o set up JAVA_HOME env var if it has not done it for you

Building using Ant

1. Build using the command >ant clean package




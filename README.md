<p align="center">
  <img src="service-bus.png" alt="Microsoft Azure Service Bus" width="100"/>
</p>

|Build/Package|Status|
|------|-------------|
|master|[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.microsoft.azure/azure-servicebus/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.microsoft.azure/azure-servicebus)|

# Moved
All new work on SDK is happening in the repository https://github.com/Azure/azure-sdk-for-java/tree/master/sdk/servicebus. This repository is only to address any issues found in versions 1.2.x. And master1.0 is the branch corresponding to versions 1.2.x. Both dev and master branches moved to the new repository.

# Microsoft Azure Service Bus Client for Java

This is the next generation Service Bus Java client library that focuses on Queues & Topics. If you are looking for Event Hubs, follow this [link](https://github.com/azure/azure-event-hubs-java).

Azure Service Bus is an asynchronous messaging cloud platform that enables you to send messages between decoupled systems. Microsoft offers this feature as a service, which means that you do not need to host any of your own hardware in order to use it.

Refer to [azure.com](https://azure.microsoft.com/services/service-bus/) to learn more about Service Bus. And package can be downloaded from [Maven](http://search.maven.org/#search%7Cgav%7C1%7Cg%3A%22com.microsoft.azure%22%20AND%20a%3A%22azure-servicebus%22)

## How to provide feedback

See our [Contribution Guidelines](./.github/CONTRIBUTING.md).

## Known issues

## FAQ
### Where is the API document?
Click [here](https://docs.microsoft.com/en-us/java/api/overview/azure/servicebus/clientlibrary).

### Where can I find examples that use this library?

The samples are located in this repo. [Java Samples](https://github.com/Azure/azure-service-bus/tree/master/samples/Java).

### Can I manage Service Bus entities with this library?

Only rules management of subscription will be supported in this client library. This library focuses on Azure Service Bus Data Plane functionalities (e.g. send, receive).

The standard way to manage Azure resources is by using [Azure Resource Manager](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-overview). In order to use functionality that previously existed in the azure-servicebus Java library, this is [Azure Service Bus Management Library](https://mvnrepository.com/artifact/com.microsoft.azure/azure-mgmt-servicebus) which is available on Maven. And this is the [API document](https://docs.microsoft.com/en-us/java/api/com.microsoft.azure.management.servicebus). This management library will enable use cases that dynamically create/read/update/delete resources.

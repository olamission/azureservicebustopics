sudo apt-get update &&   sudo apt-get install -y dotnet-sdk-7.0

curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash

dotnet new console

dotnet add package Azure.Messaging.ServiceBus

copy and paste from https://learn.microsoft.com/en-us/azure/service-bus-messaging/service-bus-dotnet-how-to-use-topics-subscriptions?tabs=connection-string

az login --use-device-code

dotnet build

dotnet run

az servicebus topic show --resource-group=1-fa263dde-playground-sandbox --namespace-name=AZservicebustopics122333 -n=my-topic  --output=json ---------doesnt work very well as in updates

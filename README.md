# Checkout and Build

To checkout the project and build from source, provide the following command
```
git clone https://github.com/akiladevimrm/AOTVendorInvoicing.git
```

# Pre-requisites:
```install docker-compose https://docs.docker.com/compose/install/```
```Java```

# How to start VendorInvoicing application
Pre-built docker image is already available in docker hub registry. 
```
$docker run -i -t --name invoice_app --network=docker_my-kafka-network-1 akiladevi26/invoiceapp:1.0
```
This starts the application in command line which continously polls for invoice data in the file system and publishes the invoices data to kafka.

# Other Dependencies
Place the keystore and truststore files under resources folder.
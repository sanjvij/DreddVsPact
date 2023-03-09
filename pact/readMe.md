
# Run Pact Server

* run `docker compose up -d` to start a local PactBroker.


# order-consumer API  Execute Tests and generate contract 


## Execute tests and generate the "contract" locally

*  run `./gradlew test` to execute tests and generate the "contract" locally.

* run `./gradlew pactPublish` to publish the "contract" to the local PactBroker.

## check with provider if Can deploy the consumer app

*  run `./gradlew canIDeploy` that will connect to the local PactBroker and be successful if provider has verified the contract 



# order-provider API  Execute Tests and generate contract 

* run `./gradlew test` to
    *  download the "contract" from the local PactBroker.
    *  execute tests accordingly.
    *  publish the result of the tests back to the local PactBroker.

## check with broker if Can deploy the provider app

  *  run `./gradlew canIDeploy` that will connect to the local PactBroker and be successful if provider has verified the "contract".

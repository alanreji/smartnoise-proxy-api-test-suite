# smartnoise-proxy-api-test-suite

**Table of Contents**

<!--ts-->
   * [Prerequisites](#prerequisites)
   * [Usage](#usage)
<!--te-->

#### Prerequisites

Postman installed on your machine (download and installation instructions available at https://www.postman.com/downloads/)

`sqlite-smartnoise-proxy` has to be running.

#### Usage

Open Postman and import the provided collection file for the SmartNoise SDK API testing suite.
Configure the environment variables in Postman to include the server address and API key header, and the proxy address and port for the MITM proxy.
Run the API testing suite in Postman. The suite includes test cases for basic aggregate queries such as `count()` and `sum()`, as well as invalid queries that should be rejected.
Observe the results in Postman and the MITM proxy console. The queries should be routed through the MITM proxy and the valid queries should be processed by the database while the invalid queries are rejected.

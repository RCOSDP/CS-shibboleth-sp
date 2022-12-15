## Overview
This Docker image is Apache 2.4 with Shibboleth SP 3.4.0 installed running on Rocky Linux 8.

This image can be used as a base image overriding the configuration with local changes.

Ports 80 and 443 are exposed for traffic.

## Logs
Logs for httpd and shibd have been configured to output to the console so that Docker's logging facilities are supported. Each of these logs have been prefaced with an identifier that indicates the type of entry being outputted: `httpd-error`, `httpd-combined`, `sp-shibd`, `sp-native`, `sp-transaction`, `sp-sign`, etc.

## Building

From source:

```
$ docker build --tag="<org_id>/shibboleth-sp" github.com/RCOSDP/CS-shibboleth-sp
```

## Author

  * John Gasper (<jgasper@unicon.net>)
  * Research Center for Open Science and data platform(RCOS) in National Institute of Informatics, Japan


## LICENSE

Copyright 2016 Unicon, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

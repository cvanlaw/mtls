# mTLS

An example of how to implement mutual TLS (mTLS) between two dotnet services. We'll implement mTLS two different ways
1. mTLS built into the service itself
2. mTLS via Istio sidecar

## Requirements

* All infrastructure should be immutable and implement via infrastructure as code.
* All services should be containerized
* Services and infrastructure should be deployed via a CI pipeline - probably GitHub Actions
* Everything should be able to be torn down and stood back up via automation. Using a CI pipeline implies this, but stating it explicitly

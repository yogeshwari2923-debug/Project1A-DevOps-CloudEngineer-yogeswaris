
# Deployment Strategies

## Blue-Green

* Two environments: Blue (live), Green (new)
* Switch traffic instantly

## Canary

* 10% → 50% → 100% rollout
* Monitor:

  * Error rate < 5%
  * Latency stable

## Rollback

* Trigger:

  * Errors >5%
  * CPU spike
* Action:

  * revert to previous version

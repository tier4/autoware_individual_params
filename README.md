# autoware_individual_params

This repository stores parameters that are different from each vehicle.

## Rational

The parameters were originally managed in `launcher` repository.
Why we manage them in a separate repository are:

- Parameter maintainers don't require write-access to `launcher` repository.
- To rollback only parameters independently from `launcher`.

## Directory Structure
<pre><code>
individual_params/
├── config
│    └ default # vehicle id
│       ├ aip_x1 # sensor id
│       │ ├ sensor_kit_calibration.yaml
│       │ ├ sensor_calibration.yaml
│       │ └ ... # other sensor settings yaml
│       └ ...
│
├ CMakeLists.txt
└ packages.xml
</code></pre>

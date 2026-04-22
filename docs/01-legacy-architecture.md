# Legacy CICS/COBOL Architecture Overview

This document summarizes the structure of the original `cics-genapp` application from the `cicsdev/cics-genapp` repository.

- COBOL programs in `base/src/*.cbl` implement customer, policy, policy-version, statistics, and setup flows.
- Copybooks such as `lgcmarea.cpy` and `lgpolicy.cpy` define the common data structures passed between programs.
- BMS map `ssmap.bms` defines the terminal screens used for customer and policy maintenance.
- VSAM KSDS files (`ksdscust.txt`, `ksdspoly.txt`) back the CUSTOMER and POLICY records.

These elements are mapped to Java microservices in `02-target-architecture.md`.

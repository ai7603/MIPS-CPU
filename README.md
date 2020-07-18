# MIPS-CPU
CPU for 5-stage pipeline, and trying to add MMU, Cache, branch predictor and etc

### 5-stage pipeline CPU for MIPS

```mermaid
graph LR;
PC-->Fetch-->Decode-->Execute-->Memory-->WriteBack
Controller-->Execute
Controller-->Memory
Controller-->WriteBack
Decode-->Controller
```

Consider divide Decode as two stages: Decode and Registers Read, which maybe useful to Cache and Branch predictor.


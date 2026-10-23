# Progress Log

Repository: `robotic-inference-optimization`

Remote: https://github.com/7henghhhy/robotic-inference-optimization

## Current development environment

- Operating system: macOS 26.6.2
- Architecture: Apple Silicon `arm64`
- Python: 3.14.7
- Git: 2.54.0
- Current use: Python, MuJoCo/robosuite preparation, CPU/MPS experiments, documentation
- CUDA status: not applicable on this Mac; CUDA integration is deferred to the Y7000P

## Day 1 — Repository setup

### Completed

- Created the local project skeleton.
- Defined `Reach` plus a scripted controller as the minimum deliverable.
- Defined fixed-seed evaluation, success criteria, failure logs, and latency stages.
- Marked BC, Lift, ACT/VLA, and CUDA integration as time-controlled extensions.

### Not yet verified

- MuJoCo installation.
- robosuite installation and version.
- Reach environment reset/step/render.
- Observation and action shapes.
- Scripted controller success rate.
- Any policy or latency result.

### Next project milestone

When Project B starts at W7/D43, run the smallest MuJoCo or robosuite example and record the exact environment versions before writing a controller.

### Evidence policy

Do not add success rates, step counts, latency values, or policy comparisons until they are produced by a reproducible command with fixed seeds and saved raw output.

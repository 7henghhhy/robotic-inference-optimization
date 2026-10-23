# Robotic Inference Optimization

MuJoCo robotic manipulation with lightweight imitation learning and end-to-end inference latency analysis.

## Project goal

Build a small, reproducible robotic manipulation system that measures where inference latency comes from under limited compute:

- MuJoCo or robosuite `Reach` baseline
- deterministic scripted controller
- fixed seeds, evaluation cases, success criteria, and failure logs
- small state-vector Behavior Cloning policy when time permits
- latency breakdown for observation, preprocessing, policy inference, and action output
- optional CUDA image preprocessing comparison using the sibling `cuda-robotics-vision` project

The minimum deliverable is a working and measurable `Reach` system. `Lift`, visual policies, ACT, and VLA experiments are optional extensions.

## 12-week milestone

| Milestone | Status |
|---|---|
| Repository and experiment log | In progress |
| MuJoCo/robosuite environment check | Not started |
| Reach scripted controller | Not started |
| Fixed-seed evaluation | Not started |
| Demonstration data and replay | Not started |
| State-vector Behavior Cloning | Optional |
| End-to-end latency breakdown | Not started |
| CUDA preprocessing integration | Optional, requires Y7000P |
| Technical report and reproducibility guide | Not started |

## Repository layout

```text
src/          environment wrappers, controllers, policies, and timing code
tests/        success criteria, data checks, and replay tests
configs/      seed, task, evaluation, and model configuration
experiments/  runnable experiment entry points
data/         small metadata only; large/raw data stays local or external
reports/      figures, tables, and technical report drafts
progress.md   dated learning and experiment log
```

## Environment policy

The current development machine is an Apple Silicon Mac. It is suitable for MuJoCo/robosuite simulation, Python development, CPU/MPS experiments, and documentation. CUDA integration and RTX 4060 measurements must be run on the Lenovo Y7000P.

Do not call a state-vector policy a vision policy. Keep observation type, preprocessing, training configuration, evaluation seeds, and success criteria explicit before comparing results.

## Related resources

- [MuJoCo documentation](https://mujoco.readthedocs.io/en/stable/)
- [MuJoCo GitHub](https://github.com/google-deepmind/mujoco)
- [robosuite installation](https://robosuite.ai/docs/installation.html)
- [robosuite basic usage](https://robosuite.ai/docs/basicusage.html)
- [robosuite benchmarking](https://robosuite.ai/docs/algorithms/benchmarking.html)
- [Gymnasium Env API](https://gymnasium.farama.org/api/env/)
- [LeRobot imitation learning](https://huggingface.co/docs/lerobot/il_robots)

## Current status

See [progress.md](progress.md). No task success rate, policy result, or latency number has been recorded yet.

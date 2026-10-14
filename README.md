# Awesome-Robotics-Scientific-Computing

# Top Robotics Scientific Computing Tools Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Rigid Body Dynamics, Optimization & Motion Planning*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Robotics Scientific Computing**. These tools provide the numerical foundations for modern robotics — rigid body dynamics algorithms, nonlinear optimization solvers, physics simulation engines, motion planning libraries, and factor graph frameworks — enabling researchers and engineers to model, control, and verify complex robotic systems.

**Examples** include Pinocchio, Drake, CasADi, MuJoCo, SymPy, SciPy, OMPL, GTSAM, JAX-MD, and Project Chrono (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom algorithm development, and transparent scientific computing — ideal for robotics researchers, control engineers, and developers building the numerical backbone of autonomous systems.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[MathWorks Robotics System Toolbox](https://www.mathworks.com/products/robotics.html)**  
  MATLAB/Simulink-based environment for robot modeling, simulation, and control algorithm development with Gazebo co-simulation support.

- **[Wolfram Mathematica](https://www.wolfram.com/mathematica/)**  
  Symbolic and numerical computation platform with robotics-specific libraries for kinematics, dynamics, and control design.

- **[Altair MotionSolve](https://altair.com/motionsolve)**  
  Commercial multibody dynamics simulation for robot design validation and optimization.

- **[Siemens Simcenter Amesim](https://plm.sw.siemens.com/en-US/simcenter/systems-simulation/amesim/)**  
  Multi-domain system simulation for mechatronic and robotic system design.

- **[Ansys Motion](https://www.ansys.com/products/structures/ansys-motion)**  
  Multibody dynamics simulation for rigid and flexible body robotics applications.

- **[COMSOL Multiphysics](https://www.comsol.com/)**  
  Multiphysics simulation platform with structural mechanics and rigid body dynamics modules.

- **Commercial Optimization Solvers** — Gurobi, CPLEX, and MOSEK for convex and mixed-integer optimization in robotics applications.

## Open-Source GitHub Projects

- **[Pinocchio](https://github.com/stack-of-tasks/pinocchio)**  
  The reference library for **state-of-the-art rigid body dynamics algorithms** for poly-articulated systems, based on revisited Roy Featherstone algorithms. Actively developed by the Willow team at Inria, Paris . Provides analytical derivatives of rigid body dynamics, constrained articulated body dynamics, and differentiable collision detection. Widely used by Crocoddyl, TSID, HPP, Jiminy, and ocs2. BSD-2-Clause licensed.

- **[Drake](https://github.com/RobotLocomotion/drake)**  
  MIT's **model-based design and verification toolbox** for robotics, with core development now led by Toyota Research Institute . Combines physics simulation, optimization, and control design in one framework with heavy emphasis on optimization-based design/analysis. Recently added GPU-accelerated async-coupling for interactive simulation . BSD-3-Clause licensed.

- **[CasADi](https://github.com/casadi/casadi)**  
  **Symbolic framework for nonlinear optimization and optimal control** with automatic differentiation in forward and reverse modes on sparse matrix-valued computational graphs . Supports self-contained C-code generation and interfaces with SUNDIALS, IPOPT, and other state-of-the-art solvers. Usable from C++, Python, or MATLAB/Octave. The foundation for many robotics trajectory optimization frameworks. LGPL licensed.

- **[MuJoCo](https://github.com/google-deepmind/mujoco)**  
  **The gold standard for contact-rich manipulation and RL research.** Free and open-source physics engine from Google DeepMind with a depth-first kinematic tree structure for efficient articulated body dynamics . Excels at contact simulation and fast computation for reinforcement learning. Apache 2.0 licensed. Includes MuJoCo Menagerie for high-quality robot models.

- **[SciPy](https://github.com/scipy/scipy)**  
  **The fundamental numerical library for Python scientific computing** . Provides optimization, integration, interpolation, signal processing, linear algebra, statistics, and differential equation solvers — the numerical backbone for most robotics research code. BSD licensed.

- **[SymPy](https://github.com/sympy/sympy)**  
  **Symbolic mathematics and computer algebra library** for Python . Enables exact symbolic derivation of kinematic and dynamic equations, Jacobian computation, and equation simplification for robot modeling. BSD licensed.

- **[OMPL (Open Motion Planning Library)](https://github.com/ompl/ompl)**  
  **The leading sampling-based motion planning library** with implementations of PRM, RRT, EST, SBL, KPIECE, and many variants . OMPL 2.0 adds constrained motion planning, asymptotically optimal planners, lazy planning, and integration with **VAMP** for SIMD-accelerated collision checking reaching kilohertz solution rates . Used by MoveIt, CoppeliaSim, Nav2, and Tesseract. BSD licensed.

- **[GTSAM](https://github.com/borglab/gtsam)**  
  **Factor graphs for sensor fusion in robotics and computer vision** — the underlying computing paradigm for SLAM, visual odometry, and structure from motion . Uses Bayes networks rather than sparse matrices to optimize for the most probable configuration or optimal plan. BSD licensed. The reference library for factor graph optimization in robotics.

- **[JAX-MD](https://github.com/google/jax-md)**  
  **Differentiable physics framework** for molecular dynamics and beyond . Simulations are differentiable functions, enabling meta-optimization over entire trajectories. Scales to hundreds of thousands of particles on a single GPU using spatial partitioning primitives. Neural network interactions can be integrated directly into simulations. Apache 2.0 licensed.

- **[Project Chrono](https://github.com/projectchrono/chrono)**  
  **Open-source multi-physics simulation infrastructure** for multibody dynamics, finite element analysis, vehicle dynamics, and fluid-solid interaction . Chrono::Vehicle provides template-based wheeled and tracked vehicle modeling. PyChrono wraps the library for Python. BSD-3-Clause licensed.

- **[PyBullet](https://github.com/bulletphysics/bullet3)**  
  Python module for physics simulation, robotics, and deep reinforcement learning built on the Bullet Physics SDK. Fast, easy to install, and widely used for RL benchmarks. MIT licensed.

- **[DART (Dynamic Animation and Robotics Toolkit)](https://github.com/dartsim/dart)**  
  Research-focused C++20 physics engine for robotics, animation, and machine learning with Python bindings . Provides kinematics, dynamics, collision detection, and motion planning. BSD-2-Clause licensed.

- **[Brax](https://github.com/google/brax)**  
  Google's **differentiable physics engine for JAX**. Enables gradient-based optimization and massively parallel RL on TPUs/GPUs . Apache 2.0 licensed.

- **[Crocoddyl](https://github.com/loco-3d/crocoddyl)**  
  **Model predictive control for complex robotics platforms** built on Pinocchio . Implements differential dynamic programming (DDP) and its variants for optimal control. BSD-3-Clause licensed.

- **[TSID](https://github.com/stack-of-tasks/tsid)**  
  **Task Space Inverse Dynamics QP** solver for whole-body robot control, built on Pinocchio . BSD-2-Clause licensed.

- **[HPP (Humanoid Path Planner)](https://github.com/humanoid-path-planner/hpp-doc)**  
  SDK implementing motion planners for humanoids and other robots, built on Pinocchio . BSD licensed.

- **[OCS2](https://github.com/leggedrobotics/ocs2)**  
  **Optimal Control for Switched Systems** toolbox from ETH Zurich for legged robot locomotion and manipulation. Built on Pinocchio and CasADi . BSD-3-Clause licensed.

- **[RoboPlan](https://github.com/Sea-Snell/RoboPlan)**  
  Modern robot motion planning library based on Pinocchio, built in C++ with Python bindings (successor to PyRoboPlan) .

### Additional Strong Open-Source Options

- **[ProxSuite-NLP](https://github.com/Simple-Robotics/proxsuite-nlp)** — Primal-dual augmented Lagrangian solver for nonlinear programming on manifolds, built on Pinocchio .
- **[Aligator](https://github.com/Simple-Robotics/aligator)** — Versatile and efficient framework for constrained trajectory optimization .
- **[Jiminy](https://github.com/duburcqa/jiminy)** — Physics simulator based on Pinocchio for robotics reinforcement learning .
- **[Simple Simulator](https://github.com/Simple-Robotics/simple)** — Simulation Made Simple, lightweight robotics simulator from the Pinocchio ecosystem .
- **[PyRoboPlan](https://github.com/Sea-Snell/PyRoboPlan)** — Educational Python library for manipulator motion planning using Pinocchio bindings .
- **[VAMP](https://github.com/KavrakiLab/vamp)** — SIMD-accelerated collision checking and forward kinematics for motion planning, integrated into OMPL 2.0 .
- **[CAPT](https://github.com/KavrakiLab/CAPT)** — SIMD-based point cloud collision checking for motion planning .
- **[Newton (Physics)](https://github.com/newton-physics/newton)** — GPU-accelerated physics simulation engine built on NVIDIA Warp, specifically targeting roboticists .
- **[mjlab](https://github.com/mujocolab/mjlab)** — Isaac Lab API powered by MuJoCo-Warp for RL and robotics research .

**Frameworks for building custom systems**: Combine **Pinocchio** for rigid body dynamics, **CasADi** for nonlinear optimization, **Drake** for model-based design and verification, **MuJoCo** for contact-rich simulation, **OMPL** for motion planning, and **GTSAM** for sensor fusion to build a complete robotics scientific computing stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Robotics scientific computing tools are mathematical and computational frameworks — validation against real-world robot behavior is essential before deployment. Incorrect dynamics models or optimization formulations can produce unsafe control outputs.
- Self-hosted open-source solutions require proper numerical validation, solver tuning, and understanding of their mathematical foundations.

---

**Made for robotics researchers, control engineers, graduate students, and developers building the numerical foundations of autonomous systems.**  
Let's make robotics scientific computing more open, rigorous, and accessible.

export const PROJECT_CASE_STUDIES: ProjectCaseStudy[] = [
  {
    id: "center-of-mass-and-velocity-calculator",
    code: "PRO-17 // AI-01",
    title: "Center of Mass & Velocity Calculator: Vectorized Multi-Body Kinematics & 3D Spatial Simulator",
    category: "ai-ml",
    categoryLabel: "AI & Machine Learning",
    year: "2024",
    status: "Completed",
    imageUrl: "centerofmass1.webp",
    images: [
      "centerofmass1.webp",
      "centerofmass2.webp"
    ],
    summary:
      "Vectorized scientific computing engine implemented in Python and NumPy to simulate discrete N-body mechanical systems, calculating spatial center-of-mass coordinates and aggregate kinematic velocity vectors with instant 2D/3D scatter and quiver vector field projections in sub-millisecond execution times.",
    overview:
      "Center of Mass and Velocity Calculator is a scientific computing and computational physics engine engineered to model multi-particle Newtonian mechanical systems. Designed to eliminate manual calculation bottlenecks and rounding inaccuracies in academic physics research, the system resolves spatial center-of-mass coordinates and kinematic velocity vectors for arbitrary N-body configurations. Rather than relying on slow iterative loops, the core computation leverages vectorized NumPy array broadcasting and matrix transpositions, executing weighted coordinate summations across three spatial dimensions simultaneously. The simulation engine couples analytical reduction with dual-mode visualization toolkits, generating synchronized 2D planar scatter plots, 3D isometric spatial projections, and directional quiver vector fields to render particle velocity trajectories. Deployed as an interactive terminal application and cloud-executable Google Colab notebook, the system guarantees 64-bit floating-point accuracy with zero truncation drift, validating multi-body mechanics against analytical proofs in sub-millisecond runtimes.",
    challenge:
      "Manual physics modeling of discrete multi-body systems is prone to compounding floating-point rounding errors and dimensional projection mistakes across three-dimensional axes. In software implementations, naive iterative Python loops scale poorly as particle counts expand, while generating synchronized 2D orthographic projections and 3D isometric vector quiver fields simultaneously creates visualization overhead and axis alignment inconsistencies in non-vectorized execution environments.",
    architectureSummary:
      "NumPy vectorized array broadcasting & dot-product reduction + Matplotlib 2D Cartesian scatter & quiver plotting + Axes3D isometric spatial projection engine + Interactive CLI & Google Colab runtime",
    objectives: [
      "Eliminate manual computation errors by implementing vectorized weighted summation routines for arbitrary N-body mechanical systems.",
      "Calculate exact center-of-mass Cartesian coordinates [X, Y, Z] with zero numerical truncation drift using 64-bit floating-point precision.",
      "Compute resultant system linear velocity vectors [Vx, Vy, Vz] from individual particle kinematic states based on momentum conservation.",
      "Render synchronized 2D planar scatter plots and 3D isometric coordinate views to visually ground multi-particle spatial relationships.",
      "Generate directional 2D and 3D vector quiver fields to simulate velocity vector trajectories originating from Cartesian reference origins.",
      "Deliver sub-millisecond calculation execution times within interactive terminal CLI and cloud-hosted Google Colab environments."
    ],
    features: [
      {
        title: "Vectorized Linear Algebraic Reduction",
        description:
          "Executes array broadcasting and axis-wise dot products via NumPy to compute mass-weighted spatial coordinates and velocity vectors without loop overhead.",
        badge: "Sub-ms Vector Engine"
      },
      {
        title: "Arbitrary N-Body Dynamic Configuration",
        description:
          "Dynamically aggregates user-defined scalar masses and multi-dimensional spatial vectors for any number of discrete physical particles across Cartesian axes.",
        badge: "Dynamic N-Particle"
      },
      {
        title: "Dual-Mode 2D & 3D Spatial Coordinate Mapping",
        description:
          "Projects particle distributions using continuous Viridis colormaps alongside a distinct high-contrast red marker anchoring the system center of mass.",
        badge: "Axes3D Projection"
      },
      {
        title: "Kinematic Velocity Quiver Vector Fields",
        description:
          "Renders directional vector arrows displaying individual velocity components and aggregate system momentum vectors across 2D planar and 3D spatial coordinate planes.",
        badge: "Quiver Field Engine"
      },
      {
        title: "Interactive Terminal CLI Workflow",
        description:
          "Provides an ergonomic terminal navigation loop enabling rapid switching between center-of-mass analysis, velocity evaluations, and safe process termination.",
        badge: "Interactive CLI"
      },
      {
        title: "Cloud-Executable Google Colab Integration",
        description:
          "Preconfigured interactive Jupyter notebook featuring verified cell execution outputs, visual inline plot caching, and zero-setup browser computation.",
        badge: "Google Colab Ready"
      }
    ],
    pipelineSteps: [
      {
        step: "01. Parameter Ingestion & Tensor Assembly",
        detail:
          "Parse user-defined particle count, scalar mass values, and Cartesian coordinate or velocity tuples into structured 2D NumPy array matrices.",
        latencyOrMetric: "0.2ms Matrix Assembly"
      },
      {
        step: "02. Scalar Mass Normalization & Reduction",
        detail:
          "Execute axis-0 summation across the mass vector to determine total multi-body system mass M_total with zero-division validation.",
        latencyOrMetric: "0.05ms Scalar Sum"
      },
      {
        step: "03. Vectorized Dot-Product Kinematic Scoring",
        detail:
          "Compute transposed dot product between position or velocity matrices and mass arrays, normalizing by total mass to derive exact coordinate vectors.",
        latencyOrMetric: "0.1ms Vector Reduction"
      },
      {
        step: "04. Matplotlib 2D Orthogonal Projection",
        detail:
          "Generate 2D Cartesian scatter plot or quiver vector field with Viridis color spectrum mapping and highlighted center-of-mass focal point.",
        latencyOrMetric: "18ms 2D Canvas Render"
      },
      {
        step: "05. Axes3D Isometric Spatial Mesh Generation",
        detail:
          "Initialize 3D isometric axis projection via mpl_toolkits.mplot3d, rendering multi-particle spatial coordinates or 3D quiver velocity vectors.",
        latencyOrMetric: "24ms 3D Scene Assembly"
      }
    ],
    evaluation:
      "Empirical validation across multiple academic benchmark problem sets confirmed 100% numerical accuracy with zero percent (0.00%) deviation against theoretical manual solutions. In planar 3-body testing (total mass 7.10 kg), the calculator resolved center-of-mass coordinates at X = 82.81690141 cm and Y = 57.46478873 cm, matching manual geometric derivations with sub-10^-8 absolute floating-point discrepancy and zero residual noise on the unconstrained Z-axis. In linear 3-body velocity benchmarks (total mass 9.00 kg), the vectorized engine determined center-of-mass velocity at Vx = 1.77777778 m/s (matching exact 16/9 m/s momentum calculations), while 4-body 3D spatial evaluations (total mass 19.00 kg) achieved exact coordinate resolution at [5.00000000, 5.68421053, 6.10526316]. The vectorized NumPy pipeline achieved sub-millisecond core computation latency (<0.4ms) across all particle configurations, while Matplotlib visual rendering delivered synchronized 2D and 3D plots in under 45ms total execution time.",
    outcomes: [
      "Validated 100% numerical accuracy with 0.00% error against manual analytical physics derivations across 2D and 3D benchmark test cases.",
      "Eliminated cumulative floating-point drift by implementing vectorized 64-bit NumPy matrix operations.",
      "Reduced multi-particle state evaluation latency to sub-0.4ms, bypassing slow iterative Python loops.",
      "Delivered comprehensive dual-mode visual telemetry combining 2D planar scatter/quiver plots with 3D isometric spatial projections.",
      "Established complete educational reproducibility through verified documentation and instant zero-setup Google Colab cloud execution."
    ],
    techStack: [
      "Python",
      "NumPy",
      "Matplotlib",
      "Jupyter Notebook",
      "Google Colab",
      "Git"
    ],
    accentColor: "indigo",
    repoUrl: "https://github.com/weztcy/Center-of-Mass-and-Velocity-Calculator"
  }
];


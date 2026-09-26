# JPEE+ Cluster World Project

A custom 3D environment and interactive space built by Unity for the **[Cluster](https://cluster.mu/en)** metaverse platform.

<img height="400" alt="G89uTPmW8AEsLOM" src="https://github.com/user-attachments/assets/0681305b-080b-44cf-9ca7-71d9a194eeba" />

## Key Features

Designed an immersive 3D environment for community events and gatherings.

Configured lighting, collider architecture, and spatial interactions using Cluster Creator Kit.

Technical Lessons & Pipeline Post-Mortem
Note on Project Status & Repository History:
The live, fully functional world is permanently published and playable on Cluster via the link above.

During development, this project underwent multiple iterations of version control and asset pipeline experiments. Due to a critical data sync loss on external cloud storage during post-project cleanup, this repository stores the core C# scripts, configuration logs, and post-mortem analysis rather than a rebuildable Unity project.

Critical Engineering & Operational Learnings:
Version Control Limits for Heavy 3D Assets:

Evaluated Git LFS (encountered bandwidth timeouts and storage limitations with large 3D models/textures).

Tested Plastic SCM (UVCS), identified usability bottlenecks and high cognitive overhead for cross-functional workflows.

Cloud Storage & Sync Risks:

Transitioned to cloud-based file synchronization (OneDrive) for individual workflow, experiencing firsthand the high risks of destructive syncs and non-atomic deletions in large binary projects.

Future Pipeline Strategy (Key Takeaway):

Strict Asset Decoupling: Keep raw 3D source files (FBX/textures) strictly separated from Unity build components via dedicated LFS buckets with retention policies.

Immutable Backups: Implement automated, read-only offline backups for final scene structures prior to post-project cleanup.

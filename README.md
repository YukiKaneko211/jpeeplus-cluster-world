# JPEE+ Cluster World Project

A custom 3D environment and interactive space built in Unity for the **[Cluster](https://cluster.mu/en)** metaverse platform, created as part of the **[JPEE+](https://jpee-plus.com/)** project.

<img height="300" alt="Cluster World Preview" src="https://github.com/user-attachments/assets/0681305b-080b-44cf-9ca7-71d9a194eeba" />

- **Project Status:** Completed (Available)
- **Live Site:** [https://cluster.mu/w/932cdbbf-bcf3-4077-9233-e39799ab5ee2](https://cluster.mu/w/932cdbbf-bcf3-4077-9233-e39799ab5ee2)
- **Original Repository:** [roua12tnt/cluster_dv](https://github.com/roua12tnt/cluster_dv)
- **My Project Role:** Unity Developer

#### Quick World Walkthrough Video
[![video](https://img.youtube.com/vi/WVpVZGec8GU/maxresdefault.jpg)](https://youtu.be/WVpVZGec8GU)

> [!NOTE]
> This repository is a personal fork of the original [Project Repository](https://github.com/roua12tnt/cluster_dv) managed by [Maria Nawatani](https://www.linkedin.com/in/maria-nawatani-a264337b/) of OÜ Roua, the organization behind the JPEE+ project. It is showcased here to highlight my skillset, role, and responsibilities within the JPEE+ team.

## World Concept & Asset Strategy

The world concept was inspired by a scene from the French webtoon **[Devilish Vows](https://www.ono.live/webtoon/devilish-vows)** created by Maria Nawatani, decorated with festive Christmas elements specifically for our seasonal online community meetup.

- **Asset Sourcing & Licensing:** Except for the main building, most 3D assets were sourced from the Unity Asset Store and Sketchfab. To ensure scalability and avoid future legal issues, all third-party assets were strictly verified for permissive, commercially friendly licenses.

## Technical Implementation & Optimization

Using Unity and the official **[Cluster Creator Kit](https://github.com/ClusterVR/ClusterCreatorKit)**, I implemented the environment lighting, collider geometry architecture, and interactive scripts for Cluster triggers.

- **Cross-Platform Optimization:** Designed with low-end mobile devices in mind—ensuring users without high-end gaming PCs or VR headsets could seamlessly participate from smartphones.
- **Lighting & Water Shading:** Integrated large glass windows with pre-baked lightmaps for high-quality reflections without realtime performance costs. Used a [lightweight toon water shader](https://booth.pm/ja/items/2184916) to balance aesthetics with optimal performance.

## Post-Mortem & Technical Lessons Learned

During development, this project served as a sandbox for testing version control and asset management pipelines for large-scale 3D projects. 

> **Notice on Project Code State:** Due to a critical cloud sync issue during post-project maintenance, this repository reflects the last successful commit on GitHub rather than the finalized production build.

### Version Control & Pipeline Challenges
1. **Git LFS Bandwidth Limits:** Attempted version control via Git LFS, but large 3D asset uploads consistently failed due to network bandwidth timeouts.
2. **Plastic SCM (Unity Version Control) Evaluation:** Tested Plastic SCM, but found its workflow overly complex for our non-technical team members, posing a risk of accidental data loss and steep learning curves for small-scale operations.
3. **Cloud Storage Fallback:** Temporarily adopted a direct cloud storage approach (OneDrive) for project sharing. While workable for a small team where other members only needed occasional preview access prior to release, it introduced file management vulnerabilities.

### Key Takeaways
- **Data Governance & Asset Preservation:** Relying on informal cloud sync setups without a dedicated administrator or strict backup policy creates significant risk for large binary game assets.
- **Team Workflow Policies:** Moving forward, establishing clear data preservation rules, automated backup strategies, and team-wide version control workflows upfront is essential to safeguarding technical assets.

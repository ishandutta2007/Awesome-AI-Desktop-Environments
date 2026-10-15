# Awesome-AI-Desktop-Environments

# Awesome-AI-Desktop-Environments

## Top AI Desktop Environments Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Cloud Desktops, Secure Workspace Streaming & AI-Native Desktop Integration*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Desktop Environments**. These tools provide the graphical interface layer for AI agent harnesses, cloud development environments, and secure workspace delivery—streaming desktops to browsers, wrapping AI runtimes in native windows, and isolating workloads in ephemeral containers.



**Examples** include Windows 365, Amazon WorkSpaces, Citrix Workspace, VMware Horizon, Paperspace, Kasm Workspaces, Shells, Azure Virtual Desktop, Shadow PC, and Neverinstall (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, containerized desktop streaming, and AI-native desktop shells—ideal for platform engineers, remote work architects, and developers seeking transparent, vendor-independent desktop infrastructure.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Desktop-as-a-Service (DaaS) and cloud virtual desktop market is estimated at **$6B–$9.5B in 2024–2025** and projected to reach **$22B–$50B by the mid-2030s** (growing at a 13%–18.5% CAGR). While the broader ecosystem is **moderately fragmented** across regional MSPs, browser-streaming startups, and specialized VDI providers, high-end enterprise infrastructure is **highly concentrated** among an oligopoly of hyperscalers and incumbent enterprise virtualization leaders (Microsoft, AWS, Citrix, and VMware/Omnissa).

## SaaS/Hosted Platforms

| Platform | Company Size (Valuation / Revenue) | Pricing | Free Tier / Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Windows 365](https://www.microsoft.com/en-us/windows-365)** | ~$3.1T Market Cap / ~$245B Annual Revenue (Microsoft) | From $28.00/user/mo (Enterprise) or $36.00/user/mo (Business, 2 vCPU/8GB RAM/128GB) | 30-day free trial; 1 Cloud PC per tenant (2 vCPU, 8 GB RAM, 128 GB storage) | Microsoft's Cloud PC delivering streamed Windows desktops to any device with Intune and Entra ID integration. |
| **[Azure Virtual Desktop](https://azure.microsoft.com/en-us/products/virtual-desktop/)** | ~$3.1T Market Cap / ~$245B Annual Revenue (Microsoft) | From $5.50–$10.00/user/mo external access + Azure VM infrastructure (pooled multi-session from ~$10/user/mo) | 30-day trial with $200 Azure credits; includes 12 months of select free services (VM compute consumes credits) | Microsoft cloud VDI with multi-session Windows 10/11, FSLogix profile containers, and MSIX app attach. |
| **[Amazon WorkSpaces](https://aws.amazon.com/workspaces/)** | ~$2.0T Market Cap / ~$105B AWS Revenue Run-rate (Amazon) | From $7.25/mo + $0.22/hr (metered) or flat $21.00/user/mo (Value tier, 1 vCPU/2GB RAM/80GB root) | 3-month free trial; up to 2 Standard AutoStop WorkSpaces with 40 combined usage hours/month, 80GB root + 50GB user volumes | Fully managed desktop-as-a-service on AWS with Windows, Amazon Linux, and Ubuntu desktop streaming. |
| **[VMware Horizon](https://www.vmware.com/products/horizon.html)** | $4.0B Acquisition by KKR (Omnissa / ex-VMware EUC) | From $9.00–$12.50/user/mo (Horizon Cloud control plane license; underlying cloud VM compute billed separately) | 30-day to 60-day free trial for Horizon Cloud Service (accessible via Azure/AWS marketplace evaluation) | Enterprise virtual desktop and application streaming platform featuring App Volumes and Blast Extreme protocol. |
| **[Citrix Workspace](https://www.citrix.com/)** | $16.5B Take-Private Acquisition (Cloud Software Group) | From $10.00/user/mo (Citrix DaaS Standard; minimum user commitments and cloud VM compute apply) | 7-day guided trial via Azure Marketplace, or 30-day custom enterprise Proof-of-Concept (PoC) | Enterprise digital workspace delivering virtual apps and desktops with HDX protocol and zero-trust security. |
| **[Paperspace](https://www.paperspace.com/)** | $111M Acquisition by DigitalOcean (~$3.5B Market Cap) | From $0.07/hr or $8.00/mo (CPU/GPU Core desktops) + $5.00/mo storage | Free tier for Gradient Notebooks (5 GB persistent storage, 1 concurrent instance, 6-hr session timeout; no free Core VDI) | Cloud GPU and CPU virtual machines and desktop streaming tailored for machine learning and development. |
| **[Shadow PC](https://shadow.tech/)** | ~$30M–$50M Est. Valuation (€2M debt-clearing acquisition + ongoing funding by Octave Klaba / Synfonium) | From $29.99/mo (Neo Lite: 16GB RAM, RTX 2000 Ada tier, 120 hrs/mo cap) | No free trial or free tier; introductory promotional discounts offered periodically (no partial refunds) | High-performance Windows cloud PC streaming dedicated RTX GPUs at up to 4K/5K resolution for gaming and pro workloads. |
| **[Kasm Cloud](https://kasm.com/)** | ~$2.8M Annual Recurring Revenue (Kasm Technologies, private) | From $5.00/user/mo (Personal Cloud) or $19.00/user/yr (Enterprise license self-hosted) | Free Community Edition (self-hosted: 5 concurrent sessions forever, community support); Cloud Personal free slots vary | Managed containerized desktop, browser isolation, and app streaming delivered via browser with SOC 2 compliance. |
| **[Neverinstall](https://neverinstall.com/)** | ~$5M–$15M Est. Seed Valuation (~$1.5M Venture Funding Raised) | From $15.00/mo (Basic plan) or $50.00/mo (Premium plan) | Free forever plan with 1-hour session limit per launch (basic compute, resets between sessions) | Cloud application and desktop streaming platform executing applications directly inside web browsers. |
| **[Shells](https://shells.com/)** | Privately Held / Seed stage (E Shells, Inc.) | From $4.95/mo (Lite: 1 vCPU, 2GB RAM, 40GB storage, 10 hrs/mo) or $11.95/mo (Basic unlimited) | No free tier; 7-day money-back guarantee on all plans to test risk-free | Personal and small-business cloud computer streaming accessible from any web browser or mobile client. |



## Open-Source GitHub Projects



- **[DSH Desktop (anywhere-labs)](https://github.com/anywhere-labs/dsh-desktop)**  

  **The reference open-source AI-native desktop environment for DeepSeek Harness** (open-source). **The most mature AI harness desktop shell available.** Wraps the full DeepSeek Harness runtime in a native Electron application for macOS and Windows—handles window management, tray lifecycle, single-instance locking, and local service orchestration . **Deliberately does not fork upstream**—users keep official profiles, plugins, sessions, and Web UI, while Desktop owns only native integration . Features **compatibility mode** (preserves upstream client) and **advanced mode** (Desktop-owned layout with native materials and drag regions) . **The architectural blueprint for building AI harness desktop environments.**



- **[DSH Desktop (zcy0735111-png)](https://github.com/zcy0735111-png/dsh-desktop)**  

  **Zero-dependency Windows desktop client for DeepSeek Harness** (open-source). **The most accessible AI desktop environment for Windows users.** Bundles Node.js runtime and DSH CLI—recipient needs no Node.js installation, no configuration, just double-click . **Port detection and auto-hosting**: scans ports 3080-3103; if existing DSH service found, attaches to it; otherwise auto-starts hidden `dsh web` with logs to disk . **Clean shutdown**: only kills servers it started—won't murder manually launched instances . **Reuses your existing `DSH_HOME`**—sessions, credentials, and settings carry over seamlessly . **The most practical Windows AI desktop wrapper available.**



- **[DSH Desktop (dataelement)](https://github.com/dataelement/dsh-desktop)**  

  **Local-first, cross-platform desktop app for DeepSeek Harness** (open-source). **The most feature-rich AI desktop environment.** Features **PPT generation** (16 templates, 192 layouts, editable PPTX output) , **phone access** via QR pairing over local network or Cloudflare Quick Tunnel , **portable Agent presets** (`.dshpreset` packages with conflict checks) , **offline DOCX/PPTX/XLSX skills** with bundled Python libraries , and **Safe Mode** that temporarily blocks third-party plugins . **Preserves profiles, plugins, workspaces, sessions, and model settings across app upgrades** . **The most complete AI desktop product available.**



- **[Selkies](https://github.com/selkies-project/selkies)**  

  **Low-latency accelerated web remote desktop streaming for self-hosting, containers, Kubernetes, or Cloud/HPC** (MPL-2.0) . **The most performant open-source desktop streaming platform available.** **WebSockets as default transport**—carries video, audio, input, clipboard, and file transfers through a single TCP port, eliminating STUN/TURN infrastructure requirements . **WebRTC as optional transport** . **Rust-based pixelflux** for screen capture and video encoding; **pcmflux** for audio . **Hardware-accelerated encoding** on Intel, AMD, and NVIDIA systems with software fallbacks . **Achieves 60+ FPS on Full HD** with zero-copy video rendering . **Two-way clipboard** (text and images), keyboard/mouse/gamepad input, microphone and webcam forwarding . **Designed for AI researchers, HPC administrators, Jupyter/Kubernetes/Coder infrastructure, and cloud gaming** . **The most capable open-source desktop streaming platform available.**



- **[KasmVNC](https://github.com/kasmtech/KasmVNC)**  

  **Modern VNC server and client, web-based and secure** (open-source) . **5,267 GitHub stars**. **The most widely deployed open-source browser-based VNC platform.** Powers Kasm Workspaces' desktop streaming and is used by hundreds of projects for remote desktop access.



- **[Neko](https://github.com/m1k1o/neko)**  

  **Self-hosted virtual browser and remote desktop system streaming Linux graphical environments through WebRTC** (Apache-2.0) . **22,343 GitHub stars**. **The most popular open-source collaborative desktop streaming platform.** **Multiple simultaneous participants** within the same shared session . **Streams browsers, individual applications, or complete desktop environments** (XFCE, KDE) . **Shared keyboard/mouse control** for collaborative browsing, teaching, demonstrations, and support sessions . **Keeps cookies and browser state on the remote system**—not the viewer's browser . **Can broadcast through RTMP** for external streaming . **The most feature-complete open-source platform for collaborative remote desktops.**



- **[Apache Guacamole](https://guacamole.apache.org/)**  

  **Clientless remote desktop gateway supporting VNC, RDP, and SSH** (Apache-2.0) . **The most widely deployed open-source remote desktop gateway.** **No plugins or client software required**—HTML5 web application . **Desktops need not physically exist**—cloud-hosted desktops accessible through Guacamole . **Built on well-documented APIs** for tight integration into other applications . **The standard for organizations needing protocol-agnostic remote access.**



- **[IsardVDI](https://gitlab.com/isard/isardvdi)**  

  **Free Software desktop virtualization platform** (AGPL-3.0) . **GPU support via NVIDIA Grid** . **Deploy in minutes with Docker and Docker Compose** . **Scalable**—manage multiple hypervisors and add/remove based on need . **Fast**—start a desktop and connect in seconds . **Versatile**—runs all OS supported by QEMU/KVM with multiple viewers: SPICE, noVNC (web), RDP, Guacamole RDP (web) . **The most accessible open-source full VDI platform available.**



- **[OpenThinRdp](https://github.com/OpenThinRdp/openthinrdp)**  

  **Open-source thin client OS with RDP over UDP** (open-source) . **The most focused open-source thin client for Windows VDI.** **Free IGEL/ThinOS alternative** . **RDP over UDP** for smoother sessions on busy servers, lossy Wi-Fi, and VPNs—adapts frame rate and quality to line conditions . **Kiosk sign-in** with full-screen remote desktop, no local shell . **USB redirection for VDI** (signature keys, tachograph keys, webcams through RDP channels) . **Managed from shared SMB folder** with Windows manager app . **Signed updates** that never interrupt sessions . **The most enterprise-ready open-source thin client OS available.**



- **[ThinLinc](https://www.cendio.com/thinlinc/)**  

  **Open-source, enterprise-ready remote desktop solution for Linux** (open-source) . **The most established open-source Linux VDI platform.** **Web browser and native client access** . **GPU acceleration support** . **Multi-user VDI layer** allowing multiple users to connect to Ubuntu Desktop through browser or dedicated client . **The standard for Linux VDI deployments requiring enterprise features.**



- **[wolf (games-on-whales)](https://github.com/games-on-whales/wolf)**  

  **Stream virtual desktops and games running in Docker** (open-source) . **2,183 GitHub stars**. **The most popular open-source game streaming platform.** Streams full desktop sessions and games from containerized environments.



### Additional Strong Open-Source Options



- **[noVNC](https://github.com/novnc/noVNC)** — VNC client web application (MPL-2.0). **14,031 GitHub stars** . **The foundational open-source VNC web client.**

- **[RustDesk](https://github.com/rustdesk/rustdesk)** — Open-source remote desktop application for self-hosting as TeamViewer alternative (AGPL-3.0). **124,065 GitHub stars** . **The most popular open-source remote desktop tool.**

- **[MeshCentral](https://github.com/Ylianst/MeshCentral)** — Complete web-based remote monitoring and management (Apache-2.0) . **The most comprehensive open-source RMM platform.**

- **[x11docker](https://github.com/mviereck/x11docker)** — Run GUI applications and desktops in Docker and Podman containers (open-source) . **The most focused open-source tool for containerized GUI apps.**

- **[gow (games-on-whales)](https://github.com/games-on-whales/gow)** — Dockerized games and apps (Steam, Firefox, Retroarch) (open-source) . **735 GitHub stars**.

- **[dsh_desktop (Tauri)](https://dshbase.com/plugins/dsh_desktop/)** — DSH Windows desktop client migrated from Electron to Tauri 2 (Rust) (open-source) . **The most modern AI desktop shell architecture**—smaller install, lower memory, faster startup, guardian waterfall for self-healing .

- **[DSH-Decktop](https://dshbase.com/plugins/DSH-Decktop/)** — Electron desktop shell for DSH that installs `@deepseek-ai/dsh` at runtime (open-source) . **The most lightweight DSH desktop wrapper**—first launch installs runtime, upgrades without rebuild .

- Community **n8n** workflows for desktop session alerting and workspace automation.



**Frameworks for building custom systems**: Combine **Selkies** for high-performance desktop streaming with **KasmVNC** for browser-based VNC access, **Apache Guacamole** for protocol-agnostic gateway, **IsardVDI** for full VDI management, and **DSH Desktop** for AI-native harness integration—creating a fully self-hosted, enterprise-grade AI desktop environment platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- AI desktop environments handling user sessions and workspace data must comply with data protection regulations (GDPR, CCPA, etc.) and enterprise security policies.

- **Open-source AI desktop environments are maturing rapidly.** DSH Desktop variants (anywhere-labs, zcy0735111-png, dataelement) provide production-grade AI harness desktop shells with bundled runtimes, zero-dependency distribution, and clean lifecycle management . Selkies achieves 60+ FPS Full HD streaming with WebSocket transport . **These are genuine alternatives to commercial platforms.**

- **The desktop shell is a product entry point, not a fork.** DSH Desktop (anywhere-labs) explicitly does not reimplement upstream Harness—it owns native integration while upstream owns agent semantics . **This architectural boundary is critical**—it prevents permanent divergence and keeps upgrades clean.

- **Containerized workspace streaming is the security model.** Kasm Workspaces streams browsers, apps, and desktops as pixels—sensitive data remains inside the organization's environment, not on user devices . Ephemeral sessions destroyed at session end minimize persistent data on endpoints . **This is the Zero Trust desktop architecture.**

- **AI harness desktop environments are a new category.** DSH Desktop exists because "Node.js, profiles, dependency installation, ports, and process lifetime are still part of the experience" for CLI-first harnesses . **The desktop wrapper solves onboarding friction**—bundled runtimes, tray lifecycle, native window management, and version discovery with confirmation-gated installers .

- Self-hosted open-source solutions require proper security hardening, GPU provisioning for accelerated streaming, and ongoing maintenance. Desktop environments are user-facing infrastructure—performance and reliability directly impact productivity.



---



**Made for platform engineers, remote work architects, and developers building transparent desktop environment solutions.**  

Let's make AI Desktop Environments more open, data-driven, and streamable.

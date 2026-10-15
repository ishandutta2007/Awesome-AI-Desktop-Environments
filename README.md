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

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Windows 365](https://www.microsoft.com/en-us/windows-365)**  

  Microsoft's Cloud PC service delivering full Windows desktops to any device via browser or Remote Desktop app. Integrated with Intune for management and Entra ID for identity.



- **[Amazon WorkSpaces](https://aws.amazon.com/workspaces/)**  

  Fully managed desktop-as-a-service (DaaS) on AWS. Features Windows and Linux desktops, WorkSpaces Web for browser-based access, and WorkSpaces Core for third-party VDI management.



- **[Citrix Workspace](https://www.citrix.com/)**  

  Enterprise workspace platform delivering virtual apps and desktops. Features Citrix DaaS, HDX protocol for optimized performance, and zero-trust access controls.



- **[VMware Horizon](https://www.vmware.com/products/horizon.html)**  

  Virtual desktop and app delivery platform. Features Horizon Cloud on Azure, App Volumes, and Dynamic Environment Manager for personalized workspaces.



- **[Paperspace](https://www.paperspace.com/)**  

  Cloud computing platform with GPU-accelerated virtual desktops. Features Gradient for ML workloads and Core for virtual machines. Acquired by DigitalOcean.



- **[Azure Virtual Desktop](https://azure.microsoft.com/en-us/products/virtual-desktop/)**  

  Microsoft's cloud VDI service with multi-session Windows 10/11, FSLogix profile management, and App Attach for MSIX packaging.



- **[Shadow PC](https://shadow.tech/)**  

  Cloud gaming and productivity desktop streaming. Features high-end GPU access, low-latency streaming, and support for multiple devices.



- **[Shells](https://shells.com/)**  

  Personal cloud desktop provider. Features browser-based access, persistent storage, and Linux/Windows environments.



- **[Neverinstall](https://neverinstall.com/)**  

  Cloud application streaming platform. Runs desktop apps in the cloud and streams them to any browser without local installation.



- **[Kasm Cloud](https://kasm.com/)**  

  Managed version of Kasm Workspaces. Streams containerized browsers, desktops, and applications via web browser with SOC 2 Type II attestation .



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

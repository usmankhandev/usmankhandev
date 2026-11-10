# Hello 👋

I’m Usman, a Senior DevOps & Platform Engineer, with a knack of Product System Design, Security and Customr Success.

For six years I’ve built and run multi-cloud production systems: cloud-native platforms on Kubernetes, CI/CD for both modern and legacy stacks, and the infrastructure that keeps production AI reliable, from LLM gateways and tracing to vector search and multi-agent workflows.

$ whoami

    🛠️ Senior DevOps & Platform Engineer with Product Design and Customer Success
    🤖 AI Infrastructure Engineer: LLM platforms, RAG, agents in production
    💼 6 years building and operating production systems
    🧯 Troubleshooter at heart: Kubernetes networking to IIS rapid-fail 503s
    ⚙️ Infrastructure as code, automation-first, production-first

$ stack

    ☁️ Cloud: AWS (EKS, VPC, ALB, Lambda, SQS/SNS), Azure (AKS, VNet, ACR), OCI
    ☸️ Containers: Docker, Kubernetes (AKS, EKS, k3s)
    🏗️ IaC & config: Terraform, Pulumi (Python), Ansible
    🔁 CI/CD: Azure DevOps (YAML, extends templates, self-hosted agents), Jenkins (Shared Libraries)
    🪟 Windows estates: IIS, .NET Framework & MSBuild, PowerShell, PowerBuilder headless builds
    📈 Observability: Prometheus, Grafana, Loki, Alertmanager, Langfuse
    🤖 AI infra: LiteLLM, Langfuse, Qdrant, pgvector, n8n, MCP, LangChain, LangGraph, AutoGen, CrewAI
    🧩 Backend: Node.js, NestJS, TypeScript, Python & FastAPI, system design
    🗄️ Data: PostgreSQL, Redis, MongoDB, ClickHouse

$ production

    🤖 Multi-tenant AI platform on EKS: LLM gateway (LiteLLM), tracing & evals (Langfuse + ClickHouse),
       vector search (Qdrant), workflow automation (n8n), MCP tool gateway and an agent-assist API
       behind Kong, CloudFront and WAF, with per-tenant namespace isolation and resource quotas
    🔁 Release automation: turned a 7-phase, email-driven manual release process into pipelines
       (Python, Jenkins Shared Libraries, Azure DevOps) across four product lines and two toolchains
       (.NET/MSBuild and PowerBuilder)
    🚚 SVN → Azure DevOps Git migration with per-region self-hosted agent pools
    ⬆️ Staged Jenkins 1.x → 2.4xx LTS upgrade ladder with a sub-10-minute rollback plan
    🔐 Corporate VPN migration to Azure AD SAML/SSO

$ building

    💬 Chatterly: an organizational-memory and team-intelligence platform for engineering teams
    ☸️ AKS from scratch with Terraform: VNet, NSG, AKS, ACR, remote state
    📈 Full Prometheus/Loki/Grafana stack with golden-signal dashboards and Slack alerting
    📨 Event-driven NestJS backend: SQS/SNS fan-out with DLQs and Workload Identity
    🧱 Reusable Pulumi platform for multi-project AWS infrastructure (VPC, EKS, RDS, ALB)

$ troubleshoot --history

    🧭 Method: contain impact → evidence over guesses → fix in code, not on the server → prevent recurrence

    🔍 503s straight after a release (IIS)
       Worker processes crashed on start; IIS rapid-fail protection stopped the pool.
       WAS and CLR events pointed to a mis-set runtime; fixed in config code, gated deploys on real health.
       → A green smoke test on static content proves nothing about a managed app.

    🔍 Healthy AKS nodes, unmanageable workloads
       An NSG rule blocked kubelet (10250): no exec, no logs, no metrics, so no safe way to operate.
       → Network rules are part of the platform contract: versioned and tested with the cluster.

    🔍 Kubernetes service CIDR overlapping the VNet
       In-cluster routing silently captured real addresses.
       → IP planning is a day-zero architecture decision; renumbering a live network costs the most.

    🔍 PostgreSQL failing to start on Azure CSI volumes
       PGDATA conflicted with how the volume was mounted; aligned the data path with the mount.
       → Stateful workloads need storage semantics understood, not just a PVC.

    🔍 Monorepo delivery blocked for days
       Circular Nx targets, executor conflicts, Prisma enums lost between Dockerfile stages.
       → The build graph is a production system: deterministic stages, explicit outputs.

    🔍 Container image cut from 248 MB to 127 MB
       Multi-stage builds and layer ordering; CVEs triaged with Trivy.
       → Smaller images mean faster scale-out, cheaper pulls and a smaller attack surface.

    🔍 Legacy PowerBuilder builds failing in CI
       OrcaScript segfaulted on long paths and reported failure on success.
       Shortened paths, then verified the output artifacts instead of trusting exit codes.
       → Automate the legacy estate you have; trust the artifact, not the exit code.

    🔍 Windows servers silently failing first boot
       Split network from OS (RDP open, WinRM closed), read logs over SSM, found a script aborting early.
       Made bootstrap self-validating and replaced instances instead of patching them.
       → Fail loudly at the cause; rebuild from code rather than repair by hand.

$ Core Areas Next:

    🧠 ML core: LoRA/QLoRA fine-tuning, evaluation, model serving (vLLM, KServe)
    🧪 MLOps: SageMaker AI, MLflow, Kubeflow, GPU scheduling on Kubernetes.
    🏛️ AI Safety Engineering: LLM Security and Secure RAG Application as per OWASP

$ ping

    💻 https://github.com/usmankhandev
    💼 https://linkedin.com/in/usmankhandev
    ✍️ https://medium.com/@dev.usmankhan
    🐦 https://x.com/dev_usmankhan
    🅾 https://www.instagram.com/dev.usmankhan/
    📧 osmankhan.dev@gmail.com

---

> “Engineering intelligence into systems.”

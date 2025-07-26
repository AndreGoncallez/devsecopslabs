# 🛡️ DevSecOps Labs

Laboratórios práticos com foco em **segurança integrada ao ciclo DevOps**. Projetos com CI/CD seguro, Docker, scanners de vulnerabilidade e automações reais.

---

## 💡 Objetivo

Demonstrar como implementar pipelines automatizados seguros com ferramentas como:

- **Docker**
- **GitHub Actions**
- **Trivy**, **Bandit**, **Checkov**
- **FastAPI**, **Terraform**, **GCP**

---

## 🚀 Projetos disponíveis

| Projeto | Descrição | Tecnologias |
|---------|-----------|-------------|
| API com CI/CD seguro | Build + scan + push no DockerHub com Trivy | FastAPI, Docker, GitHub Actions |
| Análise de código Python | Pipeline com Bandit e envio de alerta | Python, Bandit |
| IaC seguro com Terraform | Criação de infra GCP com validação de segurança | Terraform, tfsec |

---

## 🧰 Stack utilizada

- Docker, DockerHub  
- GitHub Actions  
- Snyk, Trivy, Bandit, tfsec  
- Python, FastAPI  
- Terraform, GCP (Compute, IAM)

---

## 🗂️ Estrutura do projeto

```bash
📁 devsecopslabs/
├── cicd-api-secure/
│   ├── app/
│   ├── Dockerfile
│   ├── .github/workflows/pipeline.yml
├── terraform-iac-secure/
│   ├── main.tf
│   ├── variables.tf
│   ├── scan_result.md
```

---

## 🧠 Como rodar localmente

Clone o repositório:

```bash
git clone https://github.com/AndreGoncallez/devsecopslabs.git
cd devsecopslabs/cicd-api-secure
```

Suba com Docker:

```bash
docker build -t myapi .
docker run -p 8000:8000 myapi
```

Visualize: [http://localhost:8000](http://localhost:8000)

---

## 🧪 Em breve

- Análise estática com SonarQube
- Integração com Snyk CLI
- Terraform Cloud com GCP CI

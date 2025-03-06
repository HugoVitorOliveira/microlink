# 🌐 Resumo do Projeto Microlink

## 🏗️ System Design

### Requisitos Funcionais:
- 🔗 Encurtar URLs longas para links curtos.
- ↪️ Redirecionar o link curto para a URL original.
- 📊 Monitorar métricas (ex.: cliques por link) (talvez).
- 🔒 Gerenciar usuários e permissões, excluir link's em 5h de usuários não logados.

### Requisitos Não Funcionais:
- 🚀 Alta disponibilidade e desempenho.
- ⚖️ Escalabilidade horizontal para atender a muitos usuários.
- 🛡️ Segurança no armazenamento e redirecionamento de URLs.

### Arquitetura:
- **Frontend**: Interface simples para criar e gerenciar URLs.
- **Backend**: API para geração e redirecionamento de URLs.
- **Banco de Dados**:
  - 🎯 Relacional: **PostgreSQL** para gerenciar metadados e usuários.

### Fluxo Geral:
1. Cliente envia URL longa ao backend.
2. Backend gera um ID único (ex.: hash ou UUID).
3. URL curta é salva no banco com a URL original e metadados.
4. Redirecionamentos são resolvidos pelo backend e cache.

---

## 💻 Tecnologias

### Backend:
- 🖥️ **Quarkus**: Framework leve e performático para microsserviços.

### Banco de Dados:
- 🗂️ **PostgreSQL**.

### Frontend:
- 💅 **Angular** para criar uma interface intuitiva.

### DevOps:
- 🐳 **Docker** para containerização.
- 🏗️ **Kubernetes** para orquestração.
- 🚀 **CI/CD**: **GitHub Actions**.

### Monitoramento:
- 📈 **Prometheus + Grafana** para métricas.
- 🔍 **Elastic Stack (ELK)** para logs.

## Outros
- 📈 **Implementar relatórios com Jasper Report**

---

## 🧩 Metodologia

### Planejamento:
- 🎯 Definir casos de uso e requisitos.
- 📝 Criar diagramas de fluxo e arquitetura.

### Implementação:
- 🔨 Dividir em serviços menores (microsserviços).
- 📦 Usar boas práticas como SOLID e **Clean Code**.

### Testes:
- 🧪 Escrever testes unitários e de integração.
- 🛠️ Realizar testes de carga (ex.: **JMeter ou PostMan Collections**).

### Iteração:
- 🔄 Melhorar continuamente com feedback de usuários.
- ⚙️ Escalar conforme o aumento do tráfego.

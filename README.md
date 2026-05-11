<div align="center">

# 🖥️ PoupePC

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)

**Plataforma web e mobile de pesquisa e comparação de preços de peças de informática, ajudando gamers e entusiastas a montar o PC ideal com o melhor custo-benefício.**

[Sobre](#-sobre-o-projeto) •
[Tecnologias](#-tecnologias-utilizadas) •
[Instalação](#-como-rodar-o-projeto) •
[Equipe](#-equipe) •
[Documentação](#-documentação-completa)

</div>

---

## 📖 Sobre o Projeto

O **PoupePC** é uma plataforma que centraliza a **comparação de preços de componentes de hardware** entre as principais lojas do Brasil — **Kabum**, **Pichau** e **Terabyte** — automatizando a busca e garantindo a melhor economia na hora de montar seu computador.

### 🎯 Objetivo

Simplificar a montagem de computadores, automatizando a comparação de preços e garantindo que o usuário finalize sua configuração com o maior nível de economia possível.

### 🔑 Funcionalidades Principais

| Funcionalidade | Descrição |
|----------------|-----------|
| 🔍 **Busca Inteligente** | Pesquisa de componentes em múltiplas lojas simultaneamente |
| 📊 **Comparação de Preços** | Comparativo visual entre lojas (Kabum, Pichau, Terabyte) |
| 🖥️ **Montagem de PC** | Ferramenta para configurar builds completas |
| 🌙 **Modo Escuro** | Interface adaptável com tema claro e escuro |
| 📱 **Multiplataforma** | Disponível para Web e Mobile (Flutter) |
| 💾 **Banco de Dados** | Persistência com SQLite para histórico e favoritos |

---

## 🛠️ Tecnologias Utilizadas

<div align="center">

| Camada | Tecnologia | Descrição |
|--------|------------|-----------|
| **Back-End** | ![Python](https://img.shields.io/badge/Python_3-3776AB?style=flat-square&logo=python&logoColor=white) | Lógica de negócio e scraping de preços |
| **Banco de Dados** | ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) | Armazenamento local de dados |
| **Front-End Mobile** | ![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white) | Aplicação mobile multiplataforma |
| **Front-End Web** | ![HTML](https://img.shields.io/badge/HTML/CSS/JS-E34F26?style=flat-square&logo=html5&logoColor=white) | Interface web responsiva |
| **Versionamento** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) | Controle de versão com Git Flow |

</div>

---

## 📁 Estrutura do Projeto

```
PoupePC/
├── 📂 src/
│   ├── 📂 backend/              # Lógica Python e gerenciamento do banco de dados
│   │   ├── database_manager.py
│   │   └── db/
│   └── 📂 frontend/             # Aplicação Flutter (Web e Mobile)
│       ├── lib/
│       ├── android/
│       ├── ios/
│       ├── web/
│       └── pubspec.yaml
├── 📂 docs/
│   ├── 📂 planning/             # Planejamento do projeto
│   │   ├── backlog.md
│   │   ├── roadmap.md
│   │   └── project-vision.md
│   ├── 📂 workflow/             # Fluxo de trabalho da equipe
│   │   ├── development-vs-production.md
│   │   ├── team-organization.md
│   │   ├── kanban.md
│   │   └── gantt.md
│   └── 📂 evidences/            # Prints e evidências do processo
│       └── version-control/
├── .gitignore
├── CONTRIBUTING.md
├── requirements.txt
└── README.md
```

---

## 🚀 Como Rodar o Projeto

### Pré-requisitos

- **Python 3.8+** instalado
- **Flutter SDK** (para o front-end mobile)
- **Git** para versionamento

### 🔧 Back-End (Python + SQLite)

```bash
# 1. Clone o repositório
git clone https://github.com/gabrielportella989/PoupePC.git
cd PoupePC

# 2. Instale as dependências
pip install -r requirements.txt

# 3. Inicialize o banco de dados
python src/backend/database_manager.py
```

### 📱 Front-End (Flutter)

```bash
# 1. Entre na pasta do frontend
cd src/frontend

# 2. Instale as dependências do Flutter
flutter pub get

# 3. Execute a aplicação
flutter run
```

---

## 👥 Equipe

<div align="center">

| Membro | Função | Responsabilidade |
|--------|--------|-----------------|
| **Erick Hayashi C. de Freitas** | 📋 Líder / Documentação | Gestão do projeto e documentação técnica |
| **Gustavo Henrique Satorato** | 🗄️ Banco de Dados | SQLite — persistência e segurança dos dados |
| **Miqueias Souza da Silva** | ⚙️ Back-End | Lógica em Python e integração com banco |
| **Eric Augusto Juliani** | 💻 Front-End | Código funcional em Flutter/Web |
| **Gabriel da Silva Portella** | 🎨 UI/UX Design | Prototipação e design das interfaces |

</div>

---

## 🔀 Fluxo de Desenvolvimento

Utilizamos uma adaptação do modelo **Git Flow** para organizar nosso trabalho:

```mermaid
gitgraph
    commit id: "init"
    branch develop
    commit id: "setup"
    branch feature/scraper
    commit id: "feat: scraper"
    checkout develop
    merge feature/scraper
    branch feature/ui
    commit id: "feat: dark mode"
    checkout develop
    merge feature/ui
    checkout main
    merge develop id: "v1.0.0"
```

| Branch | Propósito |
|--------|-----------|
| `main` | ✅ Código estável de produção |
| `develop` | 🔄 Branch de integração |
| `feature/*` | 🆕 Funcionalidades específicas |

> 📚 Para mais detalhes: [Desenvolvimento vs Produção](docs/workflow/development-vs-production.md)

---

## 📋 Documentação Completa

| Documento | Descrição |
|-----------|-----------|
| 📌 [Visão do Projeto](docs/planning/project-vision.md) | Objetivo, problema, público-alvo e diferenciais |
| 📋 [Backlog do Produto](docs/planning/backlog.md) | Lista priorizada de funcionalidades |
| 🗺️ [Roadmap](docs/planning/roadmap.md) | Cronograma de fases do projeto |
| 🔀 [Dev vs Produção](docs/workflow/development-vs-production.md) | Estratégia de branches e ambientes |
| 👥 [Organização da Equipe](docs/workflow/team-organization.md) | Papéis e responsabilidades |
| 📊 [Quadro Kanban](docs/workflow/kanban.md) | Acompanhamento das tarefas |
| 📈 [Gráfico de Gantt](docs/workflow/gantt.md) | Cronograma detalhado por sprint |

---

## 📝 Licença

Este projeto é desenvolvido para fins acadêmicos — **ADS / Desenvolvimento para Dispositivos Móveis** na **UNINGÁ**.

---

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Gabriel_Portella-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gabrielportella-dev)
[![GitHub](https://img.shields.io/badge/GitHub-gabrielportella989-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/gabrielportella989)

⭐ **Se este projeto te ajudou, considere dar uma estrela!** ⭐

</div>

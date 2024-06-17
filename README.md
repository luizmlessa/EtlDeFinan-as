# Projeto ETL com Apache Airflow e Docker

Este projeto demonstra como configurar um ambiente de desenvolvimento para realizar ETL (Extração, Transformação e Carga) de dados usando Apache Airflow e Docker.

## Pré-requisitos

- Docker instalado na máquina local. [Instalação do Docker](https://docs.docker.com/get-docker/)
- Docker Compose instalado na máquina local. [Instalação do Docker Compose](https://docs.docker.com/compose/install/)

## Estrutura do Projeto

projeto/
│
├── docker-compose.yml
├── README.md
├── dags/
│ ├── exemplo_dag.py
│ └── ...
├── logs/
│ └── (diretório vazio inicialmente)
└── plugins/
└── (diretório vazio inicialmente)


- **`docker-compose.yml`:** Arquivo de configuração Docker Compose para configurar serviços como PostgreSQL, Apache Airflow, Grafana, etc.
- **`dags/`:** Diretório para armazenar os DAGs (Directed Acyclic Graphs) do Apache Airflow.
- **`logs/`:** Diretório onde os logs do Apache Airflow são armazenados.
- **`plugins/`:** Diretório para armazenar plugins do Apache Airflow.

## Como Usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
Inicie os serviços com Docker Compose:


docker-compose up -d
Isso iniciará os contêineres Docker para PostgreSQL, Apache Airflow e possivelmente outros serviços configurados no docker-compose.yml.

Acesse o Airflow Web UI:

Abra seu navegador e vá para http://localhost:8080.
Use as credenciais padrão (se configurado) ou as especificadas no arquivo docker-compose.yml.
Gerencie seus DAGs:

Coloque seus arquivos de DAGs no diretório dags/.
Eles serão automaticamente detectados e carregados pelo Apache Airflow.
Monitoramento com Grafana (se aplicável):

Acesse o Grafana em http://localhost:3000.
Faça login com as credenciais configuradas (por exemplo, admin/admin).

Contribuindo
Contribuições são bem-vindas! Sinta-se à vontade para enviar pull requests ou reportar problemas.




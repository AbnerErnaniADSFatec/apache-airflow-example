# Apache Airflow Examples

Apache airflow é uma ferramenta de código aberto para a organização e monitoramento de fluxos de trabalho complexos e `pipelines` de processamento de dados. É uma plataforma para agendar tarefas e procedimentos com base na linguagem de programação `Python`.

Um fluxo de trabalho pode ser um simples cálculo, a criação de uma infraestrutura, uma consultas SQL, a execução de um script em `Python` ou comandos no terminal.

O fluxo de trabalho é dividido em uma ou mais tarefas relacionadas entre si formando um `DAG` (Directed Acyclic Graph).

`DAG` é uma coleção de tarefas relacionadas que formam um procedimento.

Airflow foi desenvolvido em Python simplificando a criação de fluxos de trabalho.

A plataforma permite o monitoramento de procedimentos enquanto ainda estão em execução.

Esta plataforma possui uma interface de usuário onde é possível visualizar os dados dos procedimentos de forma simples

#### Executar o Apache Airflow no docker

Executar o comando abaixo para a inicialização das dependências do Airflow como o `Postgres` e o `Redis`:

~~~bash
docker-compose up airflow-init
~~~

O comando abaixo irá iniciar o serviço do Apache Airflow para a interfaze Web em `0.0.0.0:8080`.

~~~bash
docker-compose up
~~~

> O arquivo [`hello-world`](./dags/hello-world.py) possui um template para a criação de `DAGs` e procedimentos.

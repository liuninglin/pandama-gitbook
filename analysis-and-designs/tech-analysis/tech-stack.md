# Tech Stack

![](<../../.gitbook/assets/tech stack.jpg>)

Besides eliminating the pain point of ordering some Chinese featured products for the Chinese students. In addition, through this project, we want to try to use some NoSQL databases to address the issues of high availability in the shopping cart, complicated recommendation queries in the product detail page, the complex and unfixed schemas of different products, and sophisticated product searchings. So, the purpose of each framework or tool shows below.

### Presentation Layer

| Name      | Purpose                                                                             | Documentation                                                                                                                      |
| --------- | ----------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Nginx     | Web Server, for transmitting the dynamic requests to Django and parsing HTML pages. | [https://nginx.org/en/docs/](https://nginx.org/en/docs/)                                                                           |
| Bootstrap | CSS framework, easy to use, and a lot of free templates                             | [https://getbootstrap.com/docs/5.1/getting-started/introduction/](https://getbootstrap.com/docs/5.1/getting-started/introduction/) |
| jQuery    | Simpilify the operation of the document                                             | [https://api.jquery.com](https://api.jquery.com)                                                                                   |

### Service Layer

| Name          | Purpose                                                                                                                                                           | Documentation                                                                                                                                            |
| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Django-Rest   | Better for creating REST API                                                                                                                                      | [https://www.django-rest-framework.org/api-guide/requests/](https://www.django-rest-framework.org/api-guide/requests/)                                   |
| RabbitMQ      | MQ for decouping sub systems and asynchronous processes. For example, the latest data of shopping cart send to MQ for asynchronous processing data in Postgresql. | [https://www.rabbitmq.com/documentation.html](https://www.rabbitmq.com/documentation.html)                                                               |
| Postgresql    | Popular open-source relational database.                                                                                                                          | [https://www.postgresql.org/docs/](https://www.postgresql.org/docs/)                                                                                     |
| Redis         | In-memory database for storing the data of shopping cart.                                                                                                         | [https://redis.io/documentation](https://redis.io/documentation)                                                                                         |
| MongoDB       | Document and shchema-less database, it's better for storing products with miscellaneous data structures.                                                          | [https://docs.mongodb.com/manual/](https://docs.mongodb.com/manual/)                                                                                     |
| Elasticsearch | By its powerful inverted indexes, it's great for building search engine.                                                                                          | [https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html](https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html) |
| Neo4j         | Great for recommendation engine as its stronger ability in processing complicated realtionship queries.                                                           | [https://neo4j.com/docs/](https://neo4j.com/docs/)                                                                                                       |

### DevOps Layer

| Name      | Purpose                                                                                                                                 | Documentation                                                |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| Github    | Easy and great for team development                                                                                                     | /                                                            |
| Travis-CI | Easy to connect with Github, after submiting codes, Travis-Ci will automatically check the quality of your codes and do all unit tests. | [https://docs.travis-ci.com](https://docs.travis-ci.com)     |
| Heroku    | Best choice for connecting with Github and Travis-CI. The basic features of it is free and easy to configure.                           | [https://devcenter.heroku.com](https://devcenter.heroku.com) |

### Monitoring Layer

| Name | Purpose                                                                                                                                                | Documentation                                                                      |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------- |
| ELK  | Short for Elasticsearch + Logstash + Kibana. It's convinent for grouping log files from different servers and providing some features to analyze logs. | [https://www.elastic.co/guide/index.html](https://www.elastic.co/guide/index.html) |

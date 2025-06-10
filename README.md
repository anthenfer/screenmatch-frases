ScreenMatch Frases
Este projeto é uma API RESTful desenvolvida com Spring Boot que oferece frases aleatórias de filmes e séries, ideais para serem integradas a outras aplicações, como um frontend do projeto ScreenMatch.

Funcionalidades
Obter uma frase aleatória (título, frase, personagem e poster).
Configuração de CORS para permitir requisições de origens específicas.
Tecnologias Utilizadas
As seguintes tecnologias foram utilizadas no desenvolvimento deste projeto:

Java 17+
Spring Boot 3.x
Spring Data JPA: Para persistência de dados.
Hibernate: Implementação JPA padrão.
Banco de Dados: Utiliza um banco de dados relacional (a query RANDOM() é compatível com H2, PostgreSQL, MySQL, etc., mas a configuração específica do banco de dados não está explícita no código, sendo H2 uma opção comum para desenvolvimento).
Maven: Gerenciador de dependências e build.
Estrutura do Projeto
ScreenmatchFrasesApplication.java: Classe principal da aplicação Spring Boot.
Frase.java: Entidade JPA que mapeia a tabela frases no banco de dados.
FraseDTO.java: Record para o Data Transfer Object (DTO) que representa a frase a ser retornada pela API.
FraseRepository.java: Interface que estende JpaRepository, fornecendo métodos para operações de CRUD e uma query customizada para buscar uma frase aleatória.
FraseService.java: Camada de serviço que contém a lógica de negócio para obter a frase aleatória.
FraseController.java: Controlador REST que expõe o endpoint para a API.
CorsConfiguration.java: Configuração de CORS para permitir requisições de origens específicas.

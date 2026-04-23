# 🏢 Logistics & Enterprise Management API

Este é um ecossistema de backend robusto desenvolvido para centralizar a operação logística e administrativa de uma empresa. O sistema integra o gerenciamento de **Clientes, Funcionários, Entregadores e Produtos**, focado em consistência de dados e escalabilidade.

O projeto foi desenvolvido com **Java 17** e **Spring Boot 3**, utilizando uma arquitetura em camadas para facilitar a manutenção e evolução do software.

## 🛠️ Tecnologias e Conceitos Aplicados
* **Java 17 & Spring Boot 3**
* **Spring Data JPA**: Persistência de dados com repositórios otimizados (uso de `Optional`, `findByEmail`, `findByLote`).
* **Tratamento Global de Exceções**: Centralização de erros com `@RestControllerAdvice`.
* **Segurança de Dados**: Validações de unicidade para E-mails, CPFs, CNPJs e Lotes de produtos.
* **Arquitetura Clean**: Divisão clara entre Controllers, Services, Repositories e Models.

## 📦 Módulos da API

### 🚚 Logística e Entrega (`/entregadores`)
Gestão de parceiros logísticos, garantindo o controle de cadastro e disponibilidade de entregadores.

### 🛒 Gestão de Estoque (`/produtos`)
Controle de produtos com rastreabilidade via **Número de Lote**, garantindo que não haja duplicidade de itens no sistema.

### 👥 Recursos Humanos (`/funcionarios`)
Gerenciamento de colaboradores com tipagem rígida para cargos e setores, além de controle salarial.

### 🤝 Base de Clientes (`/clientes`)
Cadastro estruturado de consumidores para suporte a operações comerciais e entregas.

## 🛣️ Exemplos de Endpoints

| Método | Endpoint | Função |
|---|---|---|
| POST | `/produtos` | Cadastro de produto com validação de lote único |
| POST | `/entregadores` | Registro de novo entregador com trava de e-mail |
| GET | `/dev` | Informações do desenvolvedor (Welcome Controller) |

---
## ⚙️ Como Executar
1. Clone o repositório.
2. Configure o banco de dados no `application.properties`.
3. Execute: `mvn spring-boot:run`.

---
Desenvolvido por **Rodrigo Costa** 📩 [rodrigocostas147@gmail.com](mailto:rodrigocostas147@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/rodrigo-costa-139234353/)

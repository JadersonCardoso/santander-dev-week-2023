# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week

## Diagrama de Classe

```mermaid
classDiagram

class User {
  name: String
  account: Account
  features: List<Feature>
  card: Card
  news: List<News>
}

class Account {
  number: String
  agency: String
  balance: Double
  limit: Double
}

class Feature {
  icon: String
  description: String
}

class Card {
  number: String
  limit: Double
}

class News {
  icon: String
  description: String
}

User "1" *-- "1" Account : has
User "1" *-- "1..n" Feature : has
User "1" *-- "1" Card : has
User "1" *-- "1..n" News : has
```

# Santander Sev Week 2023
Java REStful API criada para santander dev week

## Diagrama de Classes

```mermaid
classDiagram
  class User {
    - name: String
    - account: Account
    - Features: List<Feature>
    - card: Card
    - news: List<News>
  }

  class Account {
    - number: String
    - balance: Float
    - limit: Float
  }

  class Feature {
    - icon: String
    - description: String
  }

  class Card {
    - Number: String
    - Limit: Float
  }

  class News {
    - icon: String
    - Description: String
  }

  User"1" --* "1" Account
  User "1"--* "N" Feature
  User "1"--* "1" Card
  User "1"--* "N" News
```

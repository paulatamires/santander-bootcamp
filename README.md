# Santander Bootcamp 2023 - Fullstack Java + Angular
Java RESTful API criada para o bootcamp Santander

## Diagrama de classes

```mermaid

classDiagram
    class User {
        - name: string
        - account: Account
        - features: Feature[]
        - card: Card
        - news: News[]
    }

    class Account {
        - number: string
        - agency: string
        - balance: float
        - limit: float
    }

    class Feature {
        - icon: string
        - description: string
    }

    class Card {
        - number: string
        - limit: float
    }

    class News {
        - icon: string
        - description: string
    }

    User --> Account
    User --> Feature
    User --> Card
    User --> News
```

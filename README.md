## 起動方法

1. docker desktopを立ち上げる
2. docker compose up -d

## 想定機能

### お金タイプ診断

```mermaid
erDiagram
    USERS ||--o{ QUESTIONS : has
    USERS {
        uuid user_id
        string nicname
        string email
        string prefecture
    }
    QUESTIONS ||--o{ ANSWER : has
    QUESTIONS {
        uuid questionId
        string text
    }
    ANSWER {
        string questionId
        uuid productCode
        int quantity
        float pricePerUnit
    }
```

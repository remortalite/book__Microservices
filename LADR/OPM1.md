# OPM1: Использовать ADRS для документирования решений
## Статус
Принято
## Контекст
Архитектура микросервисов сложна, и требуется принять множество решений. Нам понадобится способ отслеживать важные принимаемыме решения, чтобы можно было пересмотреть и оценить их в будущем. Мы предпочли бы использовать простой текстовый формат описания решений, чтобы не пришлось устанавливать какие-либо новые программные средства.
## Решение
Мы решили использовать формат упрощенной записи аохитектурных решений LARD. Этот екстовый формат достаточно легковесный, чтобы удовлетворить наши запросы. Мы будем хранить каждую LARD в отдельном файле и управлять файлами как исходным кодом. Мы также рассмотрели следующие альтернативные решения: 
- инструменты управления проектами (отвергнуто, поскольку мы бы не хотели устанавливать дополнительные инструмсенты);
- неформальное ведение записей или сарафанное радио (ненадежно).
## Следствия
- Нам потребуется создавать записи решений для ключевых решений.
- Понадобится инструмент для управления файлами записей решений как исходным кдом.
GNU GPL v3 license — you can do anything you want, but you must give me credit and distribute your changes under the same terms.

API1 is a modular framework for OutfitTool applications, providing a standardized interface for module development and integration. The API defines core interfaces for command execution, module metadata, logging, and settings management.

Key components:

- **ICommand**: Interface for executable commands with name, description, and optional context menu
- **IModuleInfo**: Interface defining module metadata including name, version, author, and API requirements
- **IModuleController**: Main module controller interface handling initialization, shutdown, command registration, and UI integration
- **SettingsManager<T>**: Generic YAML-based settings manager for persistent configuration storage
- **ModuleVersion**: Semantic versioning class with comparison operators for version management
- **Logger infrastructure**: ILogger interface and supporting classes for structured logging with different severity levels
- **DTO classes**: Data transfer objects for notifications, context menus, and other cross-module data

The API uses .NET 8.0 and follows C# 12 conventions, with all types in the `OutfitTool.API1` namespace. Modules must implement the required interfaces and reference this API assembly to ensure compatibility with the OutfitTool ecosystem.

---

Лицензия GNU GPL v3 — вы можете делать с этим кодом всё, что угодно, но должны указывать авторство и распространять свои изменения на тех же условиях.

API1 — модульная платформа для приложений OutfitTool, обеспечивающая стандартизированный интерфейс для разработки и интеграции модулей. API определяет основные интерфейсы для выполнения команд, управления метаданными модулей, ведения логов и настроек.

Ключевые компоненты:

- **ICommand**: Интерфейс для исполняемых команд с именем, описанием и необязательным контекстным меню
- **IModuleInfo**: Интерфейс, определяющий метаданные модуля, включая имя, версию, автора и требования к API
- **IModuleController**: Основной интерфейс контроллера модуля, отвечающий за инициализацию, завершение работы, регистрацию команд и интеграцию с пользовательским интерфейсом
- **SettingsManager<T>**: Универсальный менеджер настроек на основе YAML для постоянного хранения конфигурации
- **ModuleVersion**: Класс семантического версионирования с операторами сравнения для управления версиями
- **Инфраструктура логирования**: Интерфейс ILogger и вспомогательные классы для структурированного ведения логов с различными уровнями серьезности
- **Классы DTO**: Объекты передачи данных для уведомлений, контекстных меню и других данных, передаваемых между модулями

API использует .NET 8.0 и следует соглашениям C# 12, все типы находятся в пространстве имён `OutfitTool.API1`. Модули должны реализовывать требуемые интерфейсы и ссылаться на сборку этого API для обеспечения совместимости с экосистемой OutfitTool.
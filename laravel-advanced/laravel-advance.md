# 🧠 Laravel Advanced Interview Questions & Answers

### Q1: What is service container in Laravel?
- A: It is a powerful dependency injection container for managing class dependencies and performing dependency injection.

### Q2: What is service provider?
- A: Service providers are the central place to configure and bind classes into the service container.

### Q3: What is the difference between singleton and bind in a service provider?
- A: `singleton()` binds a class once and reuses the instance. `bind()` creates a new instance every time it's resolved.

### Q4: What is Laravel Facade?
- A: Static interface to classes in the service container. It provides a simple interface while resolving real instances behind the scenes.

### Q5: How does Laravel’s route model binding work?
- A: Automatically injects model instances based on route parameters by matching them to Eloquent IDs or custom keys.

### Q6: What is the difference between implicit and explicit route model binding?
- A: Implicit uses model's ID automatically. Explicit lets you define custom logic (e.g., using `Route::model()` or closures).

### Q7: What is a policy in Laravel?
- A: A class that organizes authorization logic around a model.

### Q8: What is a gate?
- A: A closure-based approach to define authorization rules that are not necessarily tied to models.

### Q9: How does Laravel middleware work?
- A: Middleware filters HTTP requests entering the application — for authentication, CORS, logging, etc.

### Q10: What is the purpose of `FormRequest`?
- A: Custom request class used for validating and authorizing form inputs in controllers.

### Q11: What is the difference between `authorize()` and `rules()` in FormRequest?
- A: `authorize()` checks permission, `rules()` defines validation logic.

### Q12: What are observers in Laravel?
- A: Used to listen to Eloquent model events like creating, updating, deleting, etc.

### Q13: How can you prevent N+1 problem in Eloquent?
- A: Use `with()` or `load()` to eager load relationships.

### Q14: What are accessors and mutators?
- A: Accessors format data when retrieved. Mutators modify data before saving.

### Q15: What is casting in Eloquent?
- A: Automatically converts attribute values to a specific type (e.g. array, datetime, boolean).

### Q16: What is a resource controller?
- A: A controller with predefined methods for typical CRUD operations.

### Q17: Difference between `hasOne` and `belongsTo`?
- A: `hasOne` defines relationship on the parent; `belongsTo` is defined on the child (holds the foreign key).

### Q18: What are jobs and queues in Laravel?
- A: Jobs represent units of work that are pushed into queues for background processing.

### Q19: How do you retry failed jobs?
- A: Using `php artisan queue:retry` or by configuring retry attempts in queue config.

### Q20: What are events and listeners?
- A: Events allow decoupled components. Listeners handle the logic when events are triggered.

### Q21: Difference between event broadcasting and firing?
- A: Broadcasting sends events to client (e.g., via WebSockets). Firing is internal to Laravel.

### Q22: What is broadcasting driver?
- A: It determines how events are broadcast (e.g., Pusher, Ably, Redis, Laravel WebSockets).

### Q23: How does Laravel handle session?
- A: Using `Session` facade or global `session()` helper. Storage options include file, database, Redis, etc.

### Q24: How can you secure Laravel sessions?
- A: Use HTTPS, set secure & HTTP-only flags, regenerate session IDs on login.

### Q25: How does Laravel handle CSRF?
- A: Middleware checks for `_token` in POST forms. Token is stored in session.

### Q26: What is `lazyCollection`?
- A: It allows working with large datasets efficiently using PHP generators.

### Q27: What is the difference between `Collection` and `LazyCollection`?
- A: `Collection` loads all items in memory; `LazyCollection` streams them one-by-one.

### Q28: What is the repository pattern?
- A: An abstraction layer that separates data access logic from business logic.

### Q29: What is the service pattern?
- A: Encapsulates complex business logic in dedicated service classes outside of controllers.

### Q30: What is the strategy pattern in Laravel?
- A: Allows selecting algorithms at runtime (e.g., different payment gateways).

### Q31: What is Laravel Horizon?
- A: A dashboard and monitoring tool for Laravel queues powered by Redis.

### Q32: What is Laravel Telescope?
- A: A debug assistant for inspecting requests, exceptions, logs, queries, jobs, etc.

### Q33: What is rate limiting?
- A: Prevents abuse of routes/APIs by limiting number of requests per minute/hour using `RateLimiter`.

### Q34: How do you version APIs in Laravel?
- A: Group routes under versioned prefixes (e.g., `v1`, `v2`) or use route groups.

### Q35: How to customize Laravel authentication?
- A: Use `Fortify` or `Breeze` or override the auth logic manually in guards/providers.

### Q36: What are guards and providers?
- A: Guards define how users are authenticated; providers define how users are retrieved.

### Q37: What is the difference between Sanctum and Passport?
- A:
    - Sanctum: Lightweight, SPA/token-based auth.
    - Passport: OAuth2 implementation, heavier.

### Q38: What is API Resource in Laravel?
- A: Transforms models into JSON-friendly output for APIs using `JsonResource`.

### Q39: Difference between `resource()` and `collection()`?
- A: `resource()` is for a single model. `collection()` handles multiple models.

### Q40: What is Laravel Scout?
- A: Full-text search engine integration with Eloquent (e.g., Algolia, Meilisearch).

### Q41: What is Laravel Octane?
- A: Boosts performance using Swoole/RoadRunner — for super-fast apps.

### Q42: What is `artisan tinker`?
- A: REPL for executing Laravel/PHP code interactively.

### Q43: What are value objects in Laravel?
- A: Immutable objects that encapsulate a value with behavior (e.g., Email, Money).

### Q44: How do you create a custom Artisan command?
- A: `php artisan make:command` and define logic inside the `handle()` method.

### Q45: What is a macro in Laravel?
- A: Allows you to add custom methods to built-in classes like Collection, Request.

### Q46: What is dependency injection?
- A: Laravel injects dependencies into constructors or methods automatically using the container.

### Q47: Difference between `@inject`, `app()`, and constructor DI?
- A:
    - `@inject` in Blade
    - `app()` anywhere
    - Constructor DI in controllers/services

### Q48: What is a binding resolution exception?
- A: It occurs when a class or interface is not properly bound in the container.

### Q49: What is Laravel Mix?
- A: A wrapper around Webpack for compiling CSS/JS assets.

### Q50: What’s the purpose of `.env` file?
- A: It stores environment-specific configuration used by `config()` and helpers.

# 🧱 Laravel Interview Questions & Answers

### Q1: What is Laravel?
- A: A PHP web application framework with expressive syntax and MVC architecture.

### Q2: Explain the Laravel request lifecycle.
- A: Request → Middleware → Route → Controller → Response.

### Q3: What is middleware in Laravel?
- A: Filters requests before hitting the route/controller (e.g., auth, csrf).

### Q4: How does routing work in Laravel?
- A: Defined in `routes/web.php` or `api.php` using Route facade.

### Q5: What is a service provider?
- A: Used to bind services in Laravel’s IoC container (`register()` and `boot()` methods).

### Q6: What are facades in Laravel?
- A: Static-like proxies to underlying service container bindings (e.g., `Cache::`, `DB::`).

### Q7: How does Laravel handle authentication?
- A: With built-in scaffolding (`Auth::routes()`), guards, and drivers (session, token).

### Q8: What is the difference between `Auth::` and `Gate::`?
- A: `Auth` checks login; `Gate`/`Policy` checks authorization.

### Q9: What are Laravel policies?
- A: Classes that encapsulate authorization logic for models.

### Q10: What are events and listeners?
- A: Used to decouple logic. Events broadcast state changes, listeners handle them.

### Q11: How to send emails?
- A: Using `Mail::to()->send(new MailableClass)` with `config/mail.php` settings.

### Q12: What is Laravel Sanctum vs Passport?
- A: Sanctum is lightweight for SPA/token auth. Passport is full OAuth2 server.

### Q13: Explain Laravel queues.
- A: Defer heavy tasks using drivers like database, Redis, SQS.

### Q14: What is a job in Laravel?
- A: A queued task class using `php artisan make:job`.

### Q15: How does Laravel handle caching?
- A: With Cache facade, drivers (file, Redis, etc.), and tagged caches.

### Q21: What is route model binding?
- A: Automatically injects Eloquent models into routes.

### Q22: What are migrations and seeders?
- A: Migrations define schema, seeders populate tables with test data.

### Q23: What is form request validation?
- A: Custom request class for validating incoming data.

### Q24: Difference: `hasManyThrough` vs `morphMany`?
- A: `hasManyThrough` connects distant relations; `morphMany` handles polymorphism.

### Q25: What is dependency injection?
- A: Injecting class dependencies via constructors or methods.

### Q26: How does CSRF protection work?
- A: Laravel generates tokens for each session, validated in forms.

### Q27: How to create a custom Artisan command?
- A: `php artisan make:command CustomCommand`.

### Q28: What is broadcasting?
- A: Real-time event delivery to frontend apps using WebSockets.

### Q29: What is Laravel Echo?
- A: JavaScript library to listen to Laravel broadcasted events.

### Q30: How to handle file storage?
- A: Use `Storage` facade with local, S3, FTP, etc.

### Q31: Difference: `storage_path()` vs `public_path()`?
- A: `storage_path()` points to storage dir; `public_path()` to public assets.

### Q32: How to implement localization?
- A: Use `lang` directory, `__()` helper, and `App::setLocale()`.

### Q33: What are Laravel macros?
- A: Custom methods for extending core classes like Collections or Routes.

### Q34: What are jobs and how are they processed?
- A: Async tasks processed by queue workers.

### Q35: How do database transactions work?
- A: Use `DB::beginTransaction()`, `commit()`, and `rollBack()`.

### Q36: What is Laravel Horizon?
- A: Dashboard for managing Redis queues/jobs.

### Q37: How to test routes/controllers?
- A: Use HTTP tests via `get()`, `post()` in `Feature` test classes.

### Q38: Resource Controllers vs Normal Controllers?
- A: Resource: pre-defined CRUD actions. Normal: manual method definition.

### Q39: Laravel performance tips?
- A: Use cache, optimize autoloader, queues, `config:cache`, DB indexing.

### Q40: How to schedule tasks?
- A: Use `Kernel.php` with `schedule()` and set CRON for `php artisan schedule:run`.

### Q41: What is Laravel Telescope?
- A: Debug assistant showing requests, queries, jobs, exceptions.

### Q42: How to use Laravel Mix?
- A: Compile assets using Webpack wrapper with `npm run dev`.

### Q43: Share data across views?
- A: Use `View::share()` or service providers.

### Q44: Difference: `lazy()` vs `cursor()`?
- A: Both avoid memory-heavy loads, but `cursor()` uses generators.

### Q45: Eager vs Lazy Loading?
- A: Eager loads related data up front; Lazy loads on demand.

### Q46: Role of `.env` file?
- A: Holds environment variables like DB, mail, cache config.

### Q47: Multi-auth setup?
- A: Use guards for different user types (e.g., admin, user).

### Q48: How to debug Laravel?
- A: Use `dd()`, `dump()`, `log()`, or debugging tools like Telescope/Xdebug.

### Q49: Boot vs register methods?
- A: `register()` binds services; `boot()` runs after all services are registered.

### Q50: Queues with Redis or DB?
- A: Set `QUEUE_CONNECTION` and use `php artisan queue:work`.

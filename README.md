# Rails 8 - features

Study project to test rails 8 new features!

Major feratures to test! [Rails release notes](https://guides.rubyonrails.org/8_0_release_notes.html)

# Major Features
- [x] Kamal 2
  - Rails now comes preconfigured with Kamal 2 for deploying your application. Kamal takes a fresh Linux box and turns it into an application or accessory server with just a single “kamal setup” command.
Kamal 2 also includes a proxy called Kamal Proxy to replace the generic Traefik option it used at launch.

- [ ] Thruster
  - The Dockerfile has been upgraded to include a new proxy called Thruster, which sits in front of the Puma web server to provide X-Sendfile acceleration, asset caching, and asset compression.

- [ ] Solid Cable
  - Solid Cable replaces Redis to act as the pubsub server to relay WebSocket messages from the application to clients connected to different processes. Solid Cable retains the messages sent in the database for a day by default.

- [ ] Solid Cache
  - Solid Cache replaces either Redis or Memcached for storing HTML fragment caches in particular.

- [ ] Solid Queue
  - Solid Queue replaces the need for Redis, also a separate job-running framework, like Resque, Delayed Job, or Sidekiq.
For high-performance installations, it’s built on the new FOR UPDATE SKIP LOCKED mechanism first introduced in PostgreSQL 9.5, but now also available in MySQL 8.0 and beyond. It also works with SQLite.

- [ ] Propshaft
  - Propshaft is now the default asset pipeline, replacing the old Sprockets system.

- [ ] Authentication
  - Authentication system generator, creates a starting point for a session-based, password-resettable, metadata-tracking authentication system.

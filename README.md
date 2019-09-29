# Ansile role miniflux

[https://miniflux.app/](https://miniflux.app/)

To manage postgres use [https://github.com/ANXS/postgresql](https://github.com/ANXS/postgresql)

## Variables

See defaults/main.yml

```yml
miniflux_user: "miniflux"
miniflux_group: "miniflux"
miniflux_version: "2.0.18"

miniflux_dbname: miniflux
miniflux_dbuser: miniflux
miniflux_dbpassword: ""
miniflux_admin_username: "admin"
miniflux_admin_password: ""
miniflux_base_url: ""
miniflux_pool_size: 5

miniflux_polling_frequency: 60
miniflux_batch_size: 10
miniflux_database_max_conns: 20
miniflux_database_min_conns: 1
miniflux_archive_read_days: 60
miniflux_listen_addr: "127.0.0.1:8080"
miniflux_port: ""
miniflux_cleanup_frequency: 24
miniflux_https: ""
miniflux_disable_hsts: ""
miniflux_disable_http_service: ""
miniflux_disable_scheduler_service: ""
miniflux_cert_file: ""
miniflux_key_file: ""
miniflux_cert_domain: ""
miniflux_cert_cache: "/tmp/cert_cache"
miniflux_oauth2_provider: ""
miniflux_oauth2_client_id: ""
miniflux_oauth2_client_secret: ""
miniflux_oauth2_redirect_url: ""
miniflux_oauth2_user_creation: ""
miniflux_pocket_consumer_key: ""
miniflux_proxy_images: "http-only"

miniflux_database_url: "postgres://{{ miniflux_dbuser }}:{{ miniflux_dbpassword }}@localhost/{{ miniflux_dbname }}?sslmode=disable"
```

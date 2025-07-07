
## 2025-07-04
- `config/environments/test.rb`に`config.action_dispatch.show_exceptions = :none`を指定すると発生した例外が表示されて便利
- 特に`Bullet::Notification::UnoptimizedQueryError`などを表示したいとき

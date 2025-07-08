## 2025-07-08
- open api schema * railsの戦い方
- APIの数が増えてくるとopen api schemaを直接メンテするのがキツくなる（あっという間に一万行近くなる
- 手動で修正するのは難しくなってくるので自動で生成したりlintしたりしないとキツイ
### ツール
- Redocly/redocly-cli: ⚒️ Redocly CLI makes OpenAPI easy. Lint/validate to any standard, generate beautiful docs, and more. https://github.com/Redocly/redocly-cli
- willnet/committee-rails: rails and committee are good friends https://github.com/willnet/committee-rails
- exoego/rspec-openapi: Generate OpenAPI schema from RSpec request specs https://github.com/exoego/rspec-openapi

## 2025-07-04
- `config/environments/test.rb`に`config.action_dispatch.show_exceptions = :none`を指定すると発生した例外が表示されて便利
- 特に`Bullet::Notification::UnoptimizedQueryError`などを表示したいとき

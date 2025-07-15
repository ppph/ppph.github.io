## [2025-07-08] ふつうのrails
- 「ふつうのRailsアプリケーション」についての考え方 - Speaker Deck https://speakerdeck.com/edvakf/hutuufalserailsapurikesiyon-nituitefalsekao-efang?slide=7
- ふつうのRails開発を続けるために - Speaker Deck https://speakerdeck.com/mstshiwasaki/hutuufalserailskai-fa-wosok-kerutameni
- DHHはどのようにRailsのコントローラを書くのか | POSTD https://postd.cc/how-dhh-organizes-his-rails-controllers/
- 「今のプロジェクトいろいろ大変なんですよ、app/services とかもあって……」/After Kaigi on Rails 2024 LT Night - Speaker Deck https://speakerdeck.com/junk0612/after-kaigi-on-rails-2024-lt-night?slide=13


## [2025-07-08] open api schema * rails
- APIの数が増えてくるとopen api schemaを直接メンテするのがキツくなる（あっという間に一万行近くなる
- 手動で修正するのは難しくなってくるので自動で生成したりlintしたりしないとキツイ
### ツール
- Redocly/redocly-cli: ⚒️ Redocly CLI makes OpenAPI easy. Lint/validate to any standard, generate beautiful docs, and more. https://github.com/Redocly/redocly-cli
- willnet/committee-rails: rails and committee are good friends https://github.com/willnet/committee-rails
- exoego/rspec-openapi: Generate OpenAPI schema from RSpec request specs https://github.com/exoego/rspec-openapi

## [2025-07-04] `config.action_dispatch.show_exceptions = :none`
- `config/environments/test.rb`に`config.action_dispatch.show_exceptions = :none`を指定すると発生した例外が表示されて便利
- 特に`Bullet::Notification::UnoptimizedQueryError`などを表示したいとき

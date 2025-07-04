
## 2025-07-04
- `config/environments/test.rb`に`config.action_dispatch.show_exceptions = :none`を指定すると発生した例外が表示されて便利
- 特に`Bullet::Notification::UnoptimizedQueryError`などを表示したいとき
```
config.action_dispatch.show_exceptions = :noneは、RailsのAction Dispatchで例外処理の表示方法を制御する設定です。
設定値の意味：

:none - 例外が発生しても詳細なエラーページを表示せず、シンプルなエラーレスポンスを返します

他の設定値：

:all - 全ての例外の詳細を表示（開発環境のデフォルト）
:rescuable - rescue_fromで処理可能な例外のみ表示（本番環境のデフォルト）

使用場面：

API専用のアプリケーション
カスタムエラーハンドリングを実装している場合
セキュリティ上、例外の詳細を隠したい場合

この設定により、エラーが発生した際にRailsの標準的なエラーページではなく、より制御されたレスポンスを返すことができます。
本番環境でのセキュリティ向上やAPI設計において有用な設定です。
何か具体的な実装について質問があれば、お聞かせください。
```

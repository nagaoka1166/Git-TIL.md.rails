# Git-TIL.md.rails

##railsの構築環境
rails new アプリ名
rails serverでローカルホスト3000を開く。

### トップページを作る

rails generate controller home app　これでブラウザ上にhome#appのトップページができている。
rails generate controller home app　→　viewのファイルが追加される

app --- view
　　　　　    --/home  
                     -top.html.erb
                     
 のようにhtmlファイルが追加される
                  
                          
#ruby on rails 
created_at, update_atは勝手に更新される。
変数　＝ ポスト名.find_by(カラム名:値）
で取りたいデータを抽出できる。
post/"Id"はpost"index"より下に書かないといけない。
ルーティングのpost/○○でurlを作る
コントトーラーでshowを作ってviweのhtml、、？
コントローラーのアクション内ではルーティングで設定したurlの値を取得できる。
params[:id]で取得できる。           

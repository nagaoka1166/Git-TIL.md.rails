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

## 2/13
link.to( URLのタイトル、URL
ルーティング→コントローラー→ビュー

送信されたデータを受け取るルーティング
post "post/create" => "post#create"

受け取ったでーたをurlに送信するform_tagメソッド
<%=　form_tag(送信するURL）　do %>
(controller)
redirect_to(url)で自動的に指定したURLに転送される
@paramsはname="○○”の値を受け取れる
またurlの:○○も受け取れる
order (カラム名：並び替えの秩序）
降順→desc 昇順→asc
order(created_at: :asc

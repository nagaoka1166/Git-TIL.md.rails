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
                  
                          
           

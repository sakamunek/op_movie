# op_movie
自分用コード保存場所
cited by https://qiita.com/qwert-top/items/aa2f385b04de7b702c25



編集したところ
①動画をローカルで保存＆自分のアカウントのドライブにアップロード
自分用のPCに保存した時の（＝ローカルに保存した時の）ファイル名はyoutube.mp4

②パスを修正
特に$HOME_PATH
![image](https://github.com/user-attachments/assets/51b8d9a0-8fcd-480f-9231-49ab09feec7b)
※contentの配下であることに注意
もしファイルが見当たらないときは一つ上のファイルアイコン＋三点リーダーのところをクリック

まとめ
書き換えたのは３点
①ここ↓のパス指定と
![image](https://github.com/user-attachments/assets/87bb65d4-604b-4e22-891a-04f8652f1ed2)

②ここ↓と
※!rm -rf youtube.mp4
!youtube-dl -f 'bestvideo[ext=mp4]' --output "youtube.%(ext)s" https://www.youtube.com/watch?v=$YOUTUBE_ID
の二行は消した
![image](https://github.com/user-attachments/assets/26517145-1acd-44c7-b105-297b93af4afc)

③ここ↓を $OPENPOSE_PATHから $HOME_PATH　へ
![image](https://github.com/user-attachments/assets/b2402d6c-b60e-4953-b0e9-974580d1ac15)



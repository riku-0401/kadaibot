<!DOCTYPE html>
<html>


<body>
    <h1>課題管理 Discord Bot</h1>
    <p>このBOTは複数人で課題を定義、期日まで課題を終えてない人を毎日メンションをし、課題を期日までに出すことを目的としたBOTです</p>
    <p>また、期日が明日の課題を取り組んでいる最中の人のメンションを添えてお知らせします</p>
    <p>tukaikata.txtはチャンネル名や用途に合わせてUTF-8でカスタムしてください</p>
    <p>以下のようにmain.py内の上にあるチャンネルid、サーバーid、トークンを代入してください</p>
    <hr>
    <pre>
        #############################################
        # サーバーのチャンネルid、サーバーid、トークン設定
        tukaikatachid = 0
        kadaichid = 0
        cmdchid = 0
        osirasechid = 0
        kanrishachid = 0 # 管理用
        logchid = 0     # 管理用
        guildid = 0     # サーバーid
        TOKEN = "YOUR TOKEN" # トークン設定
        #############################################
    </pre>
    <h2>コマンド一覧</h2>
    <ul>
        <li><code>!o 課題名 期日</code> (cmdchidチャンネルのみ) 課題の定義 例. <code>!o C言語 0910</code></li>
        <li><code>!sss</code> (kanrishachidチャンネルのみ) 使い方をtukaikata.txtから読み取り、tukaikatachidに送信</li>
        <li><code>!reset</code>  (kanrishachidのみ) 課題ファイルの削除</li>
    </ul>
    <p><big>以下のコマンドは日付変更時に自動で実行されるので通常実行する必要はないです</big></p>
    <ul>
        <li><code>!ff </code> (kanrishachidチャンネルのみ) ３日前が期日の課題をデータから削除</li>
        <li><code>!fc </code> (kanrishachidチャンネルのみ) 明日が期日の課題を表示、取り組んでいる人をメンション</li>
        <li><code>!fs </code> (kanrishachidチャンネルのみ) 課題に取り組んでいるユーザーごとの課題一覧を送信</li>
    </ul>
    <p>通常これら3つのコマンドは日付が変わって数分後に自動で実行されます</p>

![2023-09-10_01h53_33](https://github.com/riku-0401/kadaibot/assets/131428274/154e4bb6-22b9-4e7f-9309-5e4cc2ede4b3)
![2023-09-10_01h53_40](https://github.com/riku-0401/kadaibot/assets/131428274/ac15d711-5ae7-4d0b-afdf-bc15c7797363)
![2023-09-10_01h56_41](https://github.com/riku-0401/kadaibot/assets/131428274/7d571773-4761-4f91-bf20-77c66001e8d7)
![43565](https://github.com/riku-0401/kadaibot/assets/131428274/11d7d44d-0171-46e0-9ded-db0ebf5b0790)
</body>
</html>

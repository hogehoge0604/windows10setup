# Windows10 初期設定

## 前提
- Windows 10 Pro

## Windowsの設定
1. システムの復元の有効化
    1. タスクバーの検索窓から「回復」で検索し画面を表示する
    2. 「システムの復元」を選択する
    3. 保護が「有効」になっていない場合「構成」を選択し以下の設定を変更する
        - システムの保護を有効にする
        - ディスク領域の使用量を5%に設定する
    4. 「作成」を選択し復元ポイントを作成する

2. システムの復元のスケジュール設定変更
    1. タスクバーの検索窓から「タスクスケジューラ」で検索し画面を表示する
    2. 「タスクスケジューラライブラリ」→「Microsoft」→「Windows」→「SystemRestore」を選択する
    3. 「タスクの作成」から新規タスクを作成する
    4. 「全般」を選択し以下設定を追加する
        - 名前: SR_TIMER
        - 「最上位の特権で実行する」にチェックを付与する
        - 構成: Windows 10
    5. 「トリガー」を選択し以下の設定を追加する
        - タスクの開始：毎日
        - 開始: 11:00:00
    6. 「条件」を選択し以下の設定を変更する
        - 「次の間アイドル状態の場合のみタスクを開始する」のチェックを外す
        - 「コンピューターをAC電源で使用している場合のみタスクを開始する」のチェックを外す
    7. 「設定」を選択し以下の設定を変更する
        - 「スケジュールされた時刻にタスクを開始できなかった場合、すぐにタスクを実行する」にチェックを付与する

3. Cortanaを無効化する
    1. タスクバーの検索窓から「グループポリシー」で検索し画面を表示する
    2. 「管理用テンプレート」→「Windowsコンポーネント」→「検索」→「Cortanaを許可する」を選択し「無効」に変更する

## ツール類

### ブラウザ
- Google Chrome
    - https://www.google.com/intl/ja_ALL/chrome/

### エディタ
- VSCode
    - https://code.visualstudio.com/
    
    - プラグイン
        - Japanese Language Pack for Visual Studio Code
            - 日本語化
        - PHP IntelliSense
            - PHPのコード補完
        - Markdown All in One
            - Markdownの編集に便利な拡張機能
        - Docker
            - VSCodeでDockerをサポートする
        - code-eol
            - 改行コードの視覚化

### FTP
- WinSCP
    - https://ja.osdn.net/projects/winscp/

### SSH
- RLogin
    - http://nanno.dip.jp/softlib/man/rlogin/

### PHP
- PHP
    - https://windows.php.net/download#php-7.2

- Composer
    - https://getcomposer.org/doc/00-intro.md#installation-windows

### 開発周辺ツール
- Docker
    - https://store.docker.com/editions/community/docker-ce-desktop-windows

- Git Bash
    - https://gitforwindows.org/

### その他
- 付箋紙
    - Sticky Notes
    - Windows 標準

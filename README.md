# 将棋大会運営ツール

将棋大会の参加者登録、組み合わせ作成、対局結果、成績・順位の管理を支援するWindows向けアプリです。

## 公開状況

最新版：`v.0.2.0-beta`（初版β）

公開日：`2026-10-13`

[v.0.2.0-betaの配布ページ](https://github.com/ryo-app/shogi-tournament-manager/releases/tag/v.0.2.0-beta)から取得できます。変更内容は [CHANGELOG.md](CHANGELOG.md)、ZIPの検証値は [SHA256SUMS.txt](SHA256SUMS.txt) を参照してください。

配布ZIP名：`ShogiTournamentManager-v.0.2.0-beta-windows-x64.zip`。

## ダウンロード・起動方法

1. Releasesで対象バージョンの説明と利用条件を確認し、Windows x64向けZIPをダウンロードします。
2. PowerShellの `Get-FileHash -Algorithm SHA256 -LiteralPath 'ダウンロードしたZIPのパス'` でSHA256を確認し、対象バージョンのSHA256SUMSと照合します。
3. ZIP全体を展開します。`Launcher.exe` だけを移動せず、同梱フォルダーを保持してください。Pythonの別途インストールは不要です。
4. 起動前に、下記の利用条件と同梱文書を確認してください。
5. `Launcher.exe` を起動し、初回に大会データの保存先を選択します。アプリの展開先とデータ保存先は分けてください。
6. 終了時は管理画面の「終了」を使用します。大会データは定期的にバックアップしてください。

## 利用条件

無料で利用できる独自フリーウェアです。オープンソースとしての配布ではありません。**利用前にZIP内の `_internal/distribution/EULA.txt` を読み、同意した場合のみ使用してください。** 利用・再配布の条件はEULA本文によります。以下の同梱パスは、展開された `ShogiTournamentManager` フォルダーを基準とします。

第三者コンポーネントにはそれぞれのライセンスが優先します。ZIP内の `_internal/distribution/THIRD_PARTY_NOTICES.md`、同ディレクトリの `NATIVE_NOTICES.txt`、同ディレクトリの `licenses`（ライセンス本文）と `sources`（対応ソース）を確認してください。再配布時も公式配布物と同梱文書を保持してください。

## β版の動作環境に関する注意

本ソフトウェアは**β版**です。開発環境では基本的な起動・大会管理・保存・バックアップ等を確認していますが、**クリーンなWindows環境、標準ユーザーアカウント、実際にダウンロードしたZIPでのWindowsのセキュリティ警告（SmartScreen等）については未検証**です。別PCでのバックアップ復旧も未検証です。このバージョンのOS全体オフライン動作、8時間連続運転、一部管理画面操作も実機検証が完了していません。すべてのWindows環境での正常動作を保証するものではありません。

初めて利用する環境では、実際の大会データを入力する前に、起動・保存・再起動・バックアップ・復元を試験用データで確認してください。Windowsの警告やブロックが表示された場合は、その内容を確認し、**セキュリティ保護機能を無効化してまで起動しないでください**。重要な大会データは定期的にバックアップしてください。

## 問い合わせ

- [Bluesky](https://bsky.app/profile/ryo-engineer.bsky.social)
- [note](https://note.com/morino_kuma_note)

GitHub Issuesは一般利用者向けの問い合わせ窓口として使用しません。問い合わせに実大会の個人情報やデータを添付しないでください。

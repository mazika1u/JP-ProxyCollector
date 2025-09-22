# JP-ProxyCollector

JP-ProxyCollector は、web上に公開されている無料Proxylistから
IP:PORT を収集し、日本（JP）の出口IPのみを検証・抽出する Python toolです。

## 特徴
- 複数のソースURLから自動でプロキシをスクレイピング
- BeautifulSoup による HTML/テキスト解析
- aiohttp を用いた非同期プロキシ検証
- ip-api.com を利用して国コードを判定
- JP プロキシのみ抽出して保存

## 必要なこと
```bash
sources.txtにproxy提供しているサイトURLを記載必要


## 使い方
```bash
pip install -r requirements.txt
python main.py --sources sources.txt --out all.txt --out-jp jp.txt --concurrency 80 --timeout 8

# yaml-golang 
yaml-golang は、Golang で動作する(マイクロサービス)ランタイムにおいて、yaml に当該(マイクロサービス)ランタイム固有の処理方法等を定義する場合の、記載方法を記したレポジトリです。  
Golangの場合、ライブラリの依存関係を共通レポジトリで構築できないため、AIONでは、Golangランタイムにおける 当該定義 の適用をマイクロサービス毎に定義しています。  

## 動作環境

* OS: Linux  
* CPU: ARM/AMD/Intel  
* Golang Runtime  

## Golang(マイクロサービス)ランタイム における yaml処理定義 の適用方法  

Golang(マイクロサービスランタイム)環境で yaml にて　ランタイム(マイクロサービス)固有の処理方法を定義する場合は、go.modに以下のように記載します。  
```
module MODULE-NAME

go 1.17

require (
	gopkg.in/yaml.v2 v2.3.0
)
```
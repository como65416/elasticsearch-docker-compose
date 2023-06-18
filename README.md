# Elasticsearch Docker Compose 範例

使用 Docker Composer 啟動 Elasticsearch 並且安裝中文分詞的範例

在 .env 內修改 elasticsearch 版本時需要注意 elasticsearch-analysis-ik 以及 elasticsearch-analysis-stconvert 是否有對應的版本

不然會安裝不起來

- https://github.com/medcl/elasticsearch-analysis-ik/releases

- https://github.com/medcl/elasticsearch-analysis-stconvert/releases

如果是只要測試使用沒有要走 https 的話

需要將 `xpack.security.http.ssl.enabled` 改為 false (docker-composer.yaml)

並且將相關連線的 https 改成 http


 复制服务器文件到本地

`rsync -chavzP --stats mituresdev@106.15.202.29:~/server/deploy.sh ~/cache`

复制本地文件到服务器
`rsync -ar ~/cache/test.sh mituresdev@106.15.202.29:~/server/path`


ssserver -c /etc/shadowsocks.json -d start
ssserver -d stop
sudo ssserver -d stop

### install [shadowsocks-libev]

1. run:  sudo vim /etc/apt/sources.list
2. add:  deb http://ftp.debian.org/debian stretch-backports main
3. run:  apt update
4. run:  apt -t stretch-backports install shadowsocks-libev
5. 
启动： ss-server -s 0.0.0.0 -p 444 -k [password] -m aes-256-cfb -d 8.8.8.8 -u --fast-open --no-delay --mptcp -f /run/sss444.pid

### example: 

注： psd+v

```bash
ss-server -s 0.0.0.0 -p 446 -k saV3kGJSssQwxQGv -m chacha20-ietf-poly1305 -d 8.8.8.8 -u --fast-open --no-delay --mptcp -f /run/sss446.pid
ss-server -s 0.0.0.0 -p 445 -k saV3kGJSssQwxQGv -m aes-256-gcm -d 8.8.8.8 -u --fast-open --no-delay --mptcp -f /run/sss445.pid
ss-server -s 0.0.0.0 -p 444 -k saV3kGJSssQwxQGv -m aes-256-cfb -d 8.8.8.8 -u --fast-open --no-delay --mptcp -f /run/sss444.pid

ss-server -s 0.0.0.0 -p 404 -k nPqJbXnX6VBqRYjv -m aes-256-cfb -d 8.8.8.8 -u --fast-open --no-delay --mptcp -f /run/sss404.pid
ss-server -s 0.0.0.0 -p 405 -k nPqJbXnX6VBqRYjv -m aes-256-gcm -d 8.8.8.8 -u --fast-open --no-delay --mptcp -f /run/sss405.pid
ss-server -s 0.0.0.0 -p 406 -k nPqJbXnX6VBqRYjv -m chacha20-ietf-poly1305 -d 8.8.8.8 -u --fast-open --no-delay --mptcp -f /run/sss406.pid
ss-server -s 0.0.0.0 -p 407 -k nPqJbXnX6VBqRYjv -m xchacha20-ietf-poly1305 -d 8.8.8.8 -u --fast-open --no-delay --mptcp -f /run/sss407.pid
```




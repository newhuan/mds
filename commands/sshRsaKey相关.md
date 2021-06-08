### login with rsa pubkey(without password):

ssh-copy-id -i [local pubkey path] [userName]@[remote ipAddress]

pubkey path usually: .ssh/id_rsa.pub

### create rsa key:

ssh-keygen

ssh-keygen -f "/home/xox/.ssh/known_hosts" -R "106.15.199.117" 


# output

```
starting thread (client mode): 0x4e2232e8
Local version/idstring: SSH-2.0-paramiko_2.7.2
Remote version/idstring: SSH-2.0-OpenSSH_8.1
Connected (version 2.0, client OpenSSH_8.1)
kex algos:['curve25519-sha256', 'curve25519-sha256@libssh.org', 'ecdh-sha2-nistp256', 'ecdh-sha2-nistp384', 'ecdh-sha2-nistp521', 'diffie-hellman-group-exchange-sha256', 'diffie-hellman-group16-sha512', 'diffie-hellman-group18-sha512', 'diffie-hellman-group14-sha256', 'diffie-hellman-group14-sha1'] server key:['rsa-sha2-512', 'rsa-sha2-256', 'ssh-rsa', 'ecdsa-sha2-nistp256', 'ssh-ed25519'] client encrypt:['chacha20-poly1305@openssh.com', 'aes128-ctr', 'aes192-ctr', 'aes256-ctr', 'aes128-gcm@openssh.com', 'aes256-gcm@openssh.com'] server encrypt:['chacha20-poly1305@openssh.com', 'aes128-ctr', 'aes192-ctr', 'aes256-ctr', 'aes128-gcm@openssh.com', 'aes256-gcm@openssh.com'] client mac:['umac-64-etm@openssh.com', 'umac-128-etm@openssh.com', 'hmac-sha2-256-etm@openssh.com', 'hmac-sha2-512-etm@openssh.com', 'hmac-sha1-etm@openssh.com', 'umac-64@openssh.com', 'umac-128@openssh.com', 'hmac-sha2-256', 'hmac-sha2-512', 'hmac-sha1'] server mac:['umac-64-etm@openssh.com', 'umac-128-etm@openssh.com', 'hmac-sha2-256-etm@openssh.com', 'hmac-sha2-512-etm@openssh.com', 'hmac-sha1-etm@openssh.com', 'umac-64@openssh.com', 'umac-128@openssh.com', 'hmac-sha2-256', 'hmac-sha2-512', 'hmac-sha1'] client compress:['none', 'zlib@openssh.com'] server compress:['none', 'zlib@openssh.com'] client lang:[''] server lang:[''] kex follows?False
Kex agreed: curve25519-sha256@libssh.org
HostKey agreed: ecdsa-sha2-nistp256
Cipher agreed: aes128-ctr
MAC agreed: hmac-sha2-256
Compression agreed: none
kex engine KexCurve25519 specified hash_algo <built-in function openssl_sha256>
Switch to new keys ...
userauth is OK
Authentication (password) failed.

Traceback (most recent call last):
  File "log_string.py", line 23, in <module>
    client.connect('192.168.2.249', username='melissali', password='wrongpassword', look_for_keys=False)
  File "/home/melissali/Downloads/venv/lib64/python3.6/site-packages/paramiko/client.py", line 446, in connect
    passphrase,
  File "/home/melissali/Downloads/venv/lib64/python3.6/site-packages/paramiko/client.py", line 764, in _auth
    raise saved_exception
  File "/home/melissali/Downloads/venv/lib64/python3.6/site-packages/paramiko/client.py", line 751, in _auth
    self._transport.auth_password(username, password)
  File "/home/melissali/Downloads/venv/lib64/python3.6/site-packages/paramiko/transport.py", line 1509, in auth_password
    return self.auth_handler.wait_for_response(my_event)
  File "/home/melissali/Downloads/venv/lib64/python3.6/site-packages/paramiko/auth_handler.py", line 250, in wait_for_response
    raise e
paramiko.ssh_exception.AuthenticationException: Authentication failed.

```

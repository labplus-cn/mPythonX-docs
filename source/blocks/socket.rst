网络
====


usocket.socket(af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP)
-------------

**描述：**   构建对象

**参数：**

- ``af`` - 地址。
  - ``socket.AF_INET``：=2 — TCP/IP – IPv4；
  - ``socket.AF_INET6``：=10 — TCP/IP – IPv6
- ``type`` - socket 类型。``socket.SOCK_STREAM``：=1 — TCP 流；``socket.SOCK_DGRAM``：=2 — UDP 数据报；``socket.SOCK_RAW``：=3 — 原始套接字；``socket.SO_REUSEADDR``：=4 — socket可重用
- ``proto`` - 协议号。``socket.IPPROTO_TCP``：=6；``socket.IPPROTO_UDP``：=17。一般不指定proto参数，因为有些MicroPython固件提供默认参数


usocket.getaddrinfo(host, port)
-------------

**描述：**   将主机域名（host）和端口（port）转换为用于创建套接字的5元组序列。元组列表的结构: (family, type, proto, canonname, sockaddr)


socket.close()
-------------

**描述：**   关闭 socket。一旦关闭后，socket 所有的功能都将失效。远端将接收不到任何数据 (清理队列数据后)。 内存碎片回收时 socket 会自动关闭，但还是推荐在必要时用 close() 去关闭


socket.bind(address)
-------------

**描述：**   以列表或元组的方式绑定地址和端口号

**参数：**

- ``address`` - 一个包含地址和端口号的列表或元组


socket.listen([backlog])
-------------

**描述：**   监听 socket，使服务器能够接收连接。如果指定了 backlog ，它不能小于0 (如果小于0将自动设置为0)； 超出后系统将拒绝新的连接。如果没有指定，将使用默认值

**参数：**

- ``backlog`` - 接受套接字的最大个数，至少为0，如果没有指定，则默认一个合理值


socket.accept()
-------------

**描述：**   接收连接请求。socket 需要指定地址并监听连接。返回值是 (conn, address)， 其中 conn 是用来接收和发送数据的套接字，address 是绑定到另一端的套接字


**参数：**

- ``conn`` - 新的套接字对象，可以用来收发消息
- ``address`` - 连接到服务器的客户端地址


socket.connect(address)
-------------

**描述：**   连接到指定地址的服务器

**参数：**

- ``address`` - 服务器地址和端口号的元组或列表


socket.send(bytes)
-------------

**描述：**   发送数据，并返回发送的字节数

**参数：**

- ``bytes`` - bytes 类型数据


socket.sendall(bytes)
-------------

**描述：**   与 send() 函数类似，区别是 sendall() 函数通过数据块连续发送数据

**参数：**

- ``bytes`` - bytes 类型数据


socket.recv(bufsize)
-------------

**描述：**   接收数据，返回接收到的数据对象

**参数：**

- ``bufsize`` - 指定一次接收的最大数据量



socket.sendto(bytes, address)
-------------

**描述：**   发送数据，目标由 address 决定，用于 UDP 通信，返回发送的数据大小

**参数：**

- ``bytes`` - bytes 类型数据
- ``address`` - 目标地址和端口号的元组


socket.recvfrom(bufsize)
-------------

**描述：**   接收数据，用于 UDP 通信，并返回接收到的数据对象和对象的地址

**参数：**

- ``bufsize`` - 指定一次接收的最大数据量


socket.setsockopt(level, optname, value)
-------------

**描述：**   根据选项值设置 socket

**参数：**

- ``level`` - 套接字选项级别
- ``optname`` - socket 选项
- ``value`` - 可以是一个整数，也可以是一个表示缓冲区的bytes类对象


socket.settimeout(value)
-------------

**描述：**   设置超时时间，单位：秒


socket.setblocking(flag)
-------------

**描述：**   设置 socket 的阻塞或非阻塞模式：若标记为 False，则将该 socket 设置为非阻塞模式


socket.read([size])
-------------

**描述：**   从 socket 中读取 size 字节。返回一个字节对象。若未给定 size ，则按照类似 socket.readall() 的模式运行


socket.readinto(buf[, nbytes])
-------------

**描述：**   将字节读取入缓冲区。若指定 nbytes ，则最多读取该数量的字节。否则，最多读取 len(buf) 数量的字节。 正如 read() ，该方法遵循“no short reads”方法
**返回值：**   读取并存入缓冲区的字节数量


socket.readline()
-------------

**描述：**   接收一行数据，遇换行符结束，并返回接收数据的对象


socket.write(buf)
-------------

**描述：**   向字节缓冲区写入socket，并返回写入数据的大小

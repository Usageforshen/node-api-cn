<!-- YAML
added: v14.11.0
-->

* {number} **Default:** `0`

Sets the timeout value in milliseconds for receiving the entire request from
the client.

If the timeout expires, the server responds with status 408 without
forwarding the request to the request listener and then closes the connection.

It must be set to a non-zero value (e.g. 120 seconds) to proctect against
potential Denial-of-Service attacks in case the server is deployed without a
reverse proxy in front.


----------------------------------
* {number} **Default:** `0`

以毫秒为单位设置从客户端接收的整个请求的超时值。
如果超时过期，则服务器会以408状态响应而不将请求转发给请求侦听器，然后关闭连接。
必须将其设置为非零值（例如120秒）以防止在部署服务器时前面没有反向代理的情况下发生潜在的拒绝服务攻击。

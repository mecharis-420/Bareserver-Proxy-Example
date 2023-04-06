<div align="center">
<h1>Bareserver-Proxy-Example</h1>
<h3>An example of using a external bareserver (TompHTTP) with Ultraviolent.</h3>
</div>
<h2>Changing Bare Server</h2>
In /uv/uv.config.js change the https://tcgrjc-8080.csb.app/ part to your prefered bare server.
```
self.__uv$config = {
    prefix: '/service/uv/',
    bare: 'https://tcgrjc-8080.csb.app/',
    encodeUrl: Ultraviolet.codec.xor.encode,
    decodeUrl: Ultraviolet.codec.xor.decode,
    handler: '/uv/uv.handler.js',
    bundle: '/uv/uv.bundle.js',
    config: '/uv/uv.config.js',
    sw: '/uv/uv.sw.js',
};
```

#esno // 可以直接执行esm的文件的命令


/**
 * 1. 起一个 node 服务
 * 2. 模版项目的文件，就都走静态资源路径了
 * 3. html 返回
 * 4. html 返回之前呢，塞一个 client 进去，<script src="/@vite/client" type="module"/>
 * 5. 写这个接口 /vite/client -> 内置的 client.js -> HMR
 * 6. server - websocket - client
 * 7. 监听文件变更（三方库）-> 封装一个数据结构（变更） -> websocket -> client
 * 8. 其它文件 .css .jsx 的处理
 * 9. css -> js -> createElement('style') -> header
 * 10. .jsx -> .js (引用三方，本地) / 三方（缓存） + 本地（拼路径）
 * 11. plugin 系统等
 */

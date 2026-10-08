### 卢思文 · lusiwen3742

后端开发，做权限控制系统。  
把角色、权限、资源拆清楚，而不是堆一屋子 `if-else`。

  


## 在做的事

**[rbac-demo](https://github.com/lusiwen3742-png/rbac-demo)**  —  最小可运行的 RBAC 示例

一条完整的权限链路：`POST /login` 签发 JWT，请求头带 `Authorization: Bearer <token>`  
完成认证，再用权限字符串精确控制每个接口。提供 Node.js/Express 与 PHP 两套实现对照，  
`public/` 是静态前端，浏览器打开就能登录测试。

| 接口            | 所需权限        |
| :------------ | :---------- |
| `POST /login` | —           |
| `GET /me`     | 需登录         |
| `GET /users`  | `user.read` |
| `GET /roles`  | `role.read` |

```bash
npm install && npm start     # → http://localhost:3000/
```

<sub>演示账号　`admin` / `123456`（全部权限）　`alice` / `123456`（仅 user.read）</sub>

  


## 技术栈

**语言**　JavaScript · PHP · HTML/CSS  
**后端**　Node.js · Express · JWT · bcrypt  
**数据**　MySQL  
**工具**　Git · VS Code · npm

<sub>关注方向：系统架构 · API 安全</sub>

  


## 贡献记录

![Contribution graph](https://ghchart.rshah.org/1f6feb/lusiwen3742-png)

<sub>仓库刚起步，绿格会慢慢长出来。</sub>

  


---

<sub>📮 <lusiwen3742@gmail.com>　·　欢迎交流后端架构与 API 安全</sub>

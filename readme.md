# student-api

## Install

```bash
npm install --save student-api
```

## Usage

Đây là một ví dụ cào dữ liệu từ [TLU](http://dkh.tlu.edu.vn/).

```js
const StudentAPI = require("student-api");

const api = new StudentAPI();

await api.Login({ id: "xxx", pass: "xxx" });
await api.Close();
```

## API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

- [StudentAPI](#studentapi)
  - [isAuthenticated](#isauthenticated)
  - [user](#user)
  - [browser](#browser)
  - [Login](#signup)
  - [StudentTimeTable](#studenttimetable)
  - [TimeLineByDay](#timelinebyday)

### [StudentAPI](https://github.com/2ksoft/student-api/blob/master/index.js#L10-L13)

Type: `function (opts)`

- `opts` **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** Options (optional, default `{}`)
  - `opts.browser` **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)?** Puppeteer browser instance to use
  - `opts.puppeteer` **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)?** Puppeteer [launch options](https://github.com/GoogleChrome/puppeteer/blob/master/docs/api.md#puppeteerlaunchoptions)

---

#### [isAuthenticated](https://github.com/2ksoft/student-api/blob/master/index.js#L15-L17)

Kiểm tra đăng nhập thành công hay không ?

Type: [boolean](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean)

---

#### [user](https://github.com/2ksoft/student-api/blob/master/index.js#L18-L20)

Trả về user đã đăng nhập thành công

Type: [Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)

---

#### [browser](https://github.com/2ksoft/student-api/blob/master/index.js#L21-L27)

Khởi chạy browser headless.

Type: `function ()`

---

#### [Login](https://github.com/2ksoft/student-api/blob/master/index.js#L28-L36)

Automates the creation of a new Instagram account.

Type: `function (user, opts): Promise`

- `user` **[object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** Tài khoản
  - `user.id` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Tên tài khoản
  - `user.pass` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** Mật khẩu
- `opts` **[object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** Options (optional, default `{}`)

---

#### [TimeLineByDay](https://github.com/2ksoft/student-api/blob/master/index.js#L44-L49)

Trả về lịch học được nhóm theo ngày

Type: [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

---

#### [Close](https://github.com/2ksoft/student-api/blob/master/index.js#L50-L56)

Closes the underlying browser instance, effectively ending this session.

Type: `function (): Promise`

---

## Related

- [puppeteer](https://github.com/GoogleChrome/puppeteer) - Headless Chrome Node API.

## License

MIT © [2KSOFT](https://github.com/2ksoft)

Support my OSS work by <a href="https://github.com/2ksoft">following me on github <img src="https://www.logolynx.com/images/logolynx/s_9f/9f3291b441a7a67de3d52ce601b507c9.png" alt="twitter" height="24px" align="center"></a> <a href="https://fb.me/hanhgoogle">following me on facebook <img src="https://mapstr-prod.s3.amazonaws.com/298ed6c57ada2a7560d24dabba452548_facebook-logo-F-1200x816.jpg" alt="twitter" height="24px" align="center"></a>
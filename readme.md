<h1 valign="middle">
    <img src="https://console.trustocean.com/templates/lagom/assets/img/logo/logo_big.svg"  valign="middle" width="280">
    <span style="font-size:28px" valign="middle">𝑨𝑪𝑴𝑬 𝑺𝑬𝑹𝑽𝑬𝑹</span>
</h1>

一个 [TrustOcean API](https://api.trustocean.com/?from=github-trustocean-acme) 转 [ACME API](https://tools.ietf.org/html/draft-ietf-acme-acme-09) 的项目。

客户端：[trustocean/acme-client](https://github.com/trustocean/acme-client/)


## 安装

```bash
git clone https://github.com/trustocean/acme-server.git ./
composer install
cp .env.example .env
vim .env # 修改其中的 DB_ 开头的数据库连接信息
php artisan migrate
php artisan key:generate
php artisan serve
```
修改 `.env` 中的 TRUSTOCEAN_USERNAME 和 TRUSTOCEAN_PASSWORD 为你本人的 trustocean 的账号。

然后将你的 acme 客户端的 api endpoint 修改成 localhost，即可正常使用。


## 完成度

- [x] 账户注册
- [x] 证书下单
- [x] 证书域名验证
- [x] 证书签发
- [ ] 证书撤销


## License

MIT

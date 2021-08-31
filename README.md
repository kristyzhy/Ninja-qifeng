# Ninja

Ninja 仅供学习参考使用，请于下载后的 24 小时内删除，本人不对使用过程中出现的任何问题负责，包括但不限于 `数据丢失` `数据泄露`。
CK登录 需后台有原CK(过期的也行) 输入新CK显示`欢迎回来XXX`证明更新成功 不可新增账号

## 常用指令

```bash
docker exec -it qinglong bash
cd /ql && git clone https://github.com.cnpmjs.org/QiFengg/Ninja-qifeng.git
cd /ql/Ninja-qifeng/backend
pnpm install
cp sendNotify.js /ql/scripts/sendNotify.js
pm2 start

cd /ql/Ninja-qifeng
git pull
cd /ql/Ninja-qifeng/bakcend
pm2 restart
```

## 配置文件

`推送二维码请放在 /backend/static 重命名为push.jpg`

```bash
# 是否允许添加账号 不允许添加时则只允许已有账号登录
ALLOW_ADD=true
#允许添加账号的最大数量
ALLOW_NUM=50
# Ninja 运行端口
NINJA_PORT=5701
# Ninja 是否发送通知
NINJA_NOTIFY=true
# user-agent
NINJA_UA=""
```

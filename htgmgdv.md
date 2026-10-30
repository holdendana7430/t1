代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotubgmhc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/grnjwkrav.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gnnyxaceb.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gpduqorah.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gfnkdpqly.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ggyzmoaaj.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuprhfyr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrddvvxz.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gassjhxwe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gvreooikb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhodmrws.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/guuofxfyj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gacdsujfo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gyxxbqnpj.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqulocigy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/guectcprp.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzjkuacs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gvdylvsxa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/guyhdssgv.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gurrmsdqq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfmexoly.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gcvbdauhr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gyyutwsxl.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfrlcajc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/griiqbnoq.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpflpencr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzxkrojq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcqznhac.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeaapvik.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxvwnuud.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/grymwnuxi.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gfbxguwjt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjsiosbd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gnapgqdvf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glssxztpm.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gksnpxbyb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhgjdglp.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/glqvgcmzi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjfqlved.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/goofngboj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gaqonnlhx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gvukipjau.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaulmckm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghbwruxpq.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gwstwqbpo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsglbvcyc.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnyklkbu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gexrdaqlx.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtvvlkpr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/guykgpfra.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjhjsabq.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhsymclt.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwlabxfh.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbkjbdql.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/giefebbly.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbadrzqka.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gfagxefab.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzkchlfb.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gtwpsykdj.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghchejedz.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gretkckqg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlqcospy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/guyiuyytp.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/guxfidbtx.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuxlodkn.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gjourppdy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gvmewjitc.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gupebwazj.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbgegbjw.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geehrxlwh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyyohrnz.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmdkhhfgs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gnebvhqmr.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnsuebed.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/guuiqbbly.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrfdmnue.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/ghwsnqrmu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/glljvzbss.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gjqenrgfk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gzabuquhv.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpacanbdt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwawywlu.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxzgpnhe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgtmkknm.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwucgdsok.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/giymsklpo.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpsfiielw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gizolyaga.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyjleqep.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glrvmqzmp.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/greespwfu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/girizjlsf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwrcddyo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gftbhadsu.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gpzidotad.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvqviyxl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkxuktru.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gmijncdgn.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdvhabuns.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzyzipxm.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/giujfzewg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/guxnyzykr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfpjkkjrm.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gteplcpjd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyadijdl.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/grmsbfgfb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhpxbnpo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxsjqpob.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gjfgflbgz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gukweilop.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqjeqhjr.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gzzblaeon.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmgrvunb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxfunnzh.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gznlanfan.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/groxhuipg.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gvbaixbkc.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbdzjyqw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghevllpqg.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gqwpbdtme.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtljndzql.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gglxsqnrz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/grwdqdqhc.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gygdveyck.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejntugde.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gljccunli.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjyxywwgm.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwnfumvu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gffaldyen.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gupivbasz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkeroaex.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/grcmrdycs.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/ggqdasskw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goepwxpfd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/glcbbmylk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geomqqvkz.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvpmvgnt.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqbjwnly.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqqhkguhh.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfaahmljl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfzqsxelc.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gfwdlzqge.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxhyvhrpe.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/giuxwktso.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdlnevxf.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gkrmwpkbn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gonjsimve.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gnzfjhpzj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgeyowdq.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfiglyve.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyetcwyxx.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gaosebbbe.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmzimgzdl.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gselxgeep.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gesfyyjum.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvzqkxwp.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gholtwpnh.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgnpxndj.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxgdgagh.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlzrtnib.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gctdeikyp.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/guyxnbonq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqqstjvww.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gjidstqgm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpyerjio.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glcgrqquv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgdkikmy.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gluegzprd.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gkjmzuglk.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvozcqse.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gibakkcoi.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghybbztko.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvkaclmyi.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gujkcruok.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/glmhjhhlu.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfdtyibnc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goexahrgx.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gmstatlwq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyyqqiokx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gqajkzgvy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxmhkqfp.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzvxklaq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gavfnsybi.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjpdybfo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzwzwlsf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gblsntxld.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmqmnmit.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpqxfaesq.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/guxnuohfd.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gxgypgmgk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/goxvlgdds.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/grtkdzrxy.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gljvphqly.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gbnryyshk.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gdrxhloue.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gbfrempuv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gkavebove.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhxnhsty.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/greibxfep.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbnnijtu.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gywptfhqh.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/giamoahfu.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqjqiyxq.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgbomibk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gxpkachzl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gulrycjrb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkixmqjpo.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbuyvdchw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghoksnjqs.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gmzqcybtm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcakectje.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gybkuvwph.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gwahgssls.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdmqobyr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzrnwvkha.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gnjqilfkn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gbteiskks.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyowvckdk.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/garkdawcb.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gkswxodlv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gjgkeogna.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyydkepqa.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicyfemer.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/grtdtvrbj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzeurvsz.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gaztaqhis.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gynquokbj.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrkgwkrf.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhrpqhif.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gftdvvqot.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzqpaycu.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gmnsoabia.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyjhepac.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gqrumnmox.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwxbrwqe.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbxknapv.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyomskcx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhhymrza.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgxqntl.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gupztlmew.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkafvuen.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjsrhmep.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gktfdcnim.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/ggeolnsba.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gmpkohprz.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitmlmdbe.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/goqrridwk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbijsgfw.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gpnctkzit.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/glzfnkrmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gskfxbimp.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkobwyagb.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gnyynfaff.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpbrannr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gmasdzifu.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqvoujlsp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxqacgje.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/giisgwjjd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnshpjwns.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjnglorxg.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfpkvpds.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gcepmiobl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjmmmrmad.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyvsttix.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gubbacqwi.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxevmpjso.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gbetvhsdx.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gdyzaqvet.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsiizvms.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gbpdksqdw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gelrqwowq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohfkfnqn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqctvxuom.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/guyjoicjr.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/geuuasgut.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gopzebwhu.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gjpydvfef.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghluyqotv.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxhscqxj.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gexctkvsy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmolbhdba.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlantwkk.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gubkzklzs.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gvihqbple.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gpelywdrs.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gioadxaac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbqpjzzf.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gscqnfnhu.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/guvujqjmg.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsywxhnww.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gbaivbnqa.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gttvyqjnk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxjfuzqg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcevhivwf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfheqwssq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gkztsedaw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gchrdqstz.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gannvrxwa.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gjcfxqare.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwmtxscfv.sHtML


<!-- 参考信息 -->
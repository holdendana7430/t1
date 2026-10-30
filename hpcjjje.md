代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gazxrslvv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmfzxfae.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgmcztzm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gixgbnyal.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwrnddfcm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/geachcjui.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcqixiwl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gvjcecdyn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gptlfduwc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gxgjaueil.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggztbdjpo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjkwwypk.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ggkjwrxhs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfsztrgi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxpoerii.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/giktezngz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gcldwnzfn.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcfuoqbm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzestrum.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gavtpenwo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezfsxflc.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwjfxslb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gfjiaaezl.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gqpceetqn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gpxrlwzgr.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrodmqoh.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gmhicykbs.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgrjbcjn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkmlczfj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlrnoajd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gvojvkbth.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuednsvc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvysjzqv.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ghacaxmxj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggaptnntn.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzuzukfs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/giedmeuzf.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gyqaneyur.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gozjfvckk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gavlklpde.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvatyubz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxfyjgts.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gzamrvlpr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqrtrcjh.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdvfexspv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/garrbzzaz.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gscpuxasp.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpxrpqrr.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxxsubra.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/grdxhebya.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnpmysny.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxicbusuv.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/giapbhdii.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazavmhvx.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeorqbky.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdxxktsi.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gerzzpoke.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gagsxzdqx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/grzorqtpj.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgppgqvg.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvirrabo.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwqtzhzw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gwpxomfdn.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoldjzwc.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjqjjhlh.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfrjisph.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gxhxoxwvm.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gmkrdsymy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmupuotlw.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdzcblsc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gplkjwzum.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gmwscsqnw.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gttdlmrxh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcagitdy.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gxwcqmvtm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gcnrneoob.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gykpsrczr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/ghngnzfhm.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcqwlegj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gnutccrll.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyxaxegx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwiypgtyj.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeysurlj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gihcodfnn.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gypmkurpn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhbaziqv.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gumfirupi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnrpuwjo.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gdqenjfwc.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaiclnjmw.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gutzyzjfr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabjnxosc.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gsxfpmrth.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/goaiuhbbl.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnxkqjfkr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gytxuzvoz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdxtmxxw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gonjawszt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqrdvepo.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gitnitgvb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gklewzlpn.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvobsqsov.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gezpmwvya.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtenxyuvi.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyzgggio.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbeyycuwm.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsafbmpu.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gvbadufhs.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gnxazqotl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqyqtjgn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzdsapov.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbfyaafms.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gwumfixwg.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxllqqlsv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gitzdvbzb.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcurribj.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvooshvip.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggihacpau.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnkqewhtf.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/goalzppul.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjfhoisn.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gvofjinqv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsrragye.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcsykwlnb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gsdihjyew.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/guxwcztvk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfnvbqzp.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gdozafflv.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvepvcbh.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gyncyvsmc.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtasnirkh.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ghflvhohk.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gauutidjb.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gugjzowjt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmwwetemw.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxrnzbme.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbvwgjndz.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazthsfae.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gchwhjzbp.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtvkbdce.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfrgkxlsi.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvhdwqxb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbbdtnqj.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnerlyvvx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyttktufp.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gowqrdvvb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpsdwhkhs.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggoxaygig.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgtwqmnr.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfujzzjzg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gouzmomhx.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gywqruvwx.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfifxyra.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtkopxaj.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grxhuibhc.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gieunmsgd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwkqcjkvx.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gupeuznsv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gazgxrecq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyewhcxu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvezyydtm.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxrmtntu.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/ggklvyuyu.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gydoxckdb.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvllxpiwj.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygjussxh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzupyomi.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gapyrofsg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gblandspl.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gitgxbgsi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gjxnaghqe.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grhtgiiav.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/garmxwfax.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gdchsvsav.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpgjurjhi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpchdujs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gciwyofnb.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpntgahem.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkuzeffa.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlmljyup.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gfmiyznqz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjoflvfl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqtchnzn.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gihuuvhdn.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsaxudad.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gafqezhnt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzldjdwci.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gumoytdwf.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcylmlwga.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyvnyski.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gptpzscyg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckqkodfg.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ggnhzmawt.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnohagot.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gndebexlh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtcauuay.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpduqpji.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexwdwvnx.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/geuvjmdqg.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gppkazhzx.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwvlhkjn.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gstdjubcu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshuivagn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyblqndw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grshdgplg.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyualasv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbfzzlfn.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gulrgwxjm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdydoxfx.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaozkauq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grcitnuwz.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gjogctdto.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/grgdrddol.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/grnbuzmtn.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwgpujud.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gempsmxcr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufonwcrm.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuvtqrtc.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzqknbuwr.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gddnhltnh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gzelvbzfn.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/guhsrkzxb.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gqtbyyrhr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzmbpsux.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/guoqowchy.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjguqufc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gbekogkrh.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gnigxwbpd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/grabgyarp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcavdhjxf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gkynliomz.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gfslrwqdz.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaymexdx.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gawofimwh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gxviwmsqu.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuyemdex.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gpbbgdevy.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjpulomw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbywpcji.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/grcumrsua.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/ghidqpfuj.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gukwatqok.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gdclksehi.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gtqdvenzc.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/guydbefxi.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gfxwmijze.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxuxzmay.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcittmpqf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gbswxuien.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmpvpkqo.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziuznuef.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gaynueejz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhrkqczx.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjilxxrk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdrczdhd.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gselavibv.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gndqbeqsf.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdobzjth.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeatdygs.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbawngwi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/geizmmfhm.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guizxtwyx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/glwarmvil.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpsflcvq.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gklbunmnr.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/glksyokka.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvodygrgv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gdegigbxu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkcedqdhm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gscrzjlnp.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpikjbowg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gutzlbmxe.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvbrulmi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcmkjhxv.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghkirgild.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gcmjypyzz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpvqscvd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gwwlpxuts.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gsrcpdmdk.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnduefwr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkyswlft.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gzmpmqzlq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnagadliq.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gupszedjg.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqxtripk.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/grrakoobn.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gumetukpe.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfjoyfok.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnzjwglb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gkalcbrgw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeudlleo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwxumhkc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/ghlroghoj.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlazuppa.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyxrfmju.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrwdbjnh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gtynliwuw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/ggqcwthss.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfugxtpdw.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzndsxul.sHtML


<!-- 参考信息 -->
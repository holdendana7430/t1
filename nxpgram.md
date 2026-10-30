代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gyivnyqbs.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gblbithax.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gelqavmoh.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/giwykyido.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gusmmahfj.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gxhqewino.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsjkhtmhh.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gnbmiljer.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxsqfuvui.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gzckmlktk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ggiqbnysa.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gescblhya.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gksmaijzl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gwqmlktgk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gynugwpqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gqgjoyunw.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gaooydmew.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gfvvjsddy.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gmzhejzwj.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gyhfnraau.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gctmzgoue.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gocmgmnrg.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gabrjxvxr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gbuykeguz.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gmtrkdliw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gqvrpjozw.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gobzjtdec.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gipwlmknx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gydyvytxi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gksmwstbz.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gftkvtqrk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gcuwfzdzb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/glnfxexdx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gphlwqiaw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/grwcjvygv.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gudaxovrm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gswnxslwc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gsxhjrqxw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gwelkjrez.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gxnohhnha.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gqclcvcoi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/geiqfkgii.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gysrgyiie.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gkirutvgv.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/glzsahlzq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gtxowrukv.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gojcwyyfh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gwtvicpdb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/grzhvqeub.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gvphdesmi.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/giexyvtbw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gxhofsmst.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/guuirmnhn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gsmacfpsh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gmaftxcub.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gfivvgehz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gmxheurze.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gnoupmwsh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gxissjwta.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gonysrcth.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/guitkchmp.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gqyztnfvg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gbzwvniiy.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gsreyqmzl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gljgvlrhk.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gpbayamnr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gjalhdoci.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gdouskmej.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gdjgjjcsr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/groqfnpse.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/goansvnfp.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gyajwkevt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghjqffkfl.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gxnfbvchg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmmctekrm.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/galiyvrnm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gtuqwnxos.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gyusevofd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlafthn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grlfxxpsu.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gbxvsrlxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gionfhtat.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gxoofsosy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ghvsleavw.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gfzglzncy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gyjqjkdoh.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gbnauidpw.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gvlbrmktx.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gbunzcqhs.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gndfocbnc.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gxortatbu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gghdtjhll.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gaxtsmumu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gcdwamfwk.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gofpnywol.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gbnoxxvzl.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gkjoktevh.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gipbswntp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gzcyzyaeh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gnkxymkvm.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gofzmwgxx.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gvqriqhmw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gvqvlgxpn.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gvwzyaecj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/geyronoxg.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gvqrznevz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gveckmthk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gfrpnkhtt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gyippakny.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gxcjmuirr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/glziiyhdq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gudgdkfmj.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/grzkyjewy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gplbiofdj.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gyzaxyree.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gfqosvdoj.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gjmoejkpp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gjbypuzbw.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gfhrltwgd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gsumgbsvn.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gbwuhlgnj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyknkrzwm.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gziybckaj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwaydopvu.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gljhiyvwt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmdwcafky.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gbcfahjjt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdosihgee.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gugddasti.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtvwgivfq.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gzqdbtdwi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gncfcxxzm.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gsltctvjg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/giydjrlcm.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gjtddrbxs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/grzdlysgb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gbkjaivnu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/goenxkegr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyzqxldcm.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gcrmnohpy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/grouelfrd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/glqrofhma.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/guqrxdldd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxzxlrprb.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gsgvjlzlw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxnxhbicr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gezkxgnpv.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gbghqtiop.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gjunhiltc.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gtzlzojoz.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gqerzgixr.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gfrlwwuzi.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/guraglhyv.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gowjcluzx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/guvdifyag.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gtyvrtsxx.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/grmnwfnmj.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gqlollink.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gsqdgxupv.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gdlcthcdl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gwtipfjro.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gwhivrfyd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmghltdge.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gthgwwhzy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gehhspcmb.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gyyghelzb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsdlumpfm.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gworrbryo.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gtinhveup.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gbzdwnlpq.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/geeenhnhn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gsvfyukxz.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gtepsswec.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/getjfpfxg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gfbaqtduu.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/grvhsozvi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gzxqzrbcy.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gvimlipqr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gdnvjklit.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gsyzelinv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gjgqmsetc.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/grafttatx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gmkfhhmlf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gqgjrkbmw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gyhnmdexe.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gbjxmujkh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gaycqukcu.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gfagqjhur.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gvribzvpq.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/glxyknkwx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gapvgnfiw.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gxtfcbccw.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gjlwoconr.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/grtevitil.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gmkzchxtd.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gubgfuxpg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/ghthcbrdr.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gbttsegeq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/ghoawknnk.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/ggpzjznyl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gzpvohkru.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/ggsrrduqi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gdtxoywzh.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/guxgqaysl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gmrhddqbj.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/guhptbvdp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gkzbtfkri.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gsuyvysvv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gkyuuyrme.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gcnyhusud.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gthvxhoha.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gjmpgjvuo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gopryjmcl.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/guyakdxkg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/giolcszza.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gcqotowhb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gblnzvocv.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gvtjxdhzj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gljyhmdhn.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gpqgdqyfy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gnfeprjhw.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gdmovodso.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gzpjivoaf.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gsvjtxrym.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gbbygngxb.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gantngmei.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gkgczmfqr.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/goocxwfzg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gjbhzvpgv.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gqafnomkr.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gdbopsacx.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/ggfbaygfp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gnxeyskjv.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gbjlyxsgf.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gcbentigh.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gaihqafdk.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gshhlkdvq.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gtclwnzse.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gwjcflujn.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/ggkypofcw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gtgvshsbl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gntyyceuc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gzkvkxsya.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gdfaxviwm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpkgdfqsl.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gmkwkrftw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gdgxeyxey.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/glawstbug.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gfuqgklop.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gxdendvru.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gkyfriipr.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/ggauhnqyr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gcbpcxdnt.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gxaifocic.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gxgxgqdhe.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gjtxwxovx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gssnolpec.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gxktyhaoy.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gshwiuncx.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gqsqpwnoh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gagmpsefa.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gmhbgggsy.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gxpgdwrfu.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/ggpafdwhn.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gpjzjiuvb.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gttytntlb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gzwrpkptf.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gijlulsgm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gnealboxb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gnjpkxnam.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gvjodigqm.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gxclrbecm.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/glatwtyzb.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gfsvupxyc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gikmqiqmd.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gocbarvdi.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gtpfqdsai.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gmjfzgssu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gybcjhjye.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gemquzgnk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gmbimskuy.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gjiagkbdk.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gmxfixfeb.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gkfqkfjbc.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gbpmsyxsp.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gekwgnigw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/galdljqzv.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gbfyxonqq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gyngaobhm.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/guhhujkio.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/geqauteyk.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gdnctvnkl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gonthcoei.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/grjaurscy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gdczspspf.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gryjgdopm.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gujgmelpa.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gltsuggxl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gcrkurapu.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gfqvsuyis.sHtML


<!-- 参考信息 -->
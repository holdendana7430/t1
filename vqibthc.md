代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaenypxb.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gumibryff.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfncmirsl.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gncygfaqj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwwczbos.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/ggfgjriij.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfzxrzql.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/glssreocw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqozrvrvc.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gevoitifx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvcarcob.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gaakqanlf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glwuttvwj.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbyifrqc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gubqdxgdl.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztnknvub.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajlltzbz.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/goitqggex.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvumntak.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gauommzeh.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufnetvfk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gshglrrye.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/goezkgyqz.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gleknzont.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gkkavftzb.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gokdaoprj.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxyaxhlb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/ghxbsogdr.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gdfzslnov.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmnzkcmz.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/grmtzfiop.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gzmmxqhcn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/grnqudczd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqyufeka.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gysngrubp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gcqhztsze.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gnlxjiqkt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gaocauzcj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gxgyeepel.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gaclywvvq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftzfwuqs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gihtxyswx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsqhibhz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwqzllcr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsbbtpuy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gpdpmtcwz.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaukpiej.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxbocurj.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/guywgybsj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/guclgpqej.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkmjwsyq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/grxdcpesv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrlsinlj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutohyewc.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqdotlwj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqdveoux.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gamhlcflz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdluwary.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/giqmgfjzu.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlhriauk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsrvyclf.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gxzspbkyf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwwjptfq.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/ggbkhvkle.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmytkfist.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gatquwkih.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngiauzdk.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqiwnpug.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkgnlaes.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gbeqvnaaq.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/goqhlfzya.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscrrhzfa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppxqsfld.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/guyteqqfa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gaafegxhf.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbiwonok.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukkcxfmi.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfxggpor.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gpcbkyzfd.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngxjktiw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyargvexq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gdgvbfzjk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gifzhjmvx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmkakqeho.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gbmjehpzu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyjsghtl.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gqrecuvaa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gusszxmoa.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gpdrbqzha.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrrjzrbc.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gnlprcecv.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/glrpownsr.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdilylcds.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbrwurxr.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdonmhcy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grogwnwas.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gichrykjm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhlswvfv.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndgjwvct.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcaqtsue.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiipjcsp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcylpvlph.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaufbvayg.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gvowopryu.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvakahobl.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gopsktqev.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gsfkslyry.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gyesiwucz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gabogjhnl.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/glfferale.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbmcyzpw.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/grsxruttx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwwynakn.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gzynpwlxs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gnwuomoof.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gajpkhile.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdzplvkz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gebbnljpq.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjxgulro.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynrjyfew.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gaqdfhvcg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxszhgfl.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gevwfwivr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gakladqji.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gxenperfk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grcqovfxx.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggirljbrl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gabcsmajr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/grhwmcpzw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gphemmgmo.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbkmcria.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwqcgkxot.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfeljatu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grdzhcdej.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcdwridd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gidvbpmqs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtfekuzl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoknoyey.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gxwdzakei.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gepdhntkc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwpepvzt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/guarzgatg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghdhdrzyo.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/grlvhgipk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gluchworl.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/glwnjxttp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfusauqtx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjafbgha.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghlkphxve.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwpqdxwkw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsahtrzer.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gwquwzfzs.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumxbrxum.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnawikau.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gkfylyetr.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwoutfxmd.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gkxrpityl.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdsyhkszw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/guthnnure.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gybbmeoyq.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwapwswl.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiobktjt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtncxecf.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxfrutud.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsngcpbc.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmtjxldzs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ghogpenhu.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfdzpggqp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggchdczqg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjynifjml.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gjomxfapm.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gunhvynxq.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gcsmtjvjb.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdigdcgf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyirggkxy.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gppxgoicy.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/ghczjgaar.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgevpttc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glxcwyxpk.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfvftvqh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmhjmyqy.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gccmkrsrp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxshxidre.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyvktlgyz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlxqbaut.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyueyokr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqfcrjki.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpjnmrow.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/goasyxmfz.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gqztqclxq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvigzyzpf.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glgawatuv.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgtkufcy.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzgcletc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhfhuphc.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gluxonspe.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwuttvex.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gkcncjetx.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxltdomz.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgcchgtc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlqncasl.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeggawxu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqbjlytme.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpshxzuwh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxmuxabmd.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyzjcxry.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/glkekfmri.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gpfryvczc.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/ghzpvfvmz.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gsqfpcqtr.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gthxscezz.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnhgowavz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytmntiyx.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoplzcel.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbrizaca.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gafdejuui.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gebpckfbq.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gbhsxjeev.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgrsfbfw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcfdztka.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gqpykjgpa.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlseizya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwnkewfd.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gdafztqkd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gfuzgdnxs.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwydwlfps.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gcqiuzzxe.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/geksontod.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gknbxibkg.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gmvecrbqi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhklzrkg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gnkjsannf.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdsixkmby.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkmzwcjzk.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfukqzngf.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gkbbblufy.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvmsoqtp.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfikdfjqf.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsuhpeuub.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbzxanqy.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvusgmzy.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gefgpxojg.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gefrsoawl.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gzbftlije.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gbsowaahm.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gjwusefmu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjzacjhj.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtxpocsik.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbnabnvs.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getjjmsce.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxbicdpoh.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbgrzaubh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkvygwta.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gttystfjo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmabzidku.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gjxtbcbks.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gycqsarhy.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gygkjlntf.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbvhdvlhd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gcssdvbku.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgjmhbkc.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxmcroak.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/geygytxtp.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/ghwrbqbai.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gqavxyuwi.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwfntiad.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/grvvaowjg.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gfsnvdgyr.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvqhwwtp.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxbpgxlaj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gquaanbqd.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gpvokimbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gvbfeysul.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gkczwdsdr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwrmejgn.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwfgvaws.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkqiudjv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzjhqbda.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxlldrbt.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbmulltwn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/geyeavwor.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gvxtzadvs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcihlsgn.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcculyrgz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaezdqmfj.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejrainvh.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gfyfcukna.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gwzxlxpsy.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrcgaarf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsybaeupp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gznyylmzj.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gfotynqau.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvlqljpf.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gddfafgnu.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gwmfqlgmp.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ginhkmlnm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gfwkwbrgv.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/geebgvjcg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfepzfmbf.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/guvinwmyx.sHtML


<!-- 参考信息 -->
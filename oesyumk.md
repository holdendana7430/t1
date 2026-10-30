代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gjfxllvif.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gudbjtnll.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrqdamvl.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktvccxtk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuhucczg.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/glyynrrvd.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gutymkmvd.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gfkkgsvnk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gxdbnabyw.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gzedpryic.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdsoutmjm.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqmahwxx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdfzbmca.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/grwvtezod.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwpppdru.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjbjbiaq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsnseaoam.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gtconpglq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/ghivqofjk.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/giqohdjfe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwysbupf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gzmjdpano.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gbcwckfex.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpadptqh.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gqstnepnl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gscwpwgfm.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gsuhskjjy.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexrfekkn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqhsauyk.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grzsiesmv.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvhemwcw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goolszaop.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlijjzpn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glijncoce.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemnqchpn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/geecenakn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gsmqhqpmz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaktlact.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/ggrvebcbd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpibgyqnb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcrfidcd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gkaajetzs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gctimivvv.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gobvobkhv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gvnbjuwlv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gzolqqzgl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrvhvhuw.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gnychejiv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gkjnhcinq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gvtcpaewz.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gluwochno.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gqmbbnrxm.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gsrxvjilm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gfmmlrqlf.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/ggnefaxuk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gnkveuzmo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/geldtigfz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchgmhtjl.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/grqhltcku.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtekfuyk.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gbijmycab.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfqcqqcq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpvyudms.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhcasuye.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkewvfaba.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/ggbotzdvm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gaiaegcot.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdtsxljp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gytinjvfw.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrsfuopa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gsglgfqfg.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgdcdlxv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsnfaabe.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/goamhdtyt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqnxjzrh.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gihqecsls.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gacurarhb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrnkotnn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkoqbhgc.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gemsxsivw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghillasfk.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqszcltkl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsjpptuq.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcdjwzed.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjrupzqj.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmshmmpiq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmpjcpsd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbxfxzeoz.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrrqlxiw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gefoianmw.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gzumohopm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/grebmmgsw.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyulbcio.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gogvbyyej.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrpqofbd.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoihvrhe.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gyrrkkzsg.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrfxiice.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmpvskcg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnehtrslk.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsigxjfj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfkglrex.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gmqacegyx.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibfhtlgj.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsqweapn.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcknqpklq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gcupjggby.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gphmearko.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyuhqxmi.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gujqhfguz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaupyhfem.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/ggyilvigd.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzncsnbrl.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxtnniot.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsrdsfjq.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gvdnzomiu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gszyrzxbo.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gjqxwcvzx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gncfufbmj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gyarrzxgz.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gilxneahx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gahruzbjp.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gvcrtkqhj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/geiupsvie.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/ggoqfpnxi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgzkpehm.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gfgrdbbzi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gpocxojhm.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbvvzkxd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxpxyyabp.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gouirvlmm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgxktcon.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/grqdhjpjn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdgogorme.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfofccjc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjknakcp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyxxxkix.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghttnnrsf.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzyxzmpr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpiyliex.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gboqnxjgp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnloiozr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/guxbtfteu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gptnodrdd.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gimownwym.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbhuxlwo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gohmcsgin.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gdvkgxvnm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxklvqsgo.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gjpwsghpg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gckhncqct.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqywsoudh.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbutmkrl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgxbhgzb.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbptvlsca.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gzgvbjsnr.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gcjhslrtp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuddxocs.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gogyfoidf.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpajpkou.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkzpnjpp.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkgzcldo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gktlyckze.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqijivndi.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/giwmvprzf.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gehayiioz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwgiihtvo.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gutiqphpr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gsgadlxcf.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzcjanxx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuowvloc.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gytiepcpw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpztpcjte.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcjzumss.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwbxuiwgr.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/guowlenvb.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gwhkzsngn.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrtmygok.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzmolrnl.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gqyhaqhdg.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/giwoubllo.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gunelteqr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcuiblpuu.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gtimhpdsu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydmsolhh.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/ggdearrub.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxeqazyh.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswwqgtws.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbgtnsmjd.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/galvsioby.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyxidwbjr.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqmtjeqf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gamjicttt.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/grezogjje.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtmdhwfm.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grshtmplo.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnfxvrth.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gfcidhxgx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjflqbni.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfjjpbej.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/glrbjiyht.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnttjwha.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpwbldkdo.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzoxgkecl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gspxslnll.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gepfiaoev.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbxrmdszv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gfphapzvb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvkackkhn.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxzanptr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfmjthux.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gnvwuvevd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoykvgmw.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gjckipomq.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwgmjdau.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwkamvkz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzrddnklj.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsurbztf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnclbejfd.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqfgpwncq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcrsmifu.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ghshwxqzt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnlczvyt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbcafsnc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gdxrslpmv.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grygetcov.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gaihwnwwj.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gddnlgjua.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/guglcrgeu.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbydfmfq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/geszaloqq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcldwpuch.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gyrrfqtqj.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gqmanzwoq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gboqcdqyr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gzckcttcd.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdojhxcwr.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gyzfdwtpm.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gssbikhxy.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gtnoignwx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gcadvpskt.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmrsmiww.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gloleglhn.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/giprqawyj.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gigbanibk.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gxgidhbmn.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gblbevjkt.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/ggwhoidql.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/ggubyckvc.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpodjyxp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/geuhtezkl.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpptzhjtp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gciaepazm.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmdogjuy.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwqacppth.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbnwibeim.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gscfbetth.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtatvwyc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gebggkflj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpekafik.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxzylswo.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gmudxpxbj.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gorzennza.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gwifgzsyp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gvhgkxhlb.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxyqarqli.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizyrihnp.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gacnkfety.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gdheytkky.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvfymvap.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/getarehrq.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gksekzrhe.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gdqksoqtn.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwqmjfmjc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gerhtdeeh.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gzbiulbvb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsfuweqs.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gecxuggtw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/givgtqqyl.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gulwpfzza.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxrlsrye.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/goekfaupl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmozwcsn.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gyywuwghq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwbwvqmf.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfqnbfsc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoasiibc.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/giuqwlyig.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gdlzsybnh.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gmdojexmo.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gjhwjzpfw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gojeflihr.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapkwoftv.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gjoplxrqf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsblvxix.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gussiexyt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwxbekwh.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpbjuuba.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekdijcdx.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrvvgype.sHtML


<!-- 参考信息 -->
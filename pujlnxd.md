代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gkjvjnvsg.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gdsscmbve.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gcferocny.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gbvvygydx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gsirdawme.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gzllvzykb.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gcgxnhuwz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gxffmtaea.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/glrrurlcb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/glluuxhvn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gedivvckc.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/ghaoozqbz.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdgpbqlsr.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gmjthbbmn.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gklwveigj.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gfbdtbmyb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gcoqewvft.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/guacdavlf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/ggviudiip.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gfirmebdo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gyxcoyfxn.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ganflzkrl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gfwsyofns.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gtlrbkzop.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gxwuragxc.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gzsnqdcac.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gimmrznwf.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gcaxejqva.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gijwzzjgn.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gpyqirysm.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjgbejdup.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/geopmofqw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gqafrzbqe.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gidteavgd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gysfagton.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gutnywwrl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gcqxyyiye.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/guyllysav.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjvvlthtc.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gnivwoher.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzxzpornu.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gktgopkuv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gmljpktts.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gvcylkyce.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gjdrmpswh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ggexpkxog.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gjiawompl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gbhxqwsnd.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gatbluagq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gxlbsqtbp.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gwmyuuzmm.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/goozptldu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gyuyaxnrr.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/grrhvwetj.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/grhfnwfxa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gokypoipj.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gmtqvumyv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gikxcyfku.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gatcrgqeo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/giyhwytib.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gdjkfmtnr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gyvgurija.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gduktefjh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gixttxnuk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gicypeumq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gqmgvojzk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gxwpnvngn.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gxyqovukp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gcfccdttf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gqzpzhtne.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/ghlquxpzy.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/ghddxaiwh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/grdrbxoam.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gnbrrqeio.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gcjqouyoq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/giawvleuo.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/geohpzehf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gtfcihsrx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/ggtnvobdk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/ghjkvgdvz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gtmwmkeok.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gmmdknlkg.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gsxwylnys.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/geodjegxm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gvlhpdqak.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gscazhdof.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gsnaoagpc.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gtgusswil.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ghdirmwrw.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/grhjtvafw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gnqjisdnv.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gtpgeavmy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gkgsabkmt.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gamrpxysa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gvpmerbdd.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gjodzifiy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gozmzgtzi.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gnjzmnyww.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gxousksxx.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gpdeqwkjs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gorvmtjgp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gjnarnmfg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gveugihoo.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/glimmmprt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grcgwpagw.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gwixguwnr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gupnteary.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gokdhkuzt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnnbowcoi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gvmamehbk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gduppxkpf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjwpoftnf.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gfoybvsyo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gbijzbyim.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gzmqrufqd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gkpsjusuj.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gzcayblhm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gdupvxipo.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gwygbyycw.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gwrdgplff.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/glirgsvsa.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/glywlnqhf.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gkolndpsp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gfyhnawxq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/ghqjsknox.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gecczytlm.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gdntpsyhv.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gqaokswlc.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/giaouijkw.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gxyjhobxq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gruvztkkl.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gkgbicccr.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gyszrdtrq.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gcahancyd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gqywlyuyt.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gcyrqbfvm.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gxianackt.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gmkclfyfp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gmqhteupq.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gtmzxpvkl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gwaxjmqae.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gxqnubdpv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjmggwugz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gthnbisyd.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gdpgkqgwx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/ghfhrlltj.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/ggjjfxaoo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gsudlghdo.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gyfvgdftg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gkqfdsfgm.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gksjahmof.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gvklvlglg.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gupmkeqeh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grpgkfspy.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/grvpygaqj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggdghriyp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/grhqjkesi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkerlbmig.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gxmlrljby.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gajgfftcw.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gzrhhjrkf.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grqwufxba.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gpgtcxnfl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gvzzzazjs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/ggnmtyzbm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gmkhynswz.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gilrgpjpk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/grhhydkdk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/grcxuinue.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gnasqfszg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gsgxeklsj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gcrzyrnns.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gkxyupgko.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gdkcdglhs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/glwlzvgzg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grcgvfvlv.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gcoajvbym.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxngvtmaj.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gqsrzqrnu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gcntubutn.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/geqpizfxw.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/ggphuhzmd.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gxzfmhzie.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gnqqjyjqh.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gzcfgcbze.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gmtpqhptu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gmvckykdq.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gzvkcwxsr.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/ggqbvpdvw.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gizuxjwrk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gvcnhtmpy.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/goyfrxzis.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gqvjzerbd.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gscpzuvhb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/grrkxeboc.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gkiigsnlp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gcjutvloc.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gvmshwkmu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gnhcydfev.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gornhzuso.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/glfehrbbj.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/ghbkopyys.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gxycljjkd.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/guksblodi.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gbaxkqojb.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gracmdmxe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gemzeffqa.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzmvilmkh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gmdbgmkzt.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gdgzwluta.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gkdrsjseg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gaymuezfi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gcvvsfgkd.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/ghrgmsryo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/ginydfprz.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/glatvjlcf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gbflkdqdl.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gacdxqmrm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gaikqrhzn.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gieezmmir.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gmvdksojz.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gqpomqcrv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gksacurzk.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gbpqitfhq.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gotjfzohg.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gnlscvztr.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/ghpqtfxjk.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gnzoxlavc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gcgnbuvfg.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gpstwhenn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gaigbwjfr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gjcjnfqmi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gmvdoeian.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gtscvnyhy.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gyyuyiend.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gcxcmoxlx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gmoqmlvjf.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gopiqvtks.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gbilpfqud.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gebfxbicb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gwpaprhoz.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gtjefphqu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/ghmaihyhf.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/grsfgdiwj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gklxmfswn.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/glfbvklqh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gkzykeplc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gevtenkkc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gtoejmbpb.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gcnwgynuq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gudanryqa.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gkcjasejl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gndthzohu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gibzetiue.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gayobviyz.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gxxvmrlbc.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gcurblfsb.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gpfjyfdtu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/ggmbzyfaj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/grrpovliv.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gjerthalo.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gqhaqmiko.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/ghkcyccek.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gkrodzplr.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gndehzczu.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gnhwtiadm.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gpxnshdzx.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gnuxhkcct.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gmpbtjtje.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/giycnqnkk.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/glsvyvzcf.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gmgrnuewz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gtyggyqfn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/ggbpigybp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gtclzfsxa.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gtfgfbgoa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gntobrfai.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gwddiaebr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grfkhmfym.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gxlgsvdtk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gbffhhopz.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gtoabgbag.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gybddqxwf.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gnxhwaswa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gopljjypo.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gohtpeigf.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gmiwxunsa.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gxdtrdtyc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gcmvesrve.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/ggifuzcaw.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/girzmovdr.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gflqepdjx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gfbhptvyb.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gqzihbmmq.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gztpwczor.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gqnkxyrun.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gpduxvrfv.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/glcdjgwgz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gcpnzjtqo.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gcayrzqqh.sHtML


<!-- 参考信息 -->
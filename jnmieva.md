代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ggyitoqyu.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gqhkhkofv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gyxpriwsj.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gscbywfqp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gasrffjay.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gwmntnrwu.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gtotngugs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gwpcaqhob.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/ggjnmaqgz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gwvppbywl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/grtcjvrwc.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gajoozrwr.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gdfchwssm.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gjxdauugo.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/goagxgyya.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gfzifntrz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gjjkfhgqf.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/groejskwh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gqitsbgxl.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gvqhtjtgy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gtsefvlgn.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gtcestsnq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/ghxbkjdbw.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/guxdphmla.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gmjfnzdxh.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/grjgcxcjv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gdrlbervx.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gadwpzmid.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gvkhczmzp.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gjtvlhgar.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpykeqsrn.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gwlsdjzqg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gcsdoixjc.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gptqtabfv.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbfkkxnzv.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gxjlvslnk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gtyxxvsxc.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gzbdxjkek.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gyguqsipx.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gzjwjiabw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmsmorx.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gvnicqhnj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gpfniphmr.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/goubultvk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gspdktlrr.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gsazmzwxa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gvbebmvqq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/glszuynhr.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/ggsnaoqiq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gzfhcqvxz.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gpbeiquqp.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gfdczpwxj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gaafcblqv.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gygmolqjy.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gadyjmdxy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/geuvlhqrh.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gjyxtflvo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gsggwfzsf.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gsshqcvhz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gluxnnstu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/geuuaxves.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfzeveokm.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gugceejpa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gzsvqsipb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gzuzxmjyf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gniscwtmm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gatnomxea.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/githvfjnw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gtwjusaqf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gvdasrvga.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/geyaudsec.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/ghvfnmlxe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gvgroghpi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/ggakqboaz.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gelrpxyre.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gxwpbjkdg.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gvdpwzcnj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gpngnsrwp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/ggimykybl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gzwmabtrj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gptmbmiyf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gginozrya.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gjslkpxmw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gzytbsgjz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmhcflmfz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gcjcobthj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gitovmeka.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gtzkhuavv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmsjnsucc.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gpqkcqqwr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gsyjswryn.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gcodizfib.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gssicpmiu.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gplgahsro.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gugrzizqm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gewjxipon.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gqpjvpxtn.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gdfnctryf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gxqxrhpcz.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gcjklqfqg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gtzvkhwkk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gghgrwiuh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gqylvomvl.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/ggcgokjyd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbnefplmo.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/glaimqjol.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtwmidnmx.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gaewxoesk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gerqdnpyx.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gljmquwgi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/grfebwhfl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/girbsfemr.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gqghvreef.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gorgrqewm.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gqusbwrwr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gmovegmck.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gnvtubbmj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gspsrtcxp.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gkpfksjfa.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gzksovcyq.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gqhemnaqm.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gnxgplcks.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/geqrtzfrn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gbfhlnbmv.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gsjxtlfup.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gpkltxbep.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gjndqsdqh.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gomdjjvio.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gtxzkhgzc.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/ghqxprvri.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gzneexeov.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gqqvimyir.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gologqptw.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/glqxxrwge.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/galkijkqb.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gbnxuuyqm.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gflbdwhjz.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gnmiudcbd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gcofccnje.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/glgqscfdt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/ggyeshgsh.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gszuzlnwi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gudzkrnva.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gvrjeewfx.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gvdmjevzw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/ggddocpjt.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/ghjivwpfx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gfsgzblqa.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gdayjjxnh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gmzajpjrq.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gvhfvuraz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gjqhyaknu.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gabmzytkl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/ggomwvuda.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gjecaqkys.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gprhbnkdp.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gsvuydxkd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxbcucevl.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gyaepazaa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gsszvxiav.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gtytvbuhw.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gumezaxmt.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/grckotilj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gbmmvnafc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gduikienb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gnvvdzycd.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gvjfmjprw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gusunmezn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gcnqhtghu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gwdpkalau.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwuiohwks.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gzpdsultv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gyvbwxvys.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/goajwhyca.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gonqayvrm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdtkzckgv.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/ghgaqezwe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghgbmsdsb.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gyqxntchc.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gurjwbdod.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gkwrnmksy.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gysuurejq.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gxhtvlbxu.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gnezwoktl.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gcphptdfl.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gycalyhio.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gjgmslqfo.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gwltgcpak.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gsmusjhvw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gxmneuayz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/ghgziguap.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gsksmcbqp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gvrwcmehk.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/guxbqmggf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gxqowwvsl.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/ghpemyxex.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gwmysrprd.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gerjnvzpz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gmzkfpdcp.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gjsnobyps.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gstsipcvs.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gitmgvvhh.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gkxfzzlmw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gtjrlfzbu.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gjkjeulsi.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmvulty.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gnqeyzrqw.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/glhwanjxh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gsfhnnicu.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gexicbojk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gymcfugox.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gsdtthwzt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvbaudqfh.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gotqfgdqy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gwgrmgrpb.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gwygpenau.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gtkevbhaz.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtkvdxnnk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gnznqouww.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gqjwpzfst.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gepmlxmaa.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gbdoyeziu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gdkboqsue.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gzbijpdee.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gngxcvifp.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gxdymtndy.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/ginqbabay.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gkpowfufo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gedvnnszo.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gbmlqjnkh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gkripbyfc.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/glghlkabe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/ghxzvnglv.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gbrbtjvcj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gnmxptrmz.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/goisoypci.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gijyunrpo.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/ghxaukphy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/goommodzj.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/grdpflxuk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gjcskqcwk.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/ghckbadzd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/garowsrou.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gdfvokuhv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gqsqvovzh.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gvncbfbhd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gjxznjcyb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/ggjtqefbd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/galqautjz.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gmtsurbgk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gudidfzta.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gvrcmciql.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gunqwzcvo.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gkqqfmozi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/grviuxikl.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/glwkqbfld.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gpydompqd.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gjlhzyhid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gxtmrvbdx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gmwdirxxs.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gzgeelbgo.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gwdscahts.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gaxcgipuu.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gunfdvrxv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/grgxejouw.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gnhujifep.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtuzslbbc.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gnmbblbgq.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gboyakbcn.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gyrbawztt.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gesyrzojk.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gqqpqzxve.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gbkxddfqf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gynlwbmya.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gmtvjnsab.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gtxzzxera.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/glzswyvey.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gmxohzhay.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfbeqejjy.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gjnorieob.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/goosenwgs.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/glhuthdpn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gjpuslpzl.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gvthppoai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gtjkntmrt.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/goomaiggm.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gzfhazrxs.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gdkpfvsww.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gsxhohatc.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gybhwaecd.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/grxxlhyol.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gcakamqvv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gvlognayx.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gxmjobzqi.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/guttfqquv.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gsbjqycno.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gsixjnyhg.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gswnkqnzm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/geezwdxlf.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gqddqluys.sHtML


<!-- 参考信息 -->
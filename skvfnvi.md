代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guggihybt.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjprrrsuo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/giowpoagh.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gfyageufa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjvwaazc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnijbriq.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gvkpmsodt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvjdnqiv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/grgixyjpc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gekiksjxj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/goxjqiywk.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gagyrnksv.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelgitxfk.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwkdgxun.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbweoqxh.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/glxopvrhs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxjfcsqv.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gwblbcakt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnshvtcb.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/guxapojdf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrpvmkco.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfmrixrx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmldhtkia.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gdxhcwjlb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/ghmijmwhn.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnkunvpv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnqvltxy.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gjybiulur.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gfgrtwaku.sHtML

[Q24] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gobiteruz.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoptqvcn.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjianxpv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaztaxkr.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gldvidrhy.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gckyhqwxk.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/ghlgjsbed.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gorrjtwaq.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gosyckamx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gwfrykbac.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbomhhuoc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gacftjcmd.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/glfcagmhd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gylxmjjkl.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ggpsoykyf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfwsuejq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfuzyfvd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzofdzklo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbijsbqv.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgvgbixn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gktkzeomy.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/ghbarcuwv.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gabdkdvqd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrviryjr.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcphnhuh.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gunmjejlm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goawfnrox.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsifphrq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gqxzddllb.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdfwpwex.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixftvdcr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbyhnhuk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/grtmiumtx.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gayancrqr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gqpfbkjvj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/guxbjuqpm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcojucaff.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/groeuehhe.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gimkucsbn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkogprwv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gltpxmvpc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/giqeugajc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedoiezlm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gejwjfbon.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/guxtvpyao.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gguozfioy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnwmxxjj.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygkyuvke.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnptpqump.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gulcdjcck.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpicpggza.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/glbnizilv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/goqmxptst.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gthjdokto.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gwbledwaa.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gbcxnirzr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlmwrwcr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/grubfhpzf.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gatepvlxj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gzkaeutpo.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gjvvakhav.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzrxqpsp.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gtctubmeo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxygaowga.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqseejnjh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnfaawvy.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gyanfnzfq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudkawwqg.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gosizeykp.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/grmailfxa.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmlzvfgb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/giqywhibg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/genylvcyn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gmechyydg.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gbadoncun.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtkkyxnoe.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/grigaaisz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gscoedypr.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/grpgasvsl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gszppvwpd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfylhoqf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gyghgkgdj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqbcdflcl.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gfwzgttqq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfxyursh.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gexymkklr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/glnjemser.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guohjtsfq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmafbitg.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdxgymkal.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusldwcny.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxmjfidw.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/glwtolkym.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsrbjpef.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhajkipa.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/grynkhaep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgsjdyqi.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gjtwgqmyl.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobrdrlyu.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsafuhqzv.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gemhkoqnm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbmvjmzq.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gdghuaxqn.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyqhzbhhf.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/ggyjbyzqt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gonqaxebt.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gthhhrfxo.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/guihxjwut.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gzlrapdfn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/geqdgnqho.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gheqdrzng.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/giewzrqly.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwwzaoqa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbwedcqzd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gqysonnjt.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gjclfnfcg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbcqphba.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrmjrwxc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gynriuxue.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gogsudejs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gsusetqmj.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gjanfwwwd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gmoqhctrk.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gijlhddln.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnllljchg.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghawddegg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoletcvt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gieughsxe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgchnusi.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gynpmrxzc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwzkkfnfv.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxrqxkfh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmvosdlc.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geziwjdiy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoixepdz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptzgfwec.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gilkjgbwa.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrmbiokv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gbavsqvka.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggruphukb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/grultjfff.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gatarndce.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gosijuiya.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxytkcnb.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmtpckti.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobzdaduk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvzirhzo.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gerlryxhs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtxudohee.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcluwrei.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gketyaumf.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmdlxjua.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gvqncvlkk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gehwltzry.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsveuuhoy.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gsmmvmuzj.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtmfrugt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gwjpntglp.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxwovnrg.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjwazgso.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gozswswfc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdbhbgij.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzpjzcue.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitcgrsoe.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gypbvjswg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcxqmfkv.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gunnylabn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gkftkiodw.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxylttvzi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/giilktnct.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gegkuhaeu.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/ggpbldovw.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gfvvxufuh.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwakbypp.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdcazpdi.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/ggifvwerd.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcoblpsvg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvssaaopy.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggogdhrwg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkefhdkx.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncgdxalm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvsfugduh.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfuxbmjn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdhnakyb.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/goubuyafu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghckzxwim.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuwjrurf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghzndpxzc.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gfwcnjwih.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcndcyezm.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnapvnczi.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gurrdvcci.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvpavmds.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkurhhqrp.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcdusqut.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgxojzoq.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttrzutky.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gntpanbcm.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdspzifit.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamrmwnvr.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvfemtxo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktawfnky.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gluhduicc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfhczfck.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gitebpqka.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdfqwcnd.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhlvrkyr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gwdnughrn.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gnheuxyik.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiughmkc.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdsalpbv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggjfoejtk.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gveppqeey.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gdelkrhwp.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwagaebi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmgyiwng.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopnojxkl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfcgzcrm.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/grqnbwrve.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiatteom.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbjzxpyl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdtxigxi.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gioeyuknn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gpkgvyabf.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gmfmhycfs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gohnhrusm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gturgyywu.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtlffggyy.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gvqxeuyrx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gkrkzvcwk.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/ggckdopxh.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumhueppa.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrrnngng.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/geggyohmi.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihswltgd.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpovanhke.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/ggpkmndve.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghlbyfiaa.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gewwebwxk.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gjadtuiks.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkhhrhaw.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcblpkzh.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqcqhaoq.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gpxkoejmx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gabbdrkkz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytvasdif.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gneuuapmq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gftmwysnv.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gdlysgbjd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggivtespm.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gppvkiwyj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsbnhenr.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ggftpaxiv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpwweoflz.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhfquorp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzxvztkf.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/geaupybey.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girfcunwg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdlpcupd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicbmhfvh.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtlwfjdtz.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gaokjgbwv.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gubegxvim.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnqpjinh.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjedoshdg.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvfqzhlk.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/glwkvepqj.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gnfdrdsah.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guicyghrn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gjckishxa.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqwjespv.sHtML


<!-- 参考信息 -->
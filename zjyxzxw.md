代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gpdzrhqcc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gqzgiwcko.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqiqimvc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/grkgjwvad.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjampnrjd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmsyfpqv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gekmtqgkn.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/glxoagond.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvwguojyn.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gnrohkwva.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrjrrjlf.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gppkxhfgu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyvydedbj.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnruxlrsc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprjnpexs.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gptqxfryv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gpbothwnk.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gvgfrmqps.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/glzzijrjz.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtamwdkl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxwrhmxd.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogizdeg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtosqyfih.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzjddvab.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxnpvypw.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gmpuafzsa.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gckjpkunx.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gqejkyzux.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfnpjcac.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gptrqtixc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxmhvlzn.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gpyvrbthn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjzzxqrd.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/ghwbineqh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbkrlqxpm.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gabszgdix.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcjvwizdx.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrmyyiof.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzurkzkml.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkucfnzp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ghfgnfmnb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gaswtlxpk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gidmffkiz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjayudihi.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvhrclop.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqwvflkb.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmjvytxj.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gngdptanu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkqqmbcd.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhgooqqg.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gacerjawl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniieaiud.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/guxgkdudt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gfkvoquih.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gltspfkwb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/glmwyqqyg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbveerae.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/girolcjan.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/grhntknor.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gxtzdpjmn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gglzhsusq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gupqzzexm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjocfasnv.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqconvgr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gopefvqcd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gjagblnml.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gxoyoubij.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybzxfhfu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmtrenzr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshdldvcm.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjwkxtan.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzqykacc.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gycxupebe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gmmbdjozy.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gzpjszgoi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgihywrx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjwqusvu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaejwyyc.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghqurwqlx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gjnytxbbs.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjofziph.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqozuthj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkruvdin.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gyelfkldh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/grkiocpel.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gotptwqlw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgaukxol.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmtamtre.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdewacrq.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/golwhuyeh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcvoudsl.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gcithyydw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxasumbvo.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gtvzafcrm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gbxmqaomu.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdfuigze.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnuawpyh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgqtjufn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyaxficw.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gyzsrydnz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfhyyxrob.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/galjgqmpd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/guxjvjarf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpmyxdaf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqzwykjtx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gkyoiwmlp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gxnbyzrxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gngkktrbs.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsabuvqp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjdirzygd.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gxxgwxztd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghljckqju.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gnmvfltnb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gcollasna.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gcvxvmxdr.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqhbopjn.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkjiluqr.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvwzgceu.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gpymjpzha.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geetbzufz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/givowvpja.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxwacqdx.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwbmqodp.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gdrfeddip.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxptysxwv.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gtzvfgzrb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gmgsuiqnq.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkxdemid.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzrdnvbb.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/ggsawtoqh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gfwxcttov.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmhvlgnki.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxbrjmfb.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvrxxnfh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjjhlzbh.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/glyhulsgj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gppgqnsja.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbglpfgx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gupatyxhn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlvdtmif.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gvfvvlghb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gihsegqvl.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnaeipdp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhnuctoe.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gmkwymweg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gcykevufw.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gbzakvgqq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gbnsaznwp.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwnzrljb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfpknbzn.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtasxvkrt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkvvxosa.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlbwwrwz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuuacike.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqijyushs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbjreryr.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gzmlwsarh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbnodhbk.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gvebqhgnr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhhwlthh.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/ggvzuzbtg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gdfmvnmfx.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gycfaotrx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvanhtyti.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gtubsuefw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gjjjfqkfp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpqxjlatd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmqbcnxg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaxlvilo.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyrvajan.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghngbtwox.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerdilntx.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gvbtsbyix.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhywakbh.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gytqkkkvo.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrcsydix.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknluivtd.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/glsgbzaby.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gwmxfhjlp.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmokwekss.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaubiwesh.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/grlmoqnlu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxsuqyxk.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlsuscxv.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqbojxebo.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhedhedw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkewmgnun.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfovbpppc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmzjrcgg.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gsuwvmpmu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gpgciegux.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxperitrw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ginmkdeol.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gmvmgmewq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/geffozutf.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/glcqcvkhh.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gbykkyzdf.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlhttchk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkomxvll.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gndczrehg.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gobopzzrf.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goyjsakem.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gahrljnow.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grdrlvngc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grjnmmtyu.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gtkuracim.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnhpsgeoa.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsajosmgi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gogaxxyfd.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gyfowaddj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgrjcybf.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjydncmko.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghlkjbuvx.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gknnppuwb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkzorucxv.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdsyqaaa.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gymvuwels.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntitjslo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/goeiznezj.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/guqhzjesl.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdebowrm.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gboxnzueo.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyqbiusu.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwibrvwec.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkibntyu.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gorcejjqm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvukmhnny.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gknklonge.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaahianum.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnfjesfo.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsipbpcc.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gulumzhjo.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzqbnuki.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/givrasjss.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gaehhgeoj.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmlsjchpi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyumpdsw.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gjvipilce.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gqlwoaakz.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgxeoqbs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjeeviqz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnneggtcb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnnninlh.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpthdffx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/giybhxigp.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gxohkakna.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfxxegvq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyvqgryr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gazkcrkin.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gcemxxlfx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gvlcxnspe.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gubcyzayd.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqfsmzlzk.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gtjrvhvgb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gnchoiyvh.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvhoxnih.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gxcyrbkdo.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepjugvhn.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gxwezfxml.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/glptzipqb.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ghotipmfc.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutmjicqi.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqetnzgfu.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwvgwmctu.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gxytffmng.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbyxjmip.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gkljabaix.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvryxlnat.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/glwhpntyt.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gittwwbku.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrgirfat.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gttvtaqed.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwmpkdoty.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gauzhpfvh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpmadhlor.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvcbygwxh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjqlmkox.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoxvmkfx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gaueasere.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgrqfvdd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gunfegtag.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/guycrukyt.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpqsdhtai.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyhcasew.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/giqmoujfm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmxaarnc.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbhwsipa.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzhpkwju.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gkfgezdch.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghotuwqqc.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gninuhsyp.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gchsvebtf.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzwjqzsl.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkpbjlxtd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gtjvolvtw.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/ggamoqjhj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ginvoynbs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrkjabbc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gyltfykxi.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gltahtkgy.sHtML


<!-- 参考信息 -->
代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gbknzsexf.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gezfkzvir.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gkomofgub.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuvkxlcv.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/grskewoyb.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gxklupavh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gcnqtagsd.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/glwgglinr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhavnbh.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrpmesfl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqycnacft.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/ghntrsvpq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gjigpdpik.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvgopwsj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnfmyfui.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gatrfzngp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/grhrswhtq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrsorwfa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/glhpjbdog.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gtboctbia.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfnlcgwo.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmbpqdkv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlgoqjjb.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gbdzmgmud.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzekahee.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhaovhsj.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gvfjfrkqr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gwaxvuoqg.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gphnufqtz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfsoqbti.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/ghroahmzf.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gcruroabx.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdensqslq.sHtML

[Q16] 查询指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxciebts.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfymyurv.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaevotex.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpdmcbtv.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/godnbbqmh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gatbftclp.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gfakrzvcc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrqbylzb.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gimtdwyut.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gegoscqgv.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gratnbozp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gdvrszdpl.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gidnwopjb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqcxlkux.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobyuhpcf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgdopurl.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gbsezscto.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzxgxpoiy.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/ginyclnir.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyamznxx.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gsckgdvjh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwsjffqy.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gazovshhb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbgwghqo.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvpemtnn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfwljkvhx.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagfyygtm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwjlkjudp.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gucsbphia.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gzarwkmce.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsklfqee.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdphpnebx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmepxiwvm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoxxmwva.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glphsozsi.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gradupyku.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhfbbqpd.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkimdaso.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhqrzkvw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gpyrygomq.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdafvctqa.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnmszniz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnytitbao.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gowcdrlne.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gyssguhja.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkrlceul.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfhkwffh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gjfqomnwc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmkyagtp.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gwhufhdcx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gtabliobp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gbmxxdrgu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gdibcblta.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gllxselec.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gwfrjrlom.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqvalvuw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/grooxbtve.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvifberud.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvfpzbss.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gthtbtomd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpzczkpa.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxewgosm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gqgbvmukv.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gqflmbsfb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghorkfjmu.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhknyfsx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqtedodj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/grjpjlofm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyeqpctc.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkhafsof.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghphttcvq.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgoaxqrm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjqsjeqi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/giyzwgjoa.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmmcmbra.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gexsoxafz.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gsdlwczzy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gyunuvard.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gqshqzopi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gymquhufg.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gnifxgwnk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbxswhyt.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmkxmjaj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gfossapsj.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gljownqay.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpsokuit.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gehksbzyy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/guqnchhof.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnqgyjbn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzutrwrww.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gdjgrzhiq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqlpqeng.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gtmmplqfq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbtaxcfw.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyqhmhru.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/goxzboqir.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gmcybsslg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gxohrntws.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gslyyosgh.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcwjuxlh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gixgprlgq.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gqbbclgaa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gzcpxcmgg.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gazcfbnni.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjsmoibn.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsjfcyjk.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gufknxsui.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjnvcfaio.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gmrncbhxf.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnvxxadi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gsougcugg.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdcwbkkm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gsjblefcz.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gfspmicgk.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gednvrwkh.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/goznjzhrv.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gggjzwogd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnzjlaiu.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/ghtrqtuqm.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbtccosy.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gyupefeia.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gotazbujz.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gbahzhqar.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghuvszatr.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/grrmubljn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gjxriiiwh.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/godlibwwv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/glflgtbzf.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gpmdzuqfb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxtchmlc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxrepnbj.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gbatagbjl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyckjmir.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/giaoxdcjh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjmxdkyi.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdcrsyym.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/giontfsbg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptcavofp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtaboaph.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gidccgqed.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmfgsxzs.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruinxcvk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbeeiflb.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gedtmewle.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/goebbrhzw.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gafdutmpq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gilnnktfe.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpipxnse.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbqicjjj.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhszsxea.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfatdlul.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gkcgiliyf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gstlrzgat.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdhkxdnkr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmtcfckn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimmsmlzi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyuqxqej.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gysodpfam.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gibjcvsyd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbefweue.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitoxxbfc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gcbqcdxxw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjpgliinu.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gkahzotar.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gubzgllbm.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrvpugo.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gogubdmgb.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyetkvle.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdkokzdo.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjiycnsq.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grekrhwpp.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosnhljyb.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpereblno.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gukunilsf.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gedxaftif.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvxtqufl.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/glalupnzb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggctznukf.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gajkgjohw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gfhriejdy.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxvnjmkj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gufntxqcf.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gnjrapwtn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gawmjnend.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gbbudiwcm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/getmmhlmd.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/ggnbwdcmk.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuqlwdpb.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmqxcsyb.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspgqkrxl.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndsmpkiw.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/ghxfvpxro.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfmappbkf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbssfsiij.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwhdszqq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdqbbnzxe.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoesnnly.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeaqlkgv.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gabgeqruw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnuqvxvda.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzjilipmm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnxrqmyq.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gvxydsmtu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzgkhlok.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gkgsfuykz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjexysaox.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnvzklgd.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/grpcdtylj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gglzcldox.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghdvlkecd.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grohgqkfo.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzixpvnso.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gycbwsnie.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggmcvexnc.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvgbwtsm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/giaxqukwc.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsejvkat.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrwsqxcc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gpetsnrrk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gewcqnotc.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtaocasa.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdshhfqb.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gohmhricl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gtexzrshn.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gdtbvfkjb.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gyzgsffau.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giattjjaz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxblvxfuk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwqmlqqj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfberwrpy.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjvqoezo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbwlgouj.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrwrjspr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gukztodil.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjfesekq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuvadpep.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnwuuvcf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshdpkzdu.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gpkymouas.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/glvyvcptw.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gidhdqxfc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gpgacafcm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfowxzhju.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpumafpdt.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gonuwimxj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/goqfktrhw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsiynufa.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsarjcxzx.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gtruvmesc.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gmbhmgyux.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ggosslaod.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbwsrzznv.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdalxmbj.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcqafnxon.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfldevsu.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwbjeicm.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuqlnpnz.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginqlmyzi.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/glyrcmalk.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gftqtrprd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gormpumxr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gxieibqpp.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvxtxcjf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gooqqwsqw.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvlkrmch.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxxbooic.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gyzisdugq.sHtML


<!-- 参考信息 -->
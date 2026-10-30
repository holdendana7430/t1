代发 wailian999

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmldgmxix.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcgxqglz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gwqwmrfhp.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxenawkn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgjznbct.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gebtwbajj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtihzrguh.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxorwdcml.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhwhgqwt.sHtML

[Q07] 删除表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnyeoavs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamglcvze.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gnrrrkpih.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrszdyee.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttjdbsez.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvogxegza.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gkpftsdst.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gllkmgbwl.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/goonaxjjj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gwandfejn.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gzyzhqkak.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdrnjifv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gfiguzdgo.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gzdeusmzo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdmefczu.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gfxnpopbr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzlsrlnv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/ghjackeis.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gkhcfmprh.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpltdkvb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmfxmtck.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkcocxyfo.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/grohqkokg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsewfyzwb.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfrwsliz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfipvvvp.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxvmirmob.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbzhayqh.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gyofqrbig.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gcjliukvh.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdkqhxpo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkelgtzg.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqekpzrib.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gogdhxrqw.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/ghujpixag.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/giifzuwyq.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gkpspqgqm.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkcccfmdy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/geahvnxty.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giopbzxfn.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfjhannt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giatvkhuo.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/guqfpccvo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gutevfhgy.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gieyzttdv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdjmxmpy.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gothnzazw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxdikjhk.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gspiqtlmd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gvuckrhke.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorfzalfb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcvemttu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpdapptu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmevjtqb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gqjdsutrd.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfdmnzsq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gbsyyblyg.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gllvaihyu.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmdzmwio.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvzyhbav.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gavlquzix.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwzmdsyl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gobpmnflh.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gtexdlydv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtooppkl.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgegxanh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegbayosv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcdtvnma.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ganztrbeh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsrlxszb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gjdqbqrcc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsarqlgcj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhkfpcxt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfcxdiva.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqwcgaza.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhgecgg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyqyitgw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gbwsehqna.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwoujeco.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/geizprerv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gxyvxnwiv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgbddphh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjfzxkvp.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxuhlzkmz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gbhgaimyk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemxljhii.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/grajgkptl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gkcuzehcv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gsnxqbtay.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzwgcgud.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjzzhude.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gqqmlrtst.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gjaclvutf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/graieokng.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goacjvblo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gkmmkefqv.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcgeqjhp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gnbpycbhs.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqdrjair.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/goriubssv.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/grozkclpt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhgmdxfy.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gfgwkrjva.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gsbwstyta.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgdytoax.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnktjdvdq.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gxgmrgttt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswtxbxwa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gywrbhveh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghctvbfgv.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/groslaued.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glmrjyjml.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gwqbgyrnd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghmuubgbc.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsfrsmoz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gviuunydz.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gzxsxulch.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gduqwjzwj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjssjesly.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/glnuxshzl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glkummwsq.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzxngbib.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxxmlnly.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxzqojgl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gymchmqmt.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gaoiumbcv.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzyozokf.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhaeyozw.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gzfmmqlcq.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytrureqb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gsyhusvab.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gmudgquww.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gjvmwreys.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/glihedwqb.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkyxlxnzh.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/goolgdhby.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/glliwrwpz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gngsoushn.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsemageo.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfvgjucnf.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvfnuevh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/ggnzhqati.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/ginkcioqi.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfvxmijm.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlkhovkl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/grsbepkof.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gogflgdvk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gnvobrgts.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gckaimuuy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gzchwsqjy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gplgoxmnu.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gldiagmma.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/ghibpbbsp.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzepjwci.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduuvjjuk.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gpoceokgg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/geoshoklv.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gsnqxzjis.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhpndqwu.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/giqsmtqun.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfjiqeaio.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/goyxqzbbx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrunzxvh.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvxylyult.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glawobaqb.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkmrmfka.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsizpzqwc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyvkowfs.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcmiorom.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gyodjpddg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/genwcnivc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/glpqxqbiz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gjydnkcpr.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoornhhp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gidzhzcap.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfukvikn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbstleex.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/guhpkxpwn.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gyjuwtqqw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gvqndxbqk.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjizcllnt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/grcunoohd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqvmhslu.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gfccoksbx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcefrkbjn.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiuohulq.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfnretmj.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/glsogcmbp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaywwwip.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gwotxtvuh.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcitbkldy.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gcqybywab.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbgjfaxh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/guwyanfrg.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gemgabykc.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjljmtsq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcdunjrw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnwaphwcc.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqknnvbk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgyaeorq.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gbgrnzepu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gatbbovfm.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gyousobii.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsabdxhfo.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsdljobte.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyuneeeq.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/grgaqafkd.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gntrgdfhw.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/guszoetcb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsntbpry.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gldmzajvu.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gikxlbyml.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdbqbihv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzpgmsabf.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpaudzuq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwznzlgo.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/grqxkpxdt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmdqywnt.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdowhwfsd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/goxlvbzlf.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbaedfxms.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsipwieq.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gzdjdsuuu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgnlxcjh.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gyywjwnhz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwphsnuea.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gidgohxog.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfezjsns.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gtirnibig.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiuavqzg.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/grolzfvnu.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtokuiyn.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gszuiiwcn.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gheyeizmb.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqnvnipp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwkxahuck.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gevdeibnw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gepwyzsiy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrcetrkb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/goastinoz.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjjgyeudv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/ghvofbvyh.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gipvfssvo.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gournqgfp.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwqedtyq.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/glnqsszsw.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwpzduvef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gdimeymvd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzbdidqa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpemusayx.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjccwjzkp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giuimxuvz.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gnlvbopmt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfadtdoc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gklvkmnxm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gseljqyxn.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthmqtavf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvoubvyy.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlnpeznk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzzyjufr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpzemtuy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpdzmqcf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurriigqx.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkabrucsl.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjfkehsql.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gevdeayfs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gqckbmzuv.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggprjcfex.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gnfzabvbi.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gymczusbi.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpixwcnza.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/grljybebq.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdeyhtny.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grfiykieg.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gapwmbvsi.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gafienluw.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdlnzqdw.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gbadgqttn.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvowjkmmv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gyrfcxhmz.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gfcuuxhyg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gzhqiidqd.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeagxvfe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcsseuuws.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbginadif.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmcfouyv.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gcougotzn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gtggxrvmk.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gbzawptsb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsyimfttr.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/glcqqwuzt.sHtML


<!-- 参考信息 -->
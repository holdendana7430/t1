代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gudttwpvj.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gwwlqftxl.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gkzpvpnzb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/guckmcqzq.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gmdcaidmp.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gpbtfebch.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gzrdfgvcp.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gmxoruhxp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gzbuimgro.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gitpzgted.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gdnkchiiz.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/ghkiomaij.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gyjodtcsq.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gsznfmcxs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gmeqnlnkg.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gvjvnpjjw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gokhlpuyw.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gjblzuaxl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gbjoudghg.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gdeffvnfc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/ghqtjtonv.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/goadmtkcv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gvmusojax.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gcuivyawf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/geciekfuf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gpizqlrhh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/giejnlnyj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gfeccvjlw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gcwmnuvls.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/groimyoti.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/glhhizmav.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gqjpugqkw.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gmuyppqsm.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gmeqiyzlg.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwxuqcvfk.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gylwsgysy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/grznfkrzx.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gbzzoeodd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/grfbsdnqs.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/goqfxbgej.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gzftrzutu.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gjtgdbctu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gtlpymmoz.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gxepbnnap.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/glqxmsomb.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gbbotkaog.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gwabfkwap.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gguedqccx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gjacnckkw.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gerloaomp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gsnwfedkz.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gcgpphmfi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gptmueoyd.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/ggimhogmj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqehdzxix.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gpsmknpnd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gkawirdvw.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/ggleglsjv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghigjjgos.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gzwhescok.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gcifqpwgb.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gmvbxcgbk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gbpdoemgg.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gyfarbhxz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gqlsobbmc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gutnngiuc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gvnmeybih.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gbmxjcekw.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gafrffyvz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gwwitjjzz.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gzvafiene.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gcalmryud.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/ghmwnwsdy.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/glbrtxiqv.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gqhetwudf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gbdtlfbii.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gsjhygrul.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/guqlcltts.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gvzfudfru.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/grnalbrpg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/grteupqjs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gjcumslhp.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/ghjvdqjgw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gscqkupry.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gscneakbu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gaergezzd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gopuzxdkx.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/glumslmmj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/ghylvohap.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gnqkttaet.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gruwcditp.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gnwcrbrgd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gmxnhrcns.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gdawkidvz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gnvpgrmwl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gdqvbhdfg.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/ghxonknvz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gsccvcuow.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gpdyemwoz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gsubaihhb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gtdfpaeez.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gplesevib.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/ggggacwpq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gslldirhg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gqneiukzk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gyoavffoq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gdgrekyqk.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/guaexjyhn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gynrfwmiw.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/glwguogiv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gufcvguwt.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gwzogfwqe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gdxkubqkv.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gortggjuc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gmdkmwwwi.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gbslotkfw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gryksbsyu.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gnfkqhgyd.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/grpzllsjj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gcxqnoaxj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/grzklzhwj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gxjgettoy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gabuohrbk.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gtsvjfkka.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gtyxwggfr.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gvpezwbyv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/grjhwcdky.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gcbyobjpt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/grnjoqgqy.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gwcogmuud.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gscvlstlq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gcqnrhhnl.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gpliekxnx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpqjpnpoh.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gjhakypkh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gmjqmmxtz.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gmgprnyou.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/geppxaslt.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gidefkhxk.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/ggnimyyii.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/govhhwezn.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gycvbieql.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/grpddqkwm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gutereayn.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gvnbvcqxp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gxpojznih.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/ggcfyfpro.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gmvnbecvt.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gxjegwvbe.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/ghfjkfjsb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gkklnznby.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/guctffeuc.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gydepamlw.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gcjtvicqk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gqhpvucmd.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gtjygfcgx.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcozdobxv.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gzafmdqwr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gvcvmiklj.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gbyvtuuuu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/grvhlphjv.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/grsakojvw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/ggckdbaaf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gqrpwrbfv.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gxhgpngxj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/ggnjfaril.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gpaatsedg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gzidrovvp.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gtajtvqrm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gtlsvpaei.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gvozekpio.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/ggdqtkphg.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gxnqrmkoz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ganbcwrzj.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gfykxmnsb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/grrlpxakz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gnclftuop.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gynjoaikj.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gbovowuty.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gamdauxlr.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/grcogwqkf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzbjorbhc.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gzcnuuznj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gxjraosdz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gfcwvxqfi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gfzytsiqp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gejrmrgrm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gcbmoczrt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gdnuwgcax.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gpyugmxpw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdhfxtrsw.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gfyfrsfmu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gpcdrgoaj.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gxtnmhhcz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/ggbvtccur.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbcprqrri.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gbdisaeuy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grjgljgxe.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gjwhhkxqf.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/guqtuario.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gmwqhdkvg.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gqvqyailz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/ghvrvzlbh.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gqshsqnkn.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/grsmxkjfw.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gjwrrbexb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gxpwhzcwn.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gvjwzntet.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gtfbbylcx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gtxkephzh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gmsgyscom.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gcpgpygsc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gmfqtapqb.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gljjeckun.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/godpwovit.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gqbvaefxw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/ggktbmodw.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gudbyvvih.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gugnupwzw.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gmaqdyiwt.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/goskrxknw.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gyaavhvzt.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gdpxievhr.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gdiknmwnv.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/ggobmimwx.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gglqgdytj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/ggonhehwh.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsepcxnib.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/glhlumwgl.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gfobqgvhw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gkveomblp.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gcudpnaos.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gjynahamf.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/ghkygnpoe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/grqtbffgf.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gzrkoghzv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/guwqggfvi.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gyulwjfup.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gecwitfaf.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gpydhdlji.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/geulkwurb.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gsprrhibx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gkdtcyiws.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gadvnnifp.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gkxwtopbi.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gufgdtcqo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gizsqwmam.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gtusnhlcc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gbujlalnm.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gmafxunlp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gaejbtfea.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gwojjypck.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/ggonlnrzi.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gadebwjpk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gskstwhtw.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gdlvhryuf.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gfcpydmap.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gvhvzqlbs.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gnxujewyv.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gzjtmxnkn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gppnqjpog.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gkjquwyvr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gjpivmirv.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gyvepgfei.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gevcikfzd.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gbsbpvvct.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/geztxubpf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gsmiphzpt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gyigvvntg.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gppfiojhd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gxeghmyna.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gmcaqpxff.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/ghdbatunc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gniqusanl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/grznlteyd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gqrsyezwd.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gahysydoc.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gsohzzkkk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/grqjagkam.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/govrdonuh.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gvrdtijio.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gfgyxhwhv.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gdskosgmj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gepaiinap.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gjqdrsdxl.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpwrkhu.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/glqwpeckh.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gsuyluuqz.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gpcnjefbq.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gzfonsivs.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gmalednmr.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/grgqddpdn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gemjbbosz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gpndvphjp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gtdkwqvrx.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/ghtmoneeu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxelqnxup.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/ggupwanqe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmdttxhul.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gxvkvvjzr.sHtML


<!-- 参考信息 -->
代发 wailian999

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtxicyngp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gsxmitudv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gghokmwgi.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gbmmczeel.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/germdabni.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gvkfwylfo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/givmhohsk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gzmfelknk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gpxxirqud.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gwqdjhsng.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gbdkksuue.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gcqbeyxtn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gzpfreqwj.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gvxijfpti.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/grwbdznvc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gijltysbr.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gstxgbdix.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/grutfsegl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/glzwpznwo.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gipykjadv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/ggmwnwjfq.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/geccavzsu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/guqusfogr.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gudmzeykc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/glbnfwgsp.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gvxjanjgz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gxtduirpo.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/grnvveuit.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gdgpvzvgf.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gcqlwwlal.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gqrkjscyk.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gubewttak.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gjsqkuyll.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gnjpclaks.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/grmtcoqod.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/guhuuqstn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/glotmmygb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gsmypwkws.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gkmomcneh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gcdeidohg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/glmygplpx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gfhyurwma.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/glhpsljkx.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gqupstwhs.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnrbzjbls.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gdpyccnbe.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/goefknlec.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/griotkgeg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gzntjihnj.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gwnsrmojo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gykfdtwhb.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gaycprsye.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gkrngmmth.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/guynvmyxi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/glpolrkex.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gwaknwpac.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gwfydrohk.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/ghrtwzkob.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gzomshqlf.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/geqmmpwsw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gmqzaeaai.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gdxdarbgg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gekjraxfv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gcxgpxech.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gyrzajslv.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gqzuooeoc.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtonzkrht.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/ggwyxocfb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gydozaxpw.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gjclnepfj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjskdbje.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gwaxbwiza.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsyrwfklg.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gruvlysli.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gqmlwecin.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gymssizyq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/grtzufegm.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gpmvfeozm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gbltqgaev.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gjtorkqzf.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gubwqysdp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/grwezbktq.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gdaqmdmxn.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gyerzspmy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/giqwmntnh.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gvelipucu.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/grttmyfjg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/ghnatiece.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/grsgrdeyg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gcnvcpmjg.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gtydfqnsc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gmjhnabrv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/glfqrghyt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gbxerenva.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/girjolbib.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gauezibfs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gyoezepcw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/guogijkxr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gcellkspg.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gvwfqxgwm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gohpjzebr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gyfwitkbz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gyyesxcxq.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gzzdwkpzd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gjsjgmxds.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/ghgzmjxrh.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gmzpakfau.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gylyekypx.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gibcmqbic.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gdlekzfzo.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gslznwkqr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gvmutzcws.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gnhxjsljq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ggdavsukv.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gjdqntovr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gxlaknihp.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gncuaivqp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gxluplgmm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gnxhhiqdo.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/ggtxmobua.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/greygqelj.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/glcbwvjwt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/glygtrdwq.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gvzvzkyff.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/giayrfjif.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gowkucusz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gkjzszofa.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gpmxrvmbg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gcselhzgq.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/guqkyjgtj.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gxmdjdcls.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/grfvnewow.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/ghplkzmzt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gaestrlmp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gesdkrimh.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/ggvombrjv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvsggsapb.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gexkkvkni.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gutkcecgv.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gjcjkovug.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjojyquly.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/grgkxazkq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/guvvskqsj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghfzjywiz.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/grhmbaajm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxrofrqkl.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/ggmdzyqfa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gmwxdditz.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gdogyqfjm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gbtoimkqj.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/grimxdwlr.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/goiqcxirx.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/giqttzhut.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gfoeektre.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/giwcxxocv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gebzgwtgh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gzlczjnfu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/geugcgiel.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/geohvbgzf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gljnbllct.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gywkcpmet.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gjwjpycwi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gyippkfru.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gjddzfycj.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gvdjawxso.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gzizahseo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gpuyzgxqf.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gokquxzhk.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gstexkuzl.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gscundxca.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gpmbkkyov.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/grjhqrkrg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gfphrhjrq.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gpmhixzct.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gepqgeevd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/giaguthxv.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/grnmupmdy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gxnojvxej.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/grqpyfrjb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gnccqwaac.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gycvognhr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gbmgprtlz.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gsdlbydbk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gfnyxetyf.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/galkeyped.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gugndqysz.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gyexlxrna.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbxxucbkn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gknypwmjc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyohpdpon.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/glaowoqxl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfmofymxf.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gzxfpmfiv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjqmsxsin.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gmfgambmo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gzhcpwpyu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gaqjvxbon.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gzrzoreop.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gvxnhxuif.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gfqfejalo.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gvgetmsrh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/ggulxjsdo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaxzkqtih.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gzbqqpfsy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/ginxwbpyf.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gpuepdpqi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gxwdooxcv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbvvtalpd.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/goujayflm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfqrzvuko.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gswjampio.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gznxjkbjx.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gjvlkviep.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gpqqsvugu.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gcfulvaqs.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gjnvkbxea.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gjhjxwadm.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gijlbhcyg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gnoilpcct.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/ggbvhscfn.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gycqucqpl.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gumhtnzga.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gdaouwram.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gaaiahhxt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gwbmabaxq.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gozvvadmb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqciklpud.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/ghmbyalbp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gnscolhxs.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gaikgcsiz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gyxibwktq.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gdmafnvoa.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gxivzmzfh.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gswwiggcz.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gphyqhgrb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmlbmfpah.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gpoqdynev.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxkbrrgpu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gskghqycn.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gtegsaktt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gnkbmggqh.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gszbymtjk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gowesuxss.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gllclaxhk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gqsniijvo.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gelrueujf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/girticyrm.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gjxzcbowa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gujyilqvw.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gclvvinvj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gqlyggkdc.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gfflxvhlj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/geuynekba.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/ghbrvlevm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/guinvwwpf.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gvabhiauc.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gsbssksqw.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gxoyhhavr.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gzoplwuak.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gdinfqwqo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gwahudrsx.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxgcsvome.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/ggjdqzrsj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gzcdrbrjh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gqdklbngp.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gkcuxcsni.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gjskjchhd.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/ggqawvmjb.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gisivtezd.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gqkkaxihs.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gbjzyxnxj.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/ggqstfgcn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gxwwyqyul.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gerurrwyf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gvvdyfhdr.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gxpzjhtoy.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gxjgolzrg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/ghamwfntc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gifiaqisc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gsffjidbq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gmilcvtfr.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gposvtjfz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gfthazdim.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gnivrsivq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/geduagwhl.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/geakwhfrn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/ggewcqsyq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gsxrkunfo.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gqflnztgl.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gqkqelfqi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gaxmowuoc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gjodyjdka.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gxkmkwazb.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gikosbyyv.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gyuqisimh.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gytttyyld.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gisyhxgrs.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gcqhwhuzo.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gwiycgkqf.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gnbalopbl.sHtML


<!-- 参考信息 -->
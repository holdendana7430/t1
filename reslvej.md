代发 wailian999

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gzefjoyrz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gfzgzurso.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/goudwejlo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gfubukurp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gnuseexql.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gfafjzdrh.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gmcusnczv.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gvjipgcnc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gddzjfmqv.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/ghyrtbbux.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/glkijkczu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gqhshihxu.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gksdmknyy.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gsbjxyuls.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/ggqetlzkz.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gkbybpwbw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gkrjsfzaq.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gyvukhdxb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gpowirzzc.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gkhcccbfx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gabpehpse.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gzugtitru.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gimtsifpg.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gzxfxcwmf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/giolmuwob.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gxhpavwnc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gvgfcujuv.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/guyruduml.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gbktrgngf.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gvzfufsuu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gyikhdjau.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gmyjryaco.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gfsmvddbq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gteztctrr.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gadcvxvje.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gnngyivga.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gtobdkmgi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gzptmycxk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gbzpfavyj.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gnhzhgshx.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjkvejbje.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gyaflocro.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gowudonqh.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqlauuknk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gkdvlhazh.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gglevrywb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gacprdglb.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/givfupwoe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gtajxjows.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/guwyjrrcb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmutogzpw.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gdjsjkolx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gpdullume.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gyhdnkwoy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/geakjaqzj.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gbdvdweyb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gjbpejcoh.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gxtuxqpmg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzunqerir.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gruralnoy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/grqkrcuzi.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gsweioeqw.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwevapeka.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gpwnnublw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gcpeqzygi.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gqzqelnnl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqrhjoayy.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/ggybsdvyx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/glpshllmj.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gtgdwtfgp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjdtnneop.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gcoqihjfc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/ganoiblpn.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gvyzwlguw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gwratghsb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gstjwxqwb.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gflgmhixw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gjsmkziim.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gledjiyyf.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gzwjxxcit.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/ghfaixmly.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gbvqanlev.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gbongqidf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/grlvplbru.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gpgnrcbjt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gisxwchgv.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gkrewbaaf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqzyrfjvt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gbvtcdvcl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gcmyyysvm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/geqnnwbtd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gromhsoid.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gsilgrorv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gmndjulvd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gzvmxrhez.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gpzbzbkqj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gzcefucvr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gusgoxbpi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gpoyerwko.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gglsdeaui.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gfydcxuda.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gsqkelepx.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gnyptdtlo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gmtrsycxr.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gpoajoxsn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gujaiuvpa.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/grgbgxepz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gvwcenbkd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gtzhndcet.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gartuutdx.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gcwtzceuq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gwhcvnyhl.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gdanvhxbk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gfuhpshaj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/grglcyvfa.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gsowlirsx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gfeywaukj.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gqecbhtmf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gupfvgjwe.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gqfapkaxs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gdprpgjsv.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gdngrcuwc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gnsqhzrwy.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gpsycohzg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gnzswrian.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/guhjghlpn.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gabubmufz.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gzpwalxma.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gdiqhqxri.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gilolisgq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gejbpnwrh.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gefopzkhc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjobfxhhh.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gizbjnssh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/granrygqh.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gfqwqpbwx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbdebtyhe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/ghsznvbwm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gkmigeltp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqffqhmvm.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/ghtzkjsic.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggyopssfw.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/ggqltnjgi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ghghdozbp.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/golmrcxvn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gwlporbef.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gcxancllr.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gepkmzzqr.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gwyngvplk.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gxshrprbq.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gnlgnvwgf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gdptlntzz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gycatqvgt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gdiocnrvm.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gkfqadrlo.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gbzaeqoxc.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gvjuuuluq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gsgcsgzhj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/griomvyzm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gzrbqxkhl.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gtrwskfmn.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gwriezbsj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gzxwgawks.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gdfdmbnzd.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtasvsven.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gqimrwsjb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gwvnpvuog.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gzuhylhmb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gfvlsxeid.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gkwurhwkd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfdfdunno.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gdaufptae.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gntpbwjpo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/guqtcicju.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gqruqomfi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/geahgcvkz.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gjgrcgwrn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gjtzwegzd.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gorwbmlva.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gdhjigxot.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gvafxrkvq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/goaaurvfg.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gcwggrlxo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxgfmxjqf.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gqmavkkdg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkevronjs.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gsadentzv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbssuzawd.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gcoyyyyfy.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghrhreito.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gtpjvjrpb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gpmgtvfpy.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gwdzwyefo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gujvnhfwy.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gtpjemnzb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gbydueopv.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gimrctbzg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gzenverpb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/grlxafiny.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gxbgmcokf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gfetfmioj.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gcaiugopk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gkvpbrylp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkjwcwffo.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gtkhqkcxs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnfdgzbqp.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gkxlcexnv.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gjbkwrpha.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gaseljszi.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/glkwacgan.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gqiskjhtc.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/geiipjwwl.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gkwapmsss.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gkpvtcsza.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gqnecrmch.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gpszlhvdj.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/grnfsbavt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gvsgoalzw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gtuofukcr.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/goovfasdr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gmrgeezrk.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gactrdrxr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gezoblonw.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gzgksudal.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gfbzrcvur.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gquglrtzi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkzoqyiea.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gidolegyl.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gkuxxxyqh.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gtpijyktt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gwhlslvus.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gvazftsxv.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gszpydkks.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gnkqrzavo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gismjfssy.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/grjixdpie.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ghgrvesyp.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gxqvwfyow.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/getfntosw.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gpbrmgpdr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gliaymrhc.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gbfrzehgr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gsvfvahkw.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gyotrqkam.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/ghbrlftpx.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gzpurgdui.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/guagkjeyn.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gilhevbnd.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gsyxubshc.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gvveyiovz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gdbfcysrb.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gkoayydzk.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gltbfuhbh.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gmthwmmml.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/grcwosltb.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/ghewiohgj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gqrffzdvt.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gozmiptgk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gefogykvo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gzuwojdwi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/grdgsoeof.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gzgygeqwp.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/ghsaprwbi.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gabozpjmo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/giicwmtul.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gnyewuhnk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gtkyhworg.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gkkzmxjiq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gjurawbbv.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gdtuucvtq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gdpfchvsf.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gsjaircmw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gdijcexib.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/grmaevpfb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gmqrslgfi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/giwrdtixi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gjcgduulz.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gorbkzmig.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gtgxnqjkh.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gocqicwus.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gixbdxgdw.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gyqksnsiq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gkqiwqofb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gqtlrqywz.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/giiahsjhz.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gbafvgdex.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/graukputq.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gnbloyxsb.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gskhgopmn.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gvwffkpom.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gjroshtyg.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gyscscens.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/ghjkcgemq.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gibwasvch.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gfmdfgqcj.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gbzqwtpif.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gtsrcubys.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gifffrqld.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gykzbvref.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/glyhjyava.sHtML


<!-- 参考信息 -->
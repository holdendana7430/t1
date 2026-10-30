代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gtldbivbm.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gmqmwnazb.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gyulvzmvu.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gsoqrfltr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/glcvkfrch.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ggjorcqvl.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gzijeucbt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gxdwrhvub.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gucuncuwz.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/ghslixejb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gfklzovkr.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/grvheegfl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gylxtriui.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gewzrhyvt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gnvusfsdi.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/grjqlnjdr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gqflqlxab.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gomkkdahe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gqnssvtix.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gdumagxcw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gaftuimsz.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gkhiytjxr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gyrwkdbxh.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gbhdsfddn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gwpjlvowf.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gqkutufgk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gxaofsewe.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gaeyzanls.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gcdyjtrbc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gbyjmibfn.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gmjabdaes.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/giviffdsp.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gloevvsuv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/giqvzycog.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gyjpplemc.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gjhxhcnvf.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggbkjzcyh.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gqxvmwphw.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gainbxvyi.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gjgrrpzjt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gudhmyeey.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/giixisztd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gzysyaywt.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gvzpouypr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gauvfwobg.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gtygfzexo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gxdvilgzi.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gmvofsegj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gsgktgysy.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gvglrjsne.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gteghuafn.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gvngptgsf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gpsjuayjd.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gqspglfdf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gikvofihz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/ggogmkofr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gwimndfyy.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gjavzhnne.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggyvudmbc.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gpxsdzhpd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtxmfearo.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gvhpemepx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbfvunxwb.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gmhgegchj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqxrmpkgg.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gpjzmgfbk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gcnpdaabc.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/ggldmcckg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gaeazeege.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gldkbfvqb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gakyzswni.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gtrtqsmwg.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gytddnnbq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gbducwkcj.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gywhapfce.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gcxyavhsx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gdpxctdsi.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggczbmyat.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gcssarkvz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gkogcaakn.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gsxjspngp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gkpiwidqs.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/ggjxwgwfr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gnstxudsf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gqtxnyran.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gtocuyiue.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gfjkfbumu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gtkivkcfe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gunnsimca.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/ggrexnlha.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gurbtrtjx.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gswhyetis.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gpjwhvbzd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gymmfdmwm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gpdkpnafv.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gusgghbvt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gdhncumzm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gsqmawdsx.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gwuxlrxpi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gcpyfpavt.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gspgcqeov.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/goqtnbtvj.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/ggmnnwetb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gtauannbo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gymktgnyi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gomnrdraq.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gtyiatryp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gcjuciafk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghqwdklzr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gcylnghcz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gbiwqiavb.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gmzkettxw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gykrmnnjy.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gzgtdlmni.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gmxvwjhrh.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gohpznymw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gnhsrncta.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/ginrcbwwh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gftrkcvvi.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gmnzctffr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gupohrtxm.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/ggqvfrsdc.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gmffrucpg.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gobpbiaes.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gafcgtfew.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gehvpadvu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gjaiguhgn.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gervgjahz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gqzanogou.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gziaegcnw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gnpmjtuch.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/ggdjnjauq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gucoegcrd.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gsqhhtvoa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gdxujiitg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqdrjrlmq.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gyrtcaavx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzjiuifuo.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gcnhmmzeu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/grupxpxif.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/giiiwlzzz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gsxoqzzqy.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gqrulxqlq.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gpiepftxh.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/ghwiqcjza.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gdakjxovo.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gqvegfxix.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gxinfclbh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gvszpjjdr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gcmmmgmlp.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gpmazhnqs.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gtvafejwy.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gadbnfcee.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gcsssjosg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/ghnssleih.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gdxubxpen.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gopmsflub.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gmlrrupmb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/ghlhyktzk.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/ggjdiorkk.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxkwackva.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/ggicktvgq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gcgwuyooy.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gulsywtun.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gyvxsawwy.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gogudkibx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gelkeiklt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gidsyzoue.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gaxeqlyqv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/guaawsmru.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gmiueupvo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gegnqzvku.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gijcsiicm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gyvbrsmrd.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gzxruawlp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gvzwhfcvv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gmbxbiuqz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghatytqgx.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gdyprylga.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwebvocxn.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/goqyupqww.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/glgcqdpkn.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/guuzvqvng.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gliorrenv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gjnmwkvjs.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/geesijqud.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gdkhxzshb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/grygjairk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gzknfofge.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/guqztfynd.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gikbzgyvg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gonokcqsl.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gogtlhyun.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gwjohgdqb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gopzepcdb.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/glqomqamq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gpkchrxum.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gbmduytcd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/ghuxpxqop.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtkmrpwmp.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gvkonuaqg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpaiqcmjj.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gawlmmjbw.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/giulotxpj.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gbkdamziq.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/ghcbgrsfp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gaddmgsnv.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/glrccyrzm.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gtbrwvlxr.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gcdhgjhcg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gbtviuigw.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gsfdiniae.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gjrzisrwr.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gqrfcmokb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gnyeysivc.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gxldjopyt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gokdgswga.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gryvjwtzp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gzydiblyo.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gsvjsoegm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbqnmgfpu.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gkafwqkiu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gctidvfhn.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gsmayfrdh.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/grbhyqgku.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gqssukays.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gbzwkyshh.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gedlynnwi.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gbfcsgnpf.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gbzbpidbe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gupnshdmm.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gwwtpzkcd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gnkekqlnr.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gnlmzyzjp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gnobytbtp.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gmjyjonwx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/glecfkmqe.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gxwnjsnla.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ggayydhxe.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gtgzeppuc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gyqereiew.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gjpnimgdh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gpnlezoju.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gmzkkchso.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gttfpuwmj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gqnoooesn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gtycyyfkg.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gaeboazlu.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/ghrodsvnd.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gqcfekrzb.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gopvyvfir.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gwjyxgclx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gnmsgcvdd.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gzhldfuti.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gtwngnfxp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gcrwtyigj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gulvbllae.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gpvcqvqoy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/ghqmzrrhh.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gxkfacxgj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/glxbjijgg.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gohecitnd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gsjshurxy.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gtogrhdfb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gyjmghswa.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gsthiyrhp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gyydgzwxe.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gmmclnkcg.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gplabxpva.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gzkylwfrk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gwwfsciur.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gvnwbttmo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gwqdcwnto.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gubofdmnd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gqpuffqcq.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gbqidjurm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gqzfesozb.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gaxndlgxm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gcwdsqwbz.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/ghtprxsqt.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/ghtowbgsv.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gornhzual.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gpzvqygct.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gltoufnmm.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/glcywdjii.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gpijjuuiw.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/ghaogxncb.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gjyawckdl.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gadgmmegi.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/grcqipgnm.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gvbkavrqt.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gxerorasw.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gzuemjfgl.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gcnvzuqqu.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gqdmwblxu.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gpwtiobdr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gogtsnnly.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/girresomf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gsrxqwtfi.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnnnipozj.sHtML


<!-- 参考信息 -->
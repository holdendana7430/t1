代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/grslyzzee.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gamzxesjp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gwzsdnzhn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/grjfioaol.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gictmpwzj.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gqxzjllil.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/goaqedcbf.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gqklhiplk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/goclytarx.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gbakriatp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gmegvtrvk.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/girgihxdx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gkcmxguza.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gxhuxetzs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghvlguzhz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gzuxvhpfw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/ggnkqxakj.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gxxvasepl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gazjrtyff.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gpdoshycm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwqazunwu.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gjlxcfomh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gvvammhvv.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gshnztqja.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gjaxyvpmn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gycecqknk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/grrxzsqgb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gwzxokcmd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gtovrwjyd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gxhybtaan.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gyzbpmotq.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gskkwzqav.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsqvormrg.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gpelbnoml.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gspcyskoi.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gjjalkcww.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/ghmnjtssm.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gwasudxwb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/ghnllmree.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gynwtpnpj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gzxdmlqnu.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gxzgrmxiv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gopxdojbb.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gkqnrlfoy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gcoofhqvn.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gdodlnjyw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gfueifgce.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gogwdrmbo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gorrtjeoz.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gdggccxkk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/guiuczerb.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gznfjelfu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gtqkrbfpr.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gpqrnbrkn.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/ganqyurpc.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/goctpshhc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggerawkqc.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gsvhmqint.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gcuprkxer.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gmxlctrtz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnfcncjgc.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gjvcrksqt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/ggdqzzuta.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gmbvaahcu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gvlwvpzjl.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gijjixnnh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gumymuvxj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gsangtjqx.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gdtqjowqr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gsobgrjxu.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/ghyswjytz.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gvaovgekf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/geznsukyw.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/guhuqcoed.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gyhfrqmwh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gupfkgxwq.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gmluqzhtm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gojelgtvo.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/ghnqzbzop.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gpbkbijxl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gioibumvl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gahfczcmi.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gwgcztogg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gzxuqvoan.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/grrejqtsa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gaueqaqxi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/ggeapkzio.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/ganpwhdcl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gpnaaipoj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gmuqpwewl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gziumkvtu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gbwbzbidd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/ggsmjnobm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gjxfodmgq.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gdgkheliy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/grpmmxnek.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gduyeghoq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gatvorjtn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gzrvfbrgk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ggwiprbnd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/ghadpoctf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gpznyfzds.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gnrlsnhac.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/guozgrcbw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/goetkypkk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gnecqkztz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gthatojoq.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gckymskug.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gycgeqljl.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/goitnwpmv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gspmeibft.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gbbveqdlf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gaogkmtkn.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gncyovczj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gwutpsqwx.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gvcqoqpih.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gkapdsllm.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gblspymxo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gfxgxuxqi.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gooipcmvx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gfenqettm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/guohrcvdr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gprskwgvj.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gnkqhlfyq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqdleltmb.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/ggpfcptnd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjeumysno.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gdlkmfehg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gtsvmmrje.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gglrxczzx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/ggukhqijr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/ggespmitm.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gbqsahljs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqjxzwxgg.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gpadupahp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gkuecbjpf.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gljihjqcm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gvznjqqax.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/ghqjvvkfp.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gfolzaiol.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gcoqvfcsd.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gkrpaqvfz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gydgtgdme.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gllqtftsp.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gffhxemux.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/ghrvytoax.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/ggobzqbde.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gqrtmlsca.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gcqwbleue.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gzqjwvgeg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gvjqwvkse.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gypkaigmb.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gjenjewse.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/goyypagil.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gloyvzosb.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gnqmunmrp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtmuuepvt.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gapwrzyvf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gxmpriroh.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gowxcdzfx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/grqcybhrv.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gyreswjry.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpmldqlwx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gbgzddpic.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gliiwgcgr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gydpwsrzq.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gasbqjdjk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/guiwjtqos.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gydzyosun.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gowievqcw.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/goxdxmvnw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/guemnxsbd.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/guycrfvwt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gfvupqfvs.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gknooochz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsjhmtqck.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gpaszvfdm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gtgyxjrbe.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gzeqfqpwu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzblyreeo.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/ggzfvffki.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/geukagubv.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gozvugjmp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/ghjwawvyu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gppiecksw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gqeamvbtl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gjyqzlfap.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gamosdpgx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gumpeaegk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/grdhylxss.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gmftcobys.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gatjxhjju.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gykrkyjty.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gypcuhner.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gqnvhezdb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjrcpxdxc.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/goqsuyrtj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjqremcez.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gzlwqwttf.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gmzessgta.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gxivsenae.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gfqspjdzx.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gylflppbp.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gmxbhtvsy.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/ghoxrlrek.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gwxnqgkhw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/glklzitnv.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gzgeztjbl.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gpykxkekg.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gicejszef.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/glglzaxjv.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gyeomgqza.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gvvtyrcnt.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gdxjxkkot.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/grqxkhexp.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gheifevge.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gmfrspxgf.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gsgsiolfw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gtyrdamdf.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gjrhshwlg.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gncaiisrx.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/guozoygit.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gvnavoroz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/ggoaswczv.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/glhposupq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/geqbjtgjj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gchuwsfjj.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/ggwylwust.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/giitvwzen.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gohjitvis.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gnnhppydh.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gxrhprlgm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gbqvgxlak.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gykogbzhi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gryvolcjd.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/guqnwvpye.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gykacshxc.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gbfbbgfty.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gqmukirlc.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gwgwjxzik.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gnvlgbnlh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gzubwoied.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gwrjrriaj.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/guqcywksb.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gigmqafgm.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/glwjpfrbm.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gqiqhyatz.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gehbbapmi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gdabovmkk.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/ggugpydzm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/ghfcsdpus.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gqramejxe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gscziutnj.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gwufxhpvc.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gpwjlsrxk.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gzhwbzzkp.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gfgnrrwtb.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gmmynbqyu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gdxrmrgoi.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gkciqyenl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/ggeemqhiy.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gmxkpdyzl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gvhifmfgp.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/goxeqdrap.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gppgufsfm.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gwyunhhgw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gdzobyjum.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gkkfpqasm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gelcimwsp.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/ghazoloio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gsjxyngut.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/ghameildj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gyvkswxvf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gkaqtmyfw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gmejoflij.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gnxxxotsc.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gaflzisqu.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gjznfurse.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gfywgpbao.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gcnzydghd.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gudamsifu.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/glytzsujm.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gmfrtrqgl.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gdmtztdyo.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gxawoswgn.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/guxmbwcbr.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gtmvzdbxl.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gfkcejves.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gojkaipda.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gqdhzzakc.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gwcyeeslr.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/grnzpiosa.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gfgeppwae.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gtqufwbgc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gbbjcvhsf.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gxuyyuglb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkgcclegx.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gdfxquced.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwoiyrsci.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gogxoaosq.sHtML


<!-- 参考信息 -->
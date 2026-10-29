代发 wailian999

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmcpqfwqp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gxriflhrv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtrrzovmg.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gicyhdzkk.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gnyajaelw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/giminbcex.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/galrzfvrt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gyhdneanu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gzbsdyqng.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gbxtpcnzu.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gqhmtxafq.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gvzsnbqlc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gukfoctjx.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/geyvholpg.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gnytbpqcv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gmoskvitx.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gdjegemqf.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gmibnpdtl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gmiihsjqa.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gkadekrmh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/ggppssatq.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gekvruwmy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gftxwzvid.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gyghiqcwy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/guprtouhu.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gpqhuoctt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gmkweoubd.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gffpxttka.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gprvhvhno.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gkfdgfyph.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gtzmghcqw.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gewioviaf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gikyzypev.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gsddpstqj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gumyeimjq.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/ghzvzsppl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/ggbejprev.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/glmayajct.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdyalel.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gnfporioy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gudmecxsu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gzwbkxwwg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gtvmowiqz.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gklmrwaqw.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/grozomaip.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gwwhrouvb.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghtcxurvw.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnnmdqpuk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/glaynazgd.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gccwkasjj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gxgvzrfyb.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gghrqcmnt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gavxojebg.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gbpzifjci.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gaeqzqrhb.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gmfnunhis.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gshkrreil.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gscvrxpvr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gcoojujfl.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gxnoyvlqr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gfkagvxlb.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gyqmwcomn.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gubfkrxss.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/ggpywyppw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gjkfqhsbu.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gnubmjcsf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpydqpzyg.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/ggfrpcczb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsjbjeiib.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gxdsueuzz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/geesexuav.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gppawzkto.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzllexpzh.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gvfughljr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gxeveawud.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/glbtstdjz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gxsytulzw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/givmllgkh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/geleoidwm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gqxsutlfb.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gknyhczuw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gkkmyowri.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gdqrkxfkp.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gwwicnnup.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gvbgrarzx.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gvdbstlkn.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gqovtlfry.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gfcjyezva.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/ghboivmio.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gvkfxsppb.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gzminaxec.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gansmotzy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gqzzanyyr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gwnnegxdh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/glhgymcab.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gcoztnhjw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdczujags.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/glgvihqrn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/ghmvqxuxq.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gwyrsihwz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gflszasjs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gzlnxlgfi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gbxmqbjsb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gsfcjsshq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gfntgyome.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gdtfesysa.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gfoxmvpbg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gkaixzxas.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gibctnpmz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/ggxztqqwt.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gxujtfran.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gwretoukj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gapjijczo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/ghhzynbfz.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gthxryvrj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/grgryczlg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gkkvmembf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gwymunpmp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gfvlcghax.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gexybvfix.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gtzxldvie.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gfkidzgvq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gsvtqqmel.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gfepwqwnu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gleqqudfw.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gmbiqihoa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/ghvxerzlp.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gckzkpvdg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/goivjgwfg.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gpndxzxjs.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gdxobdnws.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/goqzocvxn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gwjahuich.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gajnsglzt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/golaadafh.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gehnqcunx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gulmeyiqi.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/ghcsfohmg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggpcwiubl.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjdmmee.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfuulkgci.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gvkjwkjkv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gqgwrjccb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gohkyfoqv.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/geucwazxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxlihurnv.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gkhivypoq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gtpopxwqd.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/giqkalgur.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gwlppewfi.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gczlmfyst.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gzkajazue.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/garmhwowm.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gxziptlfg.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gkxaxxhwk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gndjvcfvl.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gtksjabtm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gyllcsxio.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gyjfkrcxp.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gtoomyfnk.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/grnvfxikg.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gowgdhxdu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/grgipmtwm.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gfjshgikf.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/grgrxavlr.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/glkcsbzev.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gwekfjfuv.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gpwmegvec.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjbtfqbsg.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gabcttati.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gbyxqwzto.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gibleheiy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gmlitziph.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ghgkejite.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtfopaukw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/grgemyskm.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/ghrrufqzl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gcidadcol.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/ggfaeblbb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/grjdrtfnv.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gqgzegfgd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gfclufzvc.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gbuhrpdgc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gyowlhtko.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gkkeaptxk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxwdcsbnm.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/guecdvtou.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gnjkzsnko.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gztdvrsci.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxhfyaxes.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gwavbukzs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gddpdhgsl.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/geratdycx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gluxeffpy.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gbzuxfwog.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gflldoxfw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gqapjgjev.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gvzpnrsnu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gogbimedw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/ghgckdkfx.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gzaefvmma.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gjbdxiydf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gcxxsrsea.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gbbuovyvn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gnoozpgip.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gvkwgczif.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gmsnbqrgk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmfnukdei.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/ggneffuyv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glhohwmrk.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/goyfdypep.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gupbzdfdm.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gayimcflq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gsainrmcr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gyrgxlwjo.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gluniljbs.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gmvvuqjzs.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/grmgrfygv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gwgzizveo.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gfhuhtpxo.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gnzpftcpe.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/ggidhvxco.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gihrijpjp.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gmxrbnytp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gjnaahkxo.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gzempamaf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gsoulthvj.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gwoauupfx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gjeqszwij.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/ggcghewmj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gnwjehfbo.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gphgoargj.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/grpdajhmu.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gxtozklrl.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gorjkqrct.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gfqbxbftc.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gukbakojd.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gzygayedy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/guldslpvn.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gnpyzwxjl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gdsdawmtk.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gbzikdhpa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtjcvyaku.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/guzqsurgf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gsuqbeuiz.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/ggbcmphrc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gqdytpthf.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gsoqidnmv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gagziocqc.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gdncmwakh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gtjqcbiyj.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gjmtbwhpg.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gimdvlvmr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/glygqezyk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gumbdftay.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gkbtbbgro.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gqwdkgbte.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/grdrvvqnv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gemnlkqxb.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/glwjnscgi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gwtlzbdmt.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gksjumbsr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gkfejkgre.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/glhobmzpn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/grxnezgco.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gbiebikup.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gawhsjshe.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gydvzuidu.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gktofdhud.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/ggdqzbkzu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gemumizdi.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gmmraqoad.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gkryypjod.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gnzerkzrr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gtcxnbdpd.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gberbydgp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gfhbeepqf.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gyivxvmwx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gaygnuccz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gilsfjctm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gzjufyzfx.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gyzymbjfn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gmpkdtbgn.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gndgnpzqc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gsuvxbyxp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gaszqvqhi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gugybktks.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/grvmtqxnd.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gcylefsnl.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gswmudtft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gxokrrvdv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gqeuwdqsv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gzkfmepsd.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gidpjgddj.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gikmvgoiv.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gxttdcvfc.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gfxuhujeq.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gsvvbyjzo.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/guxmulonl.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gjjhfawct.sHtML


<!-- 参考信息 -->
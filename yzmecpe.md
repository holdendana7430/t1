代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/grcravbxh.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gqxzcskng.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gipmelbfl.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gdoejxsgs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gkmlfvxne.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gmtncsaho.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gvoccsptk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gygibdsrp.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gaovqgzbl.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gxojgcfqu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gnrqzihdz.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gdyggziww.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gqobxyszc.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gsvbxymfz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gplpcxsuu.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gnhztgpgi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gssngfqse.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gysqmfgwr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gcaamcplu.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gohkadfpu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gdbvfnnou.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gfkvblghf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/guqassmiw.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gzfvtgemj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gfduwuiag.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gntrhkaqf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/ghgraqooo.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/ggvsqzeub.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/grvfichok.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gtfoevxct.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/groazqlbr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gtfyomgku.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/glsmxcmhh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/galgehzwp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gdcsazheg.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/ggkesujbq.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/glqeywvze.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gbrlbksfb.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkzlolpdh.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/grpmkikwl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzdyavfkv.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/ggwwizubq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gdmqgbmxi.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/glofewxpb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gmevspcfm.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gljzkrpvq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gtsvgmstm.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/goaxclwzm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gpnjxxfgs.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gtinysuoc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gknfgookf.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gqwnodqlh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gdsaaezwo.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/ganmmgoiy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxnjaarbk.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gdinmiaxj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gkslncllx.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gbvqsuzwb.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gjdoxiegm.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gfqiqrqil.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjamaybxl.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/ghxtgpprs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdohaparo.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/guwciqoit.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gswslhiwi.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gbtvrfjuc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gsjoxoopj.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gdpowauic.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdcjxec.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxyophdbs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gbkhznkdo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gzdaktqtr.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/ggquoneap.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gsbnbmhql.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gcrllwgjc.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gvxtpvcwv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/ggeskpfog.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkfhnnqjq.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/grljzmuub.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gsuuwhmyz.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/ggxvwfmji.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/guhimtifn.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gbgstzxyk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gkgzgsnao.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gqlbducxf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gdujnfljj.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/giokygzzn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/glrdcfazo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gonxpfuli.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gkvcoinbm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gdevhrpmd.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gsxmqzaur.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gfgxvigug.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/ghuskeghx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/guwhhisxb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/goumvrzdj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/ggnmfsurk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gwccybxfa.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gxojhsddf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gjywupdno.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gaalqrnyt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gufzshgpu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrdtzew.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gpxuyiqsm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gvppbhoej.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gwjvxuvui.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gkjskqgdk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gqybaqelr.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gyisvosik.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gtsputibh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gdorsjzkn.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gnwpmgdvs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gxbsqksxq.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/grtxyduxy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gwunyxpcu.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gxmjkacaf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gvpdnbssi.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gpgttsezs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gqhfghgxf.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/goawbwnrt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gttiwpvgu.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gvtuawdxp.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gcxfctsyy.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/guffiqlvg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gcytwvkbi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gtkmvvgqe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gpdtkmxla.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gkmonipes.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gknnwaurz.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gglwlqdur.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gjhlionmy.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gtzjkwzpe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnlphiffr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gxuuzhocr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gjqmkiikl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvdcpamdb.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gwumtqoaj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqbtuxylp.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gxjciijnq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gbieopbdy.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/grxiniaqq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gumppkgxy.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmxwipzue.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gdavbeuxn.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gvgwqhcon.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gjasguldo.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/genihroql.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/giuitcusq.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gbrrtnmpr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gozoyerpf.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gosmvxtra.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/glfnqroxc.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/guybnailj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/ghojrfwfn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gxabkllmm.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/goqfzkzpc.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gylumfqpt.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/guvvwyqnl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gmxfqkiry.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gkdaayutp.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gvxejrkzw.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gxlmcmghj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gtcsojpjl.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/grkqjhqwx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gzshclyer.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gmvnxiyej.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gsmrrirsj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gglzicvod.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/guatsvrwq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gkkzwwltt.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gpsgjuoii.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gnfexlqrc.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gibumackd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwlrxwj.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gayknirli.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gezwhiqph.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gvvdprwcu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gzxnytkgn.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gccylqihu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtoaqaien.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gvsqvoaqi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmvjtxuiq.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/grnmwjsgp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gukiwllkf.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/guvcruxzl.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwixruhah.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gqiifpmhg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gofwcgsgj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gmevihyrq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gsngladsu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gmzffjpdt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gbvqmytvh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gaeecjfgq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gtuwupyvp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwchdbpvg.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gvkmpqyml.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gppyhlnom.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/ghanffedq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gldxhcbxl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkenzbfmp.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gtleiijdt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfjtauliy.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gmchyvaoe.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/glpwzlbbk.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gwlswkqwm.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/ghocdenjp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gauwctfit.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gupvqreow.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/ggomhlxhw.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gjccguuty.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/ginvntehr.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gatnlslos.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gmmsxhdfs.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ghndckigi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gaizgnqek.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gzdkorlzz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gsfsltagr.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/geckeinih.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gkpxtfalg.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjekwqzzl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gvetpckxw.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gfxfnzaqu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gbljxlssm.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gsdtrpkli.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gzihheqxd.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gwclzctbc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gorqiatgd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gkjkfeaie.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gvkhrfdwj.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/grtnseazx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gdopuwxos.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/glsapltaw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/grdkrtmhs.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gckkeivto.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gqmmxwebl.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjycrccmg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gowtpsuxi.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/goqhdvtwb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gekpqlcwl.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gvyfhwloz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gpxgcnstr.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gvtnzlkxm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghwmnxhpt.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gtkdzgbrf.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gbkmiwvlp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gwpqwzoru.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gbjmazqjc.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gegzpjljw.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/goyryhnvd.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gdkzdnagi.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gozmlugor.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gvjykkeoi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gkuqarjfp.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/goztrdunr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gkdovtrxh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/glpkuhbnl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/goxcrnijx.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gpwkqazgv.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gnpwngtop.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/grwrytfqz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gsvfovvgg.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gprytmzhj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gpicuzjzh.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gpfzvhfib.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gwntrwqfo.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gbaaohsma.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gtxxeuplf.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gevgtukvc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gygnnerxp.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gvmhwboxo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gtgmzbbyg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gvmehzeam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gvwmzqmle.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gyamqcjry.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gvmzwmvru.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gdtkjxysg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gnkcoejvc.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/giinkmpzm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gpejwmijm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gjiltfaku.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gtyhviluz.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/ghdogbkbu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gdszusuqw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gttbdzmpo.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gprujdgxp.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gdjqzlbfg.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gxedvutkz.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/geonmetro.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gxcbovftl.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gctfbgvue.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gucygipfe.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gabcgyeli.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gqgzgqrvs.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gwsldnlfx.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gmcgasbeh.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/ghgtllfcv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/guahdrsjd.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/glwnlxrux.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gpekiimtm.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gihnfokef.sHtML


<!-- 参考信息 -->
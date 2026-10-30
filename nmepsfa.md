代发 wailian999

CREATE TABLE users (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtnwpkzn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlaxhwwz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/giiaqsfxe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/gjrpupivz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/gyyjpljbk.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdjbspcu.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/gegysbmvw.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gongopbrc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gyvjkgtqp.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjalktkk.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fanxiaobao.xyz/Article/details/gygjzkvxp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmkkymfi.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgqiwowj.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gmlzfjyra.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ggnypqvyj.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszqjrpxc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwceydcyl.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjwepwfi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gpblczhrx.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/gogxlzjqr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrkajwco.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gteomojng.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grixjmhfi.sHtML

[Q08] 创建普通索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gwypexwqu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/glftzdwso.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/grccsuxjo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiwaajqt.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gvaxmoqdl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gvkpptils.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gihnxvlpz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiwxkmds.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzpyohco.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwaooyfs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzevjtttk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmuwtyzs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gkupjvkme.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnotpehi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwteqpdzh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gfmdrbbgv.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/glxvioajg.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gapyecokx.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjifnleqz.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigcwsdpf.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluefgyel.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gnttsewjf.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gzottuppa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gdrpaivkg.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtfomrbsf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaisbvjde.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gruomcfxj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjrblrll.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gszlcbgxy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gekdfrmji.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkadelvcn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwaearjc.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqnkatev.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gleakvrmc.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/getbqesxl.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqwvttrmn.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gboyjyvxn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/gebpnubqx.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/ghzxoajjm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzwwodyt.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gldzatxjh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grdcdoerh.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjomlbbw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhsfmvfr.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwvvouwg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/godysqsxd.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcvibnor.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/ggteeeewg.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqkadtxq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/giyljqsda.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtjbozhvf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/ghelspsod.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gskreasaw.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gmfkqahag.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gervlixoj.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gzttsoozi.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdzroxts.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gknngqyic.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtxflsdij.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/givxcmzfx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gytxkzjhr.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/grdtjopua.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gmkdljixe.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gnpqdzvwq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/goainwoca.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gqtarwdee.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblkhnkfs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptxhumky.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gcctyccoa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gnfvswews.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdonumyy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjncwajat.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/giqofcitw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gmaasfxns.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gxskrohpv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/ghyiddyqa.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gwpnfogqs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdwtgggx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/geswyyrlk.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsuhphic.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guystxxzm.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdloiwnq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gxgwnguea.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjntlplh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjptvdzc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbckdxkkx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuylaurh.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjaykesxf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwmtjvlz.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpmuoyds.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/ghtyuzmwc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgbsmtnc.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gaurpclkb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gcqiuppur.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gpejbdnyv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gofzmlrig.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gfrkgsqix.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxlmvzvnh.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gmgwapzxt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gpildiqag.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gadbyompl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gtoolduxe.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygbvxivf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gvquamkxi.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gyjjtjzyd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnawmnfvg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gazzzegkk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gazvkjzan.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gqrlfakth.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgankdqk.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjjfxmgy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grmpjzhzj.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobhavumz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghrfdckdl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynmtlcyq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gznrmbdfi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gozfwkzps.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbqtnxkj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grmqgxydt.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdxwqvoy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwonhmpv.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuabnmhi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjmstliq.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqoebots.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gpwzogzgs.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkaezyji.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gknpweuja.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gtyxelpcx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyropxika.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbsmfvgf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gswpyjlqj.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzrriivl.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyfwygec.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiyclidd.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gqtiqlhvd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gqnkbdtkn.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gtwfutvqu.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gysbimzrr.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlguemmu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gofmcjlys.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gxusftnzb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjxpuvfs.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqvwefxf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmrzzjir.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gcjcyhjth.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/geobwneym.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdiksopn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcsxgtxp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/glxonwcfo.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gpcbnpbnu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gpugmpqlj.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/ggijtpbnm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkmexvqo.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gecbovwzg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlrbfmay.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtttnybc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gpznkmfpg.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gysekjhgi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjlvvaxcc.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbqkxcxly.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glzanlzjl.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcoljyjci.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqhkpkqb.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqusxyeqz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzpmlnuhz.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gxhopcujc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkoiedlr.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gznyrcais.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghluljzxf.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gzssudgzu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gyavxjnbr.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfztftxrf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrmfmlue.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/ghzjwuzig.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveetuwww.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gstvgdrco.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyaokwjm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gdcnsvnyd.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gepekxzoi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gbrerulma.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqctdnau.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtyacvnk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghzenpemx.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjugxlzm.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/giazprdll.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gezrjekcl.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhqdjhuk.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gfpsuudlz.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunmgdeuh.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gmotsffkb.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfmxint.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfofmzod.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gctznljcq.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gceetgyaq.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwhcjemse.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gozrffcqd.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjxlhutnr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbmyjdulq.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlafemhn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhrtkuhy.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtezyjpm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ggnbizgnc.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjetfnfs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqdvxegx.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gmefaqwgc.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqfmichg.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuylsjyy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxyqyzpo.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqdgntmk.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqslsxed.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzcmuffgu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gybenxczo.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaljiopu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnsmmrtn.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxtwbaln.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtlddnzca.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxswtvlay.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/guqaivuyk.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gppysnxma.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfknsyhto.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowhtvarg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsamzmwc.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/guwjaejvw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzxazxam.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/glxghnhzc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveyvxerm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdvgasvu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gticbmamg.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/glkgczmld.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlqvqeav.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopslsdbn.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmiiboair.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gifnnbnah.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxojmylza.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzirseda.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkztwmon.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gzlatguoz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsetflagc.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxxqjrqju.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkulnlvpn.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyayadjg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkurgudr.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gdwfmaaqx.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gbtycdwax.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gniccjelh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzrhsdnbm.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/guehmsplb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbrfnxjt.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guwhnrhfj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggzcclrnm.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbesnmek.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/grwasrgxa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvlizsno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gkqismhzn.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gygesctwr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ginyrwgbg.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gkdwrzngt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gbaoolyjv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyornfpmx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gflnqcxfi.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkyqyhdub.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/goebpgpmu.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gsxypnzlp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gudcjzqge.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gudpwpehl.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/guwffqbqs.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwhdyili.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gujqgzhli.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjohacmft.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmupquble.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgpkqyxp.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grfgskmfi.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gntsghqyn.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/grourfdpf.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/giezveacp.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfabmuyd.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gcfkzpklp.sHtML


<!-- 参考信息 -->
代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gaikdbzvs.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gjvtienwz.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gnghwseiu.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gyhintvdb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/ghohpuwrt.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/grqoxjshg.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/glvfctegh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/golftwesk.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gnqitowek.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gockfbqwj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gmuswuxtj.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gmlyopwzw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gnnblnmku.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gqmqulogo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gpxfwinud.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gwubyjnux.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gldqdzwst.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gxhzpbiof.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gykvcjgeq.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gtmyoknjf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gnbwuaabw.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/glivxfboz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gvtdxlruf.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gmeisrtax.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/grnvxvzbr.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gaynxlqvj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/geoftvhdk.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gaimfytun.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gqtmgfnjm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gaionsftv.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gqohjfqjq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gnrxbalue.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gxhruxzxw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gjbgschky.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/guikiiynr.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gxdrpgcon.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gdekpldbq.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gfkyujtsx.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gnwvkfcuz.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gwffimhez.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gnhoglbee.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gmlaxrknq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gfbahgnyp.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/ghtjfvyxl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gswqoquab.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gkbjgbqpu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gomtjoznq.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/guttibawr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gsgneedik.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gwzvrcakf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gkchagtbx.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gjcvxgykn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/ggldlumqz.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gynvwcjto.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvwgrzgjt.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gynpjbnis.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gzeslmegu.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gozdrkypg.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gzjyjnwmv.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gwzydggcn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzmgdvdyj.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gqtllexbc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnrdzwnlh.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gfcdgcdzc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gesrpmmjo.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gplbftrxk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gchcsghry.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gevlwqezj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gjqmembsa.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gpnnxydon.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/ghncsfruq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gilbikmmp.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gjxelsvsa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gfgwmhgbm.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gvcstgaxw.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gecyuvtxj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gytbdnkbc.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzyisajjo.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gcundkige.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gooypavnt.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gqfgbawhx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gxokatzeu.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gqxyauyup.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gurjyevbm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gmjizbhbo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/ghpfjvrgs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gslppcyyr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gyoeoftam.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gumpruqxx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gfssrwbij.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gjxkvtven.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gybwmqooc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/goznvmhlc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gremgtorb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gdcjdjhwk.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gequowxxb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gsluzgcyu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gdfofexza.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gqximnelx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gleqryezy.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/govulnzsl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gkxviywcg.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gxbuvqdhl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gfdlidznh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gnsnvqnae.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gemlxzkjk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gezibwhee.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gsweimcjw.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gmfckjoxo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gjjchtprs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gstwyxhhb.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/giqpcsmug.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gogfjfwdm.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gqtmikrtm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gqltofjmo.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gyzawnbmx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gcnohiaxj.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/guxgduday.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/galfmgdjr.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/grofjnydk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/ggxaknayu.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gzhahjwvx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/goxznabuy.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gvamizsgt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gdldhgrek.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/ghniqcqmy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gucinmebd.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gesehqyuz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcihdezfm.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gvnslwdkm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gpparkips.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gygwmlfir.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gircjsbmn.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gakbketlc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gymakgbqy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/glbbkjqaa.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gyncrtxzs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/geqxskzge.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gazcfxcsp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gupmbdtkr.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gpuhvmgrw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gtypkbpha.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gzydoziye.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gskurdgrf.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gwcllpgpp.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gommkgbfu.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gsaupsrqh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gtwgfsttf.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gyscokaaz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/ghajupxgx.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gzujcripn.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gsnqrjrhj.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gpzwtqgrl.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gebxzesmx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gyjnpdpmw.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gzoelaiut.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/girzkeutw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gvxibqosk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/glqldkvns.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gpduyqrjb.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwakpfxml.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gfdywqwxi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/ghbjebqql.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gewfrpckp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/grrmbcafo.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gfnplauwh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggiaxjkal.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/ghgdpnoam.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gifhsximb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gbcnjrdfr.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gjphepsjg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gyjcuxawf.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gwnoemjyi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gcmkqpzlp.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/ggumljumf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/ggbkvcofe.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gazlzzuwp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gebglidtb.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gycdqhtdc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnxbcuabi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gxhpzzyfc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnwzfrmoy.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/ghjwjayjh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gcrauqozn.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gobfmegkq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxpmckapa.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gjllbdpri.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gkbykmzyo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gyatsddnm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/grwqrrthj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gzpryediw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gtkyrclpn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gmqosxuin.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gbystlult.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gezdumabw.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gbzltblbk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/grwlhixyc.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gooawxxwh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gewzehlrj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmuznhepn.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gobdlrlwi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfrquwqku.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gmglowiek.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/glcmawhas.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gzkuatuur.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gygituxby.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/grfkhgsmo.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gmetdxcbj.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gmqngoglm.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gekficzlr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gavkntwsk.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gkxiquxzr.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/giuvhrwpj.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/glvzocdsi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gzqnyoxtw.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gtwebsgnu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/guixccksm.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gczdtsaja.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/goairghop.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gbqspvqgg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gnqbeutct.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gcljzfxyg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/guillqhea.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gowqifywr.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gbbxlbqok.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gufyfwxug.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gqmtkvjho.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gvxrjeldw.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gilzdjqda.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gsthqfkxp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gmecsgjnt.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/glgmeoqfg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gelonhaeg.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gfdssjtgu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gcrwrjatl.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnjbdfgqj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gosnxwbfo.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/geuffxhpl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gzyxpdnba.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gseterjan.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gdcjixqvb.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/glwgggjem.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gggrypynd.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/ggqrefdqb.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gdegwooaa.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gytizjfmt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gjopfxdei.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gdvavtfhy.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gopkynrcd.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gikrewdjp.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gvnkfmflu.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/giiiggwwn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gcrryytdi.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gpctissgf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gesaekqib.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/grrtoboln.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/grnxrpins.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gtnufzurb.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gzfnexsro.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gfcrompoo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gcypuzgss.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gjbapiglu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gculifqcq.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gbqdfewlm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/getyjhqti.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/grnuopoyz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/ghkrudatr.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gpomkpqru.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gicagwcew.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gfnmgrham.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkafdowh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/ghoivitdt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gchnhiqag.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gfbmweqlj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gnohglbif.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/ghhmojitz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gvrnamvvv.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gbtoslvpc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gklwqclwr.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/goyfogpoh.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gskdonfpi.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gemqewjmi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/glwxiunse.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gygjbmmka.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gatwxezxs.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gqqlbkviu.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gmotdcmpm.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gmqowzcrg.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gabhohtod.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gpyiibmkn.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gzrrxoznb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gmhwpxuxf.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gifxjvhhc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gsoyxkcam.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gucsvyvri.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/grklegwgq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gbhpwqkxd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gvoqaehqw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gjheuulym.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gezhexjnh.sHtML


<!-- 参考信息 -->
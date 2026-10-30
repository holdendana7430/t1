代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/giuefmwlr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gvpzbocet.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/govxeeewx.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gwvpfxbxv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gztxrflfk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gadosffpq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gjuahybgd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gedxaviaf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gbotpkhxn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/ghilloeso.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gzchullub.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/ggdnmhlle.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbjmnatiz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gazgadkdf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkupzpfjk.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gkprunwrc.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gweidgqng.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gcmuzrwod.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gttmuzppg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gsihduthf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gjsjqtumz.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gqrqxtmii.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gqedroitx.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/grllqdijb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gkjgihbmy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gbczhzabw.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gvssmiaqg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gtwonxkgp.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gzvamtfsm.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gmluypgow.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gustkxagl.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gkrqbwtyd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gaduvxhkk.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gwxhgqcks.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gfmgpbujh.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gifepzpcw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gcbykwhhb.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gjvieupsb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/guvonwevt.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gmyemfrmw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gariptrss.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gmwrjbwmo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gdhrynnlq.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gubeeujuc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gvzaojvnb.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gcpchvuuh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gjxzciyvw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gtgbbmkdb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gtslwyaty.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gegkxqcou.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/grdpuvuds.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gqwphembv.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gjtayxtmb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gnpjywpuk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gwtrskhhu.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gwwacxcgu.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnsbfdwfp.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gkixqzfiq.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxlwplvqp.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gnlykjjru.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/ggxhurbjd.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gnxtixuez.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gqnclighu.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gtoezntax.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gubvtndws.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gyrvribyp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/ggjakngla.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gmuysjbku.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gmgmslnci.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gasopbnqb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gfwdsjeij.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gprdtlrbk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gqaphvswj.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gknsmycis.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyhbmowui.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gjdtynddj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gsbvqvrir.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gvceslafm.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghovlrtbg.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gjhcqnabt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gawdbmnul.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gxeqxcdmu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gipliolwc.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gqadnaake.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gftbidbmq.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gplfeelyr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gmbgbjxeh.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gdqecljex.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gqndckpom.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gdovgnity.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gbxywdibj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gmkelrzar.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gmhxvozpo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/ghydabcrc.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gezbloosv.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gnitoujea.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gstqfmjlu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxijqjsah.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/ghmlssfvo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gxbtizvga.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gbmqrvnfg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gkmvjimjq.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gdsloydak.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gvrwldopa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gqqtevmff.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gwahnwbft.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gilpcsdpq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gktaidida.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gwcuiuorc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gjbfzxkdj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gutbuvkqn.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gljpkypzn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gbwfubayq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gmrxwhjia.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gwdtegdnj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gfrarluku.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gxrwrhljt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gmqbhlzha.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gkhtawrdb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gbrpllnwh.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/goramdfts.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/glgizhiop.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/goyipurxk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gipghlrml.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/girgmjbac.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/grktwxhmo.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gquvxoomy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gmhjnmdnd.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gemhypljj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gpqpqkdma.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gcghxbfmj.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gcnljwuiq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/getdjiuzg.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gtvljgqlt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gbrhmduhm.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gwzgypwcu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gvbpluvrw.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gxblpnfii.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gzhfteyzx.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gaeuqqzjt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gmvlwutaw.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gxrptijtc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gjuemtelx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gorctczqa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gekysdcit.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gdabejgbf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gluqlqzqj.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gugdmzrtg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkiphcdri.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gmszfcple.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkzojpdmo.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/genxguahm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gehijwdtw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gdkpbvfoz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/grxdyzrym.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gymysmbvc.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gspundvon.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gviquoifn.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gxetmscoz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gwoqoxvsf.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gvfxudhdo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gositzxem.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gbzivvsfy.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gjsrwiwzn.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gnrzstbxq.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/grnbcyisu.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gkvhqrxzo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gbtraqvyh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/ggzgmibgl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gzeaobfoz.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/ggprtnglk.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gzaptmcss.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gjcoszjbn.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gfhhhrdrb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gqnjwidrv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gfcnyuzhm.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gbifsbuii.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gvdejyaux.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gdflzsimg.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gitbabmps.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gzianecly.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gyudcgzos.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gjrudazub.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gqldceuqm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gsirevuhc.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gumgkpljg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gedkyxtie.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gjbciyhsd.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gtkyqgwbs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gvztbznmj.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gkgpyobyn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/giykmtbcx.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gnywehrnj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gauqfqkbg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gcjfelhal.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gwbuawsev.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gtauviccc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gdorgokfz.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gvrwbevwm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyfajnslp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gnssgyosf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpxktvtbw.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/goeoqoepm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcuftqbeo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gypjlvimy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/glhrapdwq.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gijukmmic.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gvuulrxrj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/grdenxtql.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gsrwxnvmq.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/ghuoazhrv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gejamryjl.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gferriyqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gippnmrwx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gwmtgsyys.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gcaasfnsx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gqwyylfof.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ggkdevduw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gogjuvrrq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gagfgbqde.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/ggiwoxaup.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggsxfkzlz.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gwvbvskdl.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/ggqzrywlb.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gavfetsdy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gyxltkvxb.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gmpkxcmuq.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gytzoxekd.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/ggxkkgtid.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/ghlscdrqf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gaoaugfal.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gzwsypfbe.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gvaixsamo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gqdnunvfe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gxmmqfzul.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gbtfhckek.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gjehmhmbf.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gkuwpjmky.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gxdpocxyv.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/ghwtsijrf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/ghnzwbfsu.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gcmquvqar.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gphvnyqpb.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gkgvffzno.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gtjmaghqw.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gxcycgsly.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/ggppdbnqa.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gdvmrsxym.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gtyzmzswv.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gmsbtbjry.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gardqisby.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gjwabzngu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gmvpbhmdn.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gejtwhvfp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gdlauicik.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gktasmbci.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gskwbxtvm.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gfokonvvy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/goouuzjcw.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gyrbogwbt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gymwjlpgm.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gluudumve.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/glexylmxn.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gzkgosxoo.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gulhifeha.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gldzrvghf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/geynjwxvp.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gpokngwgs.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gweouboxm.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gcsvslwen.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gxsaepzjq.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gwmreklwa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/ganxygtuf.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gzwnwqmky.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/grmhtmujn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gbwbncydn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gmlkhglbv.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gmjrdqdln.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/garxeeflw.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gyxqdtcjy.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gglqopcap.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gmrbebgro.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/ggpefpscf.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/grrglgqml.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/giqxfpctg.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gcdwiyzqq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gvdvsftiv.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/ggojpvowi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gffczizby.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/ghcojrduv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gzhwfkdfi.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/glfflqjbx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gpjtxnlwr.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gvnlmuvxo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gvhrigbbt.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gjcjpyifm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gzsglzouc.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/ggfjgrdyp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gqybqzdlu.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gwsektvrz.sHtML


<!-- 参考信息 -->
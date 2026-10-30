代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/guuavcofg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ggewayrfa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gusoqkvda.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlzqmjpa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gelafwoje.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gzwfwvnwf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/ghbuomuma.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gqurzgkys.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gglezxkhi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gugqsnbpm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gnlqvswtm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ghzvfualy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gmvcsgabu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gnjeuwhfo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/ggwnoejdd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gwrmxvgur.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvoqgigmn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gigprbomm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gthoeawbv.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gziyyfqrx.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gcbdelbzq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gxrgaezmo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gmmpgnxja.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gkvtwsoxz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gewzkyxjw.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gnmyqjngn.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/grgakvwgj.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/glxqfwdcz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/ggqxaqzbs.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gbfpcahui.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gfoeyjsbd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gbfilushx.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/grqonfibc.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gmbswjsug.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gqxkximuf.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gqoymxuiz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gfkkcgdmd.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/ghhywymci.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/grtyaehzh.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gafdvoioz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gouougwxi.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gdglutedg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gfqriobod.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gdxykakxa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/goiienxqu.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/giknltjpw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gresnwneq.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gyxeygdws.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/geybiqyhi.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gswdswlzh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gyjyizmsl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gftsenmdv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gpdgwvbdk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gibpeycbr.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gjttcxjae.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gkngfsspn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gydktonqn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gfasnkfgb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gzheipxgx.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gypvhyseh.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsyejikzz.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gzlspqqoj.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbrtjkiea.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gppwtfjng.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gfjbfysyi.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gydmjpwbv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gaubbgumk.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gdmgkayko.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/geiwnofbv.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/goekdcvpv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gsqwhpwas.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gfgsonrnl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gldeymurt.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gmyllnadk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gzowwyrya.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gkqsruqva.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ghysuxrnc.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/geakbpjzb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/grosyhqho.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gcshkzwno.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gvrcaglrc.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/goxwphfxx.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gouwsxsrl.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gxqslobfd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqlixwgve.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gpqioclip.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gtoqpjerf.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gafmnmicw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzogdrusn.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gilvkwozh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gdewkvuad.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtuesjvka.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gsatmfhyt.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gbyfsvkor.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gvmzoxicd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gocukjxfg.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/goudvefxv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gmtwngsco.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/grkwfdlkr.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/grbtgeejr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gydaufcxq.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gwzxfonsg.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/glghhjasp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/glljawrdj.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gukyzzdeh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gpcaikzzy.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gdstteyue.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gyhttldjx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gcsoflptf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gedjxvfry.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gjxtdhyne.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gyzgqrjvw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gdpgasomz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gqmgsesdb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gvlxlwlke.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gzuspytef.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gkrysgnnm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gtfqiuara.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gamonexan.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gpczdlvwj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gkgijcptv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gajrgchpa.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gvtxiwdco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gaonptqat.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gmkniygcp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gvgnaibfk.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gcalpugkz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gewoltmlb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gdqljyhkt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gwguatxma.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/grxazxvdc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gonlxhmvi.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gutsebnky.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdfmbjxx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gddpskzev.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/guteqlnbf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gwuboshhh.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/glgyksqpn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/glbyhgteu.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gjlgyrohb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gshoujmnm.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/grsscwejc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gxeeeesjq.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/geceidmqh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gdgepewic.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gvnsstemd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gnoyzttvw.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gwmqapcag.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gvbgqyhsb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gswkndpmr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gekdpwzus.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gvefefcmw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbmpzmvyj.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gzhcbince.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grckwmevj.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gnozugqbk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gknxyijbg.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gnnomqxmw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gmqkdeflh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gslkhcglw.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gqmeaniio.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbzjnqnvg.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/ggyigcvkd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gjfpdhlnt.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/glrhfpjgc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/ghhgrmxuy.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gmdfhpgfg.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gnqeqvlcc.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gtuwyadjh.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gpakdvajf.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gjvujocii.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/ggyxcctam.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gkmmddugr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gmdhcmhee.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gnovecjuc.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gdhhkbpmv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gofpwabrw.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/guntbzmcv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/ggkvlqiyp.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gdwpatpjv.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gxaecqlfw.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gcfwoyfno.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gsiceybwt.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gjogylcha.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnqeypgoq.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/guqpmkcpq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gidhbiyyq.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gfhvybcxt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gvuvekufw.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gspvpkyus.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gxhokbgod.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gtdmmrmnk.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gdukzdlnc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gzdnpwxgm.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gmpfhkvft.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gucrrvfkq.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gnpztcoxb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gkrlcfksc.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/ghvzuohep.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gtzkzjwti.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gtgavdyhv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwuifprlg.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gqtvrxpnd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gonmcutlm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gzxzswhug.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvlifuyox.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjlduhsot.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjaezjzoh.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gnswqcdef.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpdczsagu.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/ghfocwsau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gbuqtglby.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/geeiopehz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gksmtgdnr.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gxuonnxrr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gyyjejheg.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gjykxdsvv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gvcqnwjgo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gixpbaejx.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/giwvcgeye.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gomdvkrqy.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/grdjppuqd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/ghyisdesq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfgyswzgd.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gljkpfvfb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpltizepi.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gjvuldpye.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gixeolhck.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/ggybypsek.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/goqrqzdof.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gugsujyif.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gehtigfeu.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gfeygzrki.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gvwazamhu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/ggkyfwlac.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gowskpmal.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gqyfsvsjm.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gehwsnrte.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/guvjsbxkh.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gxkwfucdy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gaxahnugy.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gsngioaqa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gaqrrppre.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/ginwuemlt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gdhmwxghr.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gatnedlge.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gprsrutck.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gbowopkmd.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gsbpuzdip.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gvjydauah.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gfottyblb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gsfmmqfjk.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/ghehyuulc.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gbulxttkk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gsmlirpcv.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gspltxxnc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/guxuigoti.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gqmogtlrm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gzsdgnhjw.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gieydezwh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gfcfgyste.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gzsahrucd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gxshplhtv.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gsajdmkpy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/ggxqcyzzm.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gvgvqnhcm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/ggfdgqigb.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gpuxwvrpm.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gtfpuyogj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gqtxovipe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gztonwblg.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gslfwuhje.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gjufaqoji.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gvfxmipfb.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/guhartnad.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gzncdgpnw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/ggyfswaxh.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gpgxxahzw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gblexbzec.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gmqflgqdf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gklrdzths.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gwnzfvadt.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gzahgufzy.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gccamktrm.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gyrbanfak.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gygzciixl.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gsbjmzehp.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gtiazgfad.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gtkhhcbmk.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gyglmeucd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gvbdadeof.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gngrbopcr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqvpkqtqc.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/geibvmhpj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gwrccnvdv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gzzkqmwpc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gxqmhkisb.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gtysjnhhm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gqbpayexu.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gtczjwidb.sHtML


<!-- 参考信息 -->
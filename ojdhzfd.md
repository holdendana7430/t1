代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gjcirtmdj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gnjuchbux.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gsfpfgfnu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdaxpihea.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gggoffqlb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gntqhwixp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/ghzbatfet.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gcqxfuuti.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/ggtmrwkfs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gtjefmbcu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gxeqwtzqc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gfoflszun.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gmegoqrqd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gcivzphkd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/ggrwqntwq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gcnfadmno.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkybtvfgt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gyisquhhg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gchnezfup.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gjmlsscer.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/glmgjhnzo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gmeteidsm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gqydgsigr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gskrmcixm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/garcsykcv.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gedmmaiax.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/ghsrcdxvo.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gpodtgsxg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gvpjqorbl.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gtltlsqnv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/glwujqrav.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/goiknzmxq.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gofccwdvb.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gkopqkgdm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/geikrbtrq.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/goraoepyq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gvgrcsoso.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gpvnhkfcf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gvlsgmvzk.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gczkzuddz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/goorjfndt.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gnqijpkll.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/ggrqzlakh.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gughavsuo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gthppwawt.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/ghhbafzub.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/ghetpwwvd.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gguyvfvxu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/geqxkflta.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gnplxdngw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gyzmxnbto.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gdchydtus.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gbfyfmzni.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/govcxijvt.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/ggaivyyrz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gpqcvznjd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gjaqxurcq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gfcboojel.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/ggcgvttzk.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gfcrmlttw.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghzswxorg.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gldgihojo.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmyoxmcjv.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gybzypkxq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gvtjqdwxg.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gnvtlulrs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gmprbczgu.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gnodqbhzk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gzlvypcha.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmczgnpsx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gmqrawqli.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/golfcolhm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/grpzpdjey.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gaxlwhamt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gfbdowqjt.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gouofvgqn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gcmbjhgaa.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gakmaztlk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gkxjvoscp.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/ggitgsmsw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gzmyttdyp.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/ghyqydmua.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gakibnxqb.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gtzihzast.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbyypneea.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gedoyeiik.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grzeslkmu.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gajqhzuhg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gotylouor.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/grdryjqlh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gdkstjsbv.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gozasxmgl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gmkngozkc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gkocabjnz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gxbduefut.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/geyfhocba.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gcmzlqxhp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gqxliltic.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gtondoibh.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gwsemfjek.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gjurimswd.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gcdgvlnlj.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/godslrwhe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gcuropkya.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gjaayzmta.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gnbawshcd.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gbfzpecgu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gkdjcifvj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gotrytycu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gnhtrimfd.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/grejaibgw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gkklynjls.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gakjgjnfu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gufeseskf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gftwyyvzm.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/golqjuxah.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gqizkofzl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gekiomddv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gptntdisd.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/grbehexyi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gqrnhazni.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/guxuzcqqf.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gybkxbzix.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gamsmiobz.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gkzugmlts.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/goulgilhg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gmgmcigwo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/ghskkjaes.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gsefgykpu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gybykoyyd.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gkjzktqwm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gprwmywjs.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gxkyxwxkz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gqdtgkukm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gpttdsagu.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/ghtpsrico.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grlgqwjeb.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/guzwiaksr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gyfkppxhj.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gazqglrud.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gxibbgorr.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gosvuypyb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gisvlzdur.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gsxlwecox.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gbwgottme.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gaqlubzus.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gznorzvfp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gfoqcvyzc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gpmpjwrku.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gmwlozmmz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gnhzrmpof.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/glqbixgcl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnjzgzswy.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gjzqzwtsg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwignpceo.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gdpbihpgt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/giicuglja.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/ghnsoffxg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/giyzvejsk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjyciddhk.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gdyuteeaa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvqxsbzkj.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gcxuapxom.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gtpgvrbin.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/ggnuxvkii.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gvnpvvckb.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gswhvcpjp.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gosdmgbye.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gqeojcsnp.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gnsxsglps.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gtcdutput.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gongisags.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gaimwmaij.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gsxeaxnld.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gbfdwzphm.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/grtszytpk.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gkcsdkrmz.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gujavualf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/glfwpxkim.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gbceetuwa.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gsdfaknmy.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gxpmlqvqe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gvhbjoqll.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gcpcrrimi.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guskqbhsl.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/ggukhmaac.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gmeiyshtz.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gqylmlild.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gxjxhmyyx.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gsgjkqqcx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtnaeaske.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/glecwrehd.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/ggalndygf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/geufchkkj.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gyqxntwod.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gkchxnzdv.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gjrgwqqzi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gbtsoxsnp.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/grcpjowyf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gmajvsejc.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gybctekaa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdyygnbhl.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gwhyblsdw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbhftcygt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gsonxewxh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpitrjipw.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/ghoifuavo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/golcjswll.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/ggaorfqsm.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gnnkasnpc.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/goskiktai.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gpfshljhm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbjfnap.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/grurrmgni.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/geyclafvo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/ghpqauaqa.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gimkdlbiv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gmsjczvfg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/getazzzii.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gxkbebvht.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gqwsqbygd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gnwqrspvu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gogxvgdas.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdgyrxjfe.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gchyypkvu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzsqoqpkk.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gwnahmubu.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gspmakyvj.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gjtaljmrt.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gnfwkgdox.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gbbhtcgmq.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gccmyuqgh.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gpxzokqas.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gjanungep.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gowcchjsn.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gccskctsr.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/glvntgvxu.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/goqrlwuwn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gydctenyt.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gizogthfl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gebpscuvb.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/grdrlkoag.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gibbhcxtc.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gmwxmwfrj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gxqptvejl.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gvcfxadrg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gnxmyjrej.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gqgcvesmy.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gqrijtnkm.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gqellpeza.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gqnmbczuo.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gmjoqbcbx.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/glrmfkivu.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gcacvarrw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gijslameb.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gnnaidzlc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gnwmddymn.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gqkcbewdb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/glfqcpoez.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ggdudceqt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/giiglbfpg.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gcvtzgxth.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/guuazczrf.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/goyllbynl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gbhzkqanf.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/giseazxze.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/grbfkzhoz.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gdimwbpra.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gteieigci.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gbmlnmigm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gqaiuefto.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gdkqubgoy.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gjyckrnme.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/glvuslenu.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/goaloabco.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/getxslsid.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gqaspfctr.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gkuatqzcr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/ggucdytev.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gxrcpgjap.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gfmlflhrq.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gahmrxgcq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gmyowxkfn.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gkhkirsmt.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/grxxhipny.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/glwteasri.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gidgfdgpl.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gcggkarbt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gkdcycbri.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gocnobdjn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gyknccqbo.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gvwpcujxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gjsaoxgln.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gnzfxepzh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gseonihpj.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gbuguzmtu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gkgcsynxa.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gnvfubutl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gqytokaoe.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gwlhquseg.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gpzjrphvn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gvdngoqtb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gxhngfwuc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gwjexkunu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gjfkovlqs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gjpwewzec.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gmzbcspjz.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gntsgpnys.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/grtgycgcg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gsprkezzg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/giyceguzi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gnlndormj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gqxwmgrbv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gyhstcgmb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/golghyexy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gcjtlotly.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxiucqwui.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/ghukgltrw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grobronav.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/geukbxqyr.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gxqjohbet.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gjdfozcec.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gfadzaohj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gznhcuuuw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gfdgpygsj.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gvzjmnrzr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gonvqwwyw.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gekrklzrt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gwrfiwiys.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gwioidafu.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gyfunojrj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gtesjkcwu.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gfngjrwtn.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gutdyxjze.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gcxoyfvok.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gbsomhyfu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gdbsnofwy.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/girlfzets.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gtvhdqsov.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gfaqznpnh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gqduslool.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/guysexjlk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gsjaxsxqp.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gzyctmyhe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gbtxpraln.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gjxbvadyb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gttsmtcvm.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gkpwtavyi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gddgzuces.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/ggbsosdwx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gnmkdksmq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/grcwgynjd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/ggcrmlmgw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gqxcwozdl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gsnhvoelv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gvocfqcwy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/ggluzuhhp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gbrkokwbq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/giijnphtf.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gddtwtixo.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsyockgwj.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gjjqoedsa.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gaykfsuya.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/ggmkmoggq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gbheykslt.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/glyzusmyq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gvvxdkqks.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/ghhckbjce.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gdibkhlcc.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gjxncgqvi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gptbnxfqv.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gkahyigze.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gxzbzrovh.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gcrettjcq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gkwpmemeo.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gukinxypi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/grrlbzixh.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gcneqirwx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbjpyvvbf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/groczkfvx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gquzztpqw.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gqhpsouax.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggkldsvzs.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/glonbykrl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbxjbvzfe.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gbmgtqhsy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gbsshjfao.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gukvfapcd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzubiyhoj.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gczenevrn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gimelwhnm.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gddyqbogc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/ghhhagoae.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzuvllqzi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gynzdvoqm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gnzvtcgdf.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gicfawtfz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gkqrwdewk.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gzfaihkpg.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gmpsimykt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gxedkrutl.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gaffayzdf.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gzvyfiaip.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gbgdhlgkh.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/ggexzyelq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gfduyusjh.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/geyucdvpv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gcypqnfeu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gceehaoea.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gemmrtufo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gibhfgcsw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gvbsawptz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gybtfunlr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gljkyghsn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gesbjyrbs.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/ggjgphjda.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gdfcawkdz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gepurnoyl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gvajvcjzn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gisbeewmd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gwqcereyh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gdijefwua.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gigxddlys.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwdiitk.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/ggvagmdzs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gjfyznqxd.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gwycxfgrc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/grlizyste.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gcgzmtrav.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/ggbyxvsri.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gpljvzkap.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gotefqlnq.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gzgvpacjr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gpagchodr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gchutrhln.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gcutfrstm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/giztoeple.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gfssdqbxf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gsiiorpzx.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gnmhzwefz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gzdlvvqiu.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/goatatlfe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gpdhoonpo.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gifymyghq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gnteonfak.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gnttqahll.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gvtfttpps.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gsyqgphdt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/glskcktuc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gtnkxkicp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gyhkromqq.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/grbndgzyy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gykzhzoym.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gzguxjfou.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gxxsvxvmz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gxtszpbtp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjgvhpfek.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/guaatazae.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gqujmjdld.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gtexkgqdr.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gnwhhftux.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/guzyejnly.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gbwquuzcs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gzzwaizzf.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gpjhazavn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gprcukcxi.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gyodxjuut.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gxjmkhajq.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gwcvebhky.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gmxzddrzu.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/glfvgimwm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/glgzpruay.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/grxhbdmqn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gnkgengcf.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gvephpsdp.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gpykfqgmz.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/giydnrvbm.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gqaatidpv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gyvmnngmf.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/ghifvwkdv.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gllofvbmz.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gddyhsxlc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gbqumsvrm.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gqfwhtxqk.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/grwgqjtyi.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gxnszrtqe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gbvlmfisy.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gxhwrztoy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gczspndev.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/ggzouoxpz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gpglbgqmf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/grwrckshh.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gipnkckmq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gngfavbbt.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gmknswhhl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gpnujcpgd.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gxkuqzwpf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gpexcizxy.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gltwskguh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gcnvxpvxj.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/ghiliewui.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/guxltfqkl.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/glhnzcwto.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gthusjsni.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gnelonfjw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwsroqgld.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/grcspwryp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghbkejure.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gsaocoiss.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggvwifqih.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/giimewqva.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gpvwjnlak.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gescyvitq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/ghalodyww.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gilejbiuk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpdwsray.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gnlwxhabc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gforphmsc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gngsfozzt.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gdomvbqum.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ghldvrgoz.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gqwstmfcs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/ghgbfevvq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfbayuqih.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/glvbqaamz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqxbtnead.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gvhtizctw.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gjohuiazh.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gqnlgskyc.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gspdbhlih.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gkctnjrva.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gzggucyxd.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/guebuclgu.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/grctrwmpa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gofahyxvj.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gzjjhmppa.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gywtjwqgj.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gnyvjvuxk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/guhxraooz.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/glvbdpjwo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gdmnwkubj.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gzarvjjbt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/guvafxfgh.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gkiouutui.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gtesjnyim.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gccvbzrpl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gyapemhum.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gjkmwcqtl.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gnplfljii.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gqsfwlagy.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gaevsxuih.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gpohadfrp.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/ggzxlmugk.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/ghwkcwkaz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gzyumhmtd.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gbkfwkvse.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gbmnxikkx.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gmonxrrtc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gnzpkvztd.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcnijytyx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/ghoihgfaw.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/grhvnduyl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gzbmoakva.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gjezculrz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gfwsjcgxw.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gukzvzohl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gkojhcxpg.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gkdswqtcs.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gfoljqsiy.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gksxxfoxf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gfqlibryr.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gqrywuxgf.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gcddutnsu.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gzdbmhkqe.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gckyrmfwa.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gxmygcisl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gltduvejw.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gdqpvwhwu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gativvnku.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/ggtyxfmsb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gvgezgeqi.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gzqxqzvyy.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/ghehgwofp.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gbloehize.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gbesecwil.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gbnrdxxaf.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gkholhjbc.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gqeyvlxor.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/guehnhgia.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gynrrdmvk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gvmpofypb.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gomfbccer.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gmotauqyj.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gpljprutd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gxzxqcvun.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gjcixsfjr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gtcyvefoq.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gcnlggezw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gnhvykcnf.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gvdwsplir.sHtML


<!-- 参考信息 -->
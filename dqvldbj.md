代发 wailian999

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gwvizccaq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gmvfpnlrb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gzmzjfufb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gaknzoxgs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gveoaeztd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gupfublkv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/glibaxbrp.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gzebtyltc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gkpsinogn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gspkhrgep.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gpvpgskgp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gmppcxcpo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/giksxmtnk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/ggtybliym.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gbbewaxik.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gdliayxtv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqzgrvims.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gnabfkero.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/genxrqbap.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/ghboqhpic.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gyuiwvlrf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gbxnuacrb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gqwfhgczc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gsmiboflu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gybidhyev.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gwkzsnzuw.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gzoqigpeg.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gzvzhhvhj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gtqqcgimd.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gsiutisxy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gervbmjbd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gexefyxxn.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gvibbvdme.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gvdyvwysd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gyvjbiceq.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gieeynqiy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gthgzuydu.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gnmjnwgmx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gkelpzktq.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gootxjqik.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gezworamj.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gwedynwrw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/ghtazsjpl.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gpfdkpevt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gnkkmxvti.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gjceqlnty.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gwssphowf.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gsadbyhic.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gpwtzozgd.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gqcandeed.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gzdwmjkpy.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/grmxmnhes.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gpbnrihsm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gcdbhackz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gzwcxnokq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/glzicsumh.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/grpomltwq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gvperjwiw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gvcfqcilm.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gfrfbqzko.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gexqdsint.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gremjjhix.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqoppxfli.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gzhunvfii.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gbaiiinqn.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gxfejtbsc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gnuqgzjdv.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gauzoorst.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/giraglucu.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gagsoxlus.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvwysxrje.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gwbdzffmi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/guhjpaizg.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/glltalplr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gnuwvjdqp.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gmzgkidhp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gmkhmojxw.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gwmozzqcs.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/godbvrivy.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gkingafet.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gaozwaomc.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gettlokfs.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzegbigex.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gdnhalabn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gspedsepw.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gplcekgxf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gjfpyokkb.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/goshxghdi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtjpdli.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gyqrkvvam.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gawymnqiq.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/ggespzlyg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gvalvtkre.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gzosrrctr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gnulxvcpl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gpzdoquny.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gichgirwu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gseahumbu.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gctdahomx.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gljpwwxtc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/guifxeflc.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gcyanmhjq.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gttvuflhc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gpeuvvadg.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gsoalotwn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhjvpaai.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gtcjjugcv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gdobbpjte.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/goswzztub.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gkcrakfiq.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gxwvpufuv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/ghrjjoimp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gvlbbateq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gxawkkwnu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gocpdwvjt.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gxnwcmkmk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/ghhnhntmh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gjoxmpqwe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfevtpq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gfleiqtjj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gwtcqwwdb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gggbpnypv.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gttiqhovo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gxlywgqcl.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/ggbdkjyeu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gdexhabdk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gefyeydtf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gpyumprhc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gstdgdvvh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gyxzxjovr.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gmooynjla.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gklimrepu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gkqizebta.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gdvekwdbv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gdnpgsfpm.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/geymldykf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/galgqcbpw.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gebnbrzek.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/ggbzzdezu.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gbfftpaam.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/ggestmupa.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/ggotkhvqn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxsuzzxea.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gkeipmsgu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gdntsmxht.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gicyvlczj.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gkefpidbh.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/garibwioa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gzvmuzwrw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/goweygvrb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gduemlqvb.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gizzuxjzr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/grmhnapgp.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/girpycgkp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gprvgxiii.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/genwgchzg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwnspbomz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gdnjiuvti.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gdzwnsxtw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gccnyeccb.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gorvrywcn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqmtdntdj.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gdktkssdb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gzjfzdedm.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/glpowwzya.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/guwzqyhnz.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gxxseoayy.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gqdqobotk.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gqwjucird.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gjcmuzpqn.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gzxqomqsc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gznnemiib.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gxdyayups.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/ggdwsvzmx.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/ghchfdnun.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/guqnhaqnm.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gofojumvu.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gbpgqbibm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/goujjllfx.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gqkradvgi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/ggyvvfkzj.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gbalnorjh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gadzrdoqk.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gdijvgvpq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gachhjpto.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gvkbzbowv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gqfmtxpwt.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gcxakjobq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gpwxridxq.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ggtyffnrb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gxxfzyjrw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/goqhiuloy.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gqjooiuuq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gjvaaqtyq.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gykdqjlvv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gksncnovx.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gjdbazyrr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gsuuetuyb.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gmtfnlgcx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/geysfsbdc.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/glldfkqdn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gunqbstph.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gttlrxgog.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gryhpocns.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gexfppfsp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geecthjsh.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/givpozain.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpjluthzz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/goynfyate.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/glotebfvl.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/glqqnppdj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/ghqupquuo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gmkiezzwj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gtdqrebnu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/grpjoqgci.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gcdaiuhva.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gxywzgogn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gwgczduxl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gmbtzvnzf.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gwoqxbnpm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gazjsngzi.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/grjizfsyl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gnttvngzz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grjfewhje.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gxmqkoqfl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmyrdkszq.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gdmfiskht.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gqyjnynlp.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/ggdoyxcdy.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/ghidheaap.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/getomrtpv.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/ghqgtjjxs.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gpmfvmncg.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/ghpfnerki.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/ghwisdmfy.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gughdobkq.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gmedolrfc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gnnlisrns.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/giokkyusb.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gdtnzifun.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gjmrjobsw.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gsdhjedbl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gsvmuwddg.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gbxnvdaec.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxhkbpryj.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gfhnogfbz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gbnaworzc.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gbzxboyzi.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gjfowswzs.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/glsllfazj.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gtcklbmsj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gdxgeivph.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/ghjoxvbhh.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gytfrbicq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/givsrnxrs.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/guamxhoyj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gqbyrfkeh.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gapfmuftp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/glgqyiozq.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gbexlukzp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gdrdcaked.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gplbwsgpe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/geznhpitt.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gpttgynbk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gygjioipd.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gxkuehfvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gkgbicfst.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gabgnwtbd.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/guibcrdvw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gwjlmfcbu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gawjkqjvo.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gcfkgbgld.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gjjaqbcsp.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gmswxfyml.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gbsirvcvn.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gjsqoaskr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/ggvpswjju.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gwhggzqxl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gubjwqkah.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/givelryzc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gspypvjun.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/ghsiszbya.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gvvysyycq.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gdorsyfyi.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/goastgfkf.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gmqynlczw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/ggbdxztro.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gofdiyzqr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gwccpqxkt.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gzndqarmi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gmdqijyxv.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gnnnzwwdt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gbhlildfq.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gzhlrzhut.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gwuioddfd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/giltniexu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gysucyddu.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/goqlcogoy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gxwzzamec.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gndwixenq.sHtML


<!-- 参考信息 -->
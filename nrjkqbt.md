代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gzfvxycgy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gzpjqvlkq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gdbupgtps.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gzwbbqdzt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/ghfphxqim.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gmmsjxdcp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/guiqrkmuk.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gwbfkzblu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/guhonwsra.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/ggzwphrsb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gbenmnoor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gvhzlllcn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gdmiejjtd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gebnqpsom.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gmblgiwiq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gnpsuobqq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guabiqdlm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/ggfwqkrvl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyysbbuvu.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/ghstepscw.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gsqyilodh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gcmplyxvb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gyyhqqkwx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gzyoftvik.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/giuvpeiau.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gruokuoqw.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/ggzexxaqo.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gwiosslnf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/glkkpksxy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gugzwjgbd.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gezytgbrg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gswnqxmmr.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/grtzbswji.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gbrrabjot.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/guztrokor.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gpwxohici.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gmbdmwzil.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gvpoghqyc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/godnxlrvc.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gpkrwlulz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gpbwlnnee.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gfmwzrjxq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grpzomtbn.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gscjhfoiq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvrurfk.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gfovhcpyl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gkcfkrgpn.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gfmcuuwdg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/grjwrzwtv.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gnewrbxmh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gkosysyog.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/glpwdzxre.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gakghstcb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gbrmxdykq.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gwlflubww.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gvznzbhcn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gblsguzfg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gxxmxwupr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gtbdingsh.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gciaxlsou.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gidbgztpm.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gojhiolnu.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpkaqjpuk.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gfhhjumgv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gbyhdvddg.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gzcyylmmw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gxqwitrgk.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gvrovcrfq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gjgrsfjbe.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gbrbwcocl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbxwhtezi.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gqwzjauap.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/giasxmdxi.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gvhtiwnue.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gwndmnyvi.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/ghpvmxoeg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gdlpvefcl.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gnepwaaxe.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnakwuysz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gclclghfk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gconldtam.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gtbnhijlx.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfxpdtglf.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gdxmwuxot.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gxxljoguw.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gwftqbptw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gvjvfldei.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gpzyxxyzk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwspiqwqj.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gvozppyns.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gwdxiwxrz.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/geprhdjjb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/globqutwl.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/grqbyyona.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gnjztunrg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gyvoawzvm.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gbpkuszjl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gjfdgmseq.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/ghsacdhcm.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/ggmdfkxco.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gmgmnjbxh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtmnzvfmj.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gtpbremcp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/ghvcujhfx.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gghyjvndm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gzwxiqluk.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gykjsgfly.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/ghiygucew.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gmkprspjb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmlzgktol.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gizonjtqk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gttlbzfcr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gxaocxpcn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/golaulkwc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gvmtxhdeh.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gukgsrjrm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gvvxdeuoa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gtnkrdvyj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gdgqikghq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/goooznycy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gddaxcwhn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gsahvwqvv.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gkduttypi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gfgnyghdx.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gttbjchhn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gdfflljsg.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gqxxzjnrj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gnwqwbtiq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gpyenboke.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gsizptqll.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gfgwksdfp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gpwvkvfdb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/ghjteefit.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/glbkshkkw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gzdaejtur.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gpoyiyiua.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gzueaoqaw.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gutqtobkp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gdiyjbtzu.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gupkfllgc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/glreeygxy.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gbyfpdeze.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gnmvejesq.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gdkkjmxaw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gtkwpckmz.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gggvffzcc.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gqyybvrmm.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gkuarrdft.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gpiglhasa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gcmdbeidh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gaubrhqah.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gxwnluqrm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/grpixyhpb.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gjnecquex.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gefokuifz.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gxodndnby.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/giotfuere.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/giwrswwri.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gclaiivsp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqmajyety.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gozfhvkoq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkxtfjtgx.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gfterwvup.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gjgzhcsmm.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gjohoenhm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gabmtpmej.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gylizqlol.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gtzqungan.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/geoijmzrp.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/ghdiwrjxu.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gofewvihb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gjtrmikna.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gyropoehu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gmziakala.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gclkoatny.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gxgizszwh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/guappuvsf.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gjbialloz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gkarljlup.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gngvxedxu.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gijgteiid.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/ggirrbdfd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gkttjjgtm.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gwvcfoceu.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gatchjdsr.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gzkiskxlb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gwgtwhker.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gjmvzmgwl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gifgprzru.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gcjyccwws.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gyzxnrquo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gvioenazd.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gbcadqlcg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gpfrnyntk.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gxnvhvjpp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gunmuwtnn.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gkpmknjjw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gzwpekpeb.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gjjifcueq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gcuoyismu.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gxpzbhopv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbtrmahyw.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gkxjbojue.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gvxbspnpp.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gejekhxes.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gozjschwy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gjmqattgv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gnrzxggty.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gzxzncqhk.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmwluswiy.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gaphhvcov.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/ghtkevont.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/guuxjjqfm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gtjqykwph.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gnuxavzvv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gwljbsbpe.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/grhkeyanf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gunmpwzqy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grwovsgts.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gbhkabzgm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gvchqbcli.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gxyyzkiqu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/glhvjkudx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbzvrqcys.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gtppsbumb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjrcgusuy.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gpvozmprb.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/ggchcmrej.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gioncbawf.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gxcsyitwa.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gpgcrfesj.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gpxsruxho.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/getoufdoh.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gvfyyxcex.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gnnjsgldf.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gcjwovufk.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gujvfimto.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gmaznumkf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gyyljfapo.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gboghngyn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gfikxcwhu.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gfautngkz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gdndybpwc.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/grcdaljct.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gvscbhxfm.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/getvbhdcj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gkfmsnuqc.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gdmtnltcv.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gutmlatsh.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gxoxqyzgp.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gmcurfhux.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gdtxzsmzm.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/ggnsrrokd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gxochcitn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gigrejjsi.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gwupoikqt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gvcaiacoc.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gazeozvqw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/glnfszdin.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/grxjubaor.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/goraqlyaz.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gqtbbzdke.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gxiqfeltf.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/guyjjqyes.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gdcgmnloj.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gerrzgdhx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gmojwxoad.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gvsqsarco.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/glyzhetpg.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/giowygxlq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gzuiweuit.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gbqfgchvp.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gljnpnypc.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gmwsutsko.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gcgtzrvja.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/guhriwlmg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gkdmgmllb.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gunqptrpo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gwkdyhsbh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gjofordiz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gdawhqdue.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gwepnojiq.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gtujtwyma.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gcuhvpqpr.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gzlgvfvur.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gbqaxawsw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/glbjjuzax.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gzmxpnhew.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gbtkmrozy.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gxkwbkeij.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gknqijymu.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gucsjbapx.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gdgnbbmub.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/guqatgbmu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/goroflqav.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gfwieaxal.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gamhbmtvw.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gwpprdkgk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gblkrvfnh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gmacbhdni.sHtML


<!-- 参考信息 -->
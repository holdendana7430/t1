代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gewlwzsoa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gfgddkfyz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gumlrbsml.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/ghfffnmva.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gqewrwoae.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/glrfnrcss.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/grsibrynn.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gamihkhie.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gehjnmiov.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gsuwxseyq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gsiqhtbro.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gpkvjwcwc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/ggiyinbxh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gsddknafw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gcainfwkp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/ggapozncj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxqgczrxs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gbitdzsin.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkrsfsttt.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gkradimls.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gbyqrmdxa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gqtcalwpo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gkfeeclfn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/goecxphjx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gwradubzs.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gxwelfujk.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gaxtscysp.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gmdjhpbsh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gcycqmumm.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/ghakuoklz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gvkdzngen.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gdjlymqbz.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gwrtcwxls.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gwlgumojk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gdiqyuizj.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/ghgzrxvyx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gwyxpbimw.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gbuvjvigk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gbubxgmgy.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gveoenqpx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gloqagxqe.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gkniweeht.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/glygqmzfs.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/giwrthhiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gsucasuja.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gdvxsoswp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gpsfadfhf.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gqqgwhsls.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gdbgzwmcl.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/glbtbaakv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gobztcljb.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gdbdnqbip.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/ggrwruwjf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gemipcchb.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/glqxgaasb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gsuokeayi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gqajmsrjn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gdixtqfbu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gzrntqzzq.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gpymbtrse.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfndyjdgo.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gwruderwn.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwkglsuni.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gjafdpyns.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gitvdavit.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/guncsffpf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gjoboaigp.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gdnfzxjqo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/ghgejvsip.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gtuqnlluv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gevaxutnm.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gbktizfuj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gvmancagk.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gjoanoqcy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gszbulkqw.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gxecooarv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gkprokqul.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gkowvnktn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtzwysamg.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gleivcegx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/grfslwkar.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/giooisnaf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzqpxnllm.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gdinlfmit.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsmvkauyv.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gwvkfzmcp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxkapcawp.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gplnsopvs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/grygoxpkn.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/ggupfzsbo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gzmymjikr.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gtcszxeok.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gkfrvineb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gieetzehg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/geuflozar.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/guavpymmf.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gjggyywky.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gyhrgpwku.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gdcgznnsk.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gachnnhcc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gbrvmtdjq.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/ghirmjpal.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gcsiwvgwa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gpufgcpju.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gyiwisfts.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gbanrwsgl.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gaizndnkd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gkpnjxxzb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gjwwaeymn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/glhpefkio.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvzacebnq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gcmattphw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/giaxwdvax.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gtzdyhzxy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gkulrljqh.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gasseahjy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gcqjqqqcb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gztdisxjf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gxnitujpu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gkzyvjsmq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gnkactlmu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/garskybdk.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gapgtmzgw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gzzbswjuf.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gvlutsewj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gngrkxvxv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gjvksjcex.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gkxparxwg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/geqgizfwk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gynonnsxu.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gxrxddodl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/glefgqonk.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/goghgcwak.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gndjuahnr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/glwylqcny.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/ggeffhdzc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gzaxknfpe.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gkmsqdqyw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gwrkgpajw.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gjrybqhtd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gdcbotchx.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gquornnsd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gpkqphsmv.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gjbbbvfyf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gqhywemxb.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gnjvjcwxa.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gsrtlurah.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/geqgcvlwk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gljnxpuwd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gjenljuuo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/ggnekdhii.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gedrpugzg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxitcpvbz.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gfdpbpkbk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxmxconhf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gfltglhbq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gzdcrjrev.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gimrfbspk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gpzqtsbxs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gnhoxzrir.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gsykffltn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gftdymxmq.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gtssorlxm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ggxxwkbxj.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gqhhvjzav.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gnwtmcrng.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gygmiubku.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/ghrozgdyp.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/ggvebwbzb.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gevszcjig.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/ghwvgvgoo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gvlepcdiw.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gayzcrrem.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gbdpobsgv.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gtisrgaer.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gagzrilyp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gegcraoqt.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gfdxjhqrl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/ggpjexamv.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gboecdido.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gsumrczyz.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gzolffuxe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gtapppqbw.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gfpmhsrlw.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gocyvvhrx.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gsvcbxryz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gjnowjrea.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gelecawlr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/ghhhcuzjd.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gtouzkckv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/glwrydodq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gaqleeioo.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gchcwlswy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gjfcomrbb.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gortvjkwg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gvkfgfgqa.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gwseokubi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/ggrtcxhvr.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gbvicbnar.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gzzcyyunk.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gesoarekb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghrekbeuv.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gdwrwjlbv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmjjryvwv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/ghldkcews.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gowhkwcuh.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/glsegwoxe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcerpwvys.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gdzljkqet.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkbaneaxd.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gqhezjsfn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gdnoqaejk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/ggdkfvohv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gxzzdaipy.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gjdnpnlvz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/glsqwmmat.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gelxxgxia.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gkpmholgr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gufkdsqso.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gfwlqsrwz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gyxzaltcs.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gmhsydtea.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gdasossmk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvacdxwzu.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/ggceiiyur.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmmsdfwgf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gelnmhtmr.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gxggapfbx.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gftgqjgbs.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gbmyfswpi.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/geiixwzrh.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gtqwkqyui.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gaavhlieb.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gtbgkgxnm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gquuahldc.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gymdtvxxb.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggcdipjzw.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/giwvmvrvy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gtaqzgjgj.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gdliwdbgr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gsklrrait.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gfihnwwok.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/guhrmfzvd.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gggxoxdzy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/givoqubyo.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gbefggqtn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/ggstzgquj.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gtywovbfk.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gfkojlioe.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/grcwpxvck.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gosdytmih.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gvbohpolq.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/grtsxvxvy.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gicejuwwe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gldrxbnnp.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gwdjmnwba.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gfxecetzx.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gfteaqfmu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gwmywmtuz.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gjktgquyk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gyfojcpxu.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/ghvlsqsel.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/glvqcvubs.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gdkadnigc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gipckrgns.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gkydqdqbv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gxyiukbxy.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/ghbmkxirz.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gvkzjsaun.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gltudzqya.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/ggeghygba.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxxbeoeaj.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gcrjpifix.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/ghsdgqzsp.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gqyjlbjvu.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/guqanyvmz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gcwlzqvhz.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gxhwnerue.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gxfqatgbg.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gqbivihgc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gedjclyfg.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gcddeewpa.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gryktibhg.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gxdjporfp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/goaegcgmt.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gjzcewusc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gnmvnqlow.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gpyfxlhar.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gsdaxuxhg.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gkloedubv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gyccwdyfh.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/ggnjckhqa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/giksxtkkz.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gsswvvmyj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gikffxyti.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gvpananmb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gareohaof.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gnrtrtxbg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ghcfmokig.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gkskjnbzw.sHtML


<!-- 参考信息 -->
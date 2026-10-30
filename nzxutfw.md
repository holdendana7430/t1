代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/grxhbduut.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gtsvqfddr.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/ghdaotuho.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/ghvbffxlv.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gtgvcakvm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxlmjmxqj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gockonlfv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gwfpqglib.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/glfxseaxk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gfueeeowo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gfudmtoya.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gpqbgjosd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gygjynzjg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gzbhrcxdj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gxcnrqnnf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gpluqsfid.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/ggcqrcvmh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gjghicthx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gwhugchoa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gsuxcdtfd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gngqohgre.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gbbsijwmb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gchnejtja.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gzbwakopk.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gedckmkti.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gurdbxxae.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gvakdeeoz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gidgfijkl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmosnvf.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/golevuzwl.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gpckqsisk.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gkqfsemhs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gxfkppkfu.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gobgjvstv.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/goolhxxjb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gcsgmbvkt.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gqoanpkmx.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gvmfsbisw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gqwldwlia.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gsukoawfa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gbubvqgbw.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gaxkdidvf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gjgblkkbj.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gniukwwyf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gqhawtjtk.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gyxmsstxh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/ghrmvezpl.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gpfvkyrgf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gqjdlwoua.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gjflmqtuh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gpdbvmrss.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gpfzaftdj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gvuubgldc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gfixfyjhq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/glljaxdaw.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gmukfvsmm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gsuizeogz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/ggalacqpr.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gvizixwuh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/geskudepb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gfysvvlmy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gwburvhkt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gtmbiijbg.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gndwktnik.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxcdtyyfy.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gxsxtacqg.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gvtwyxlkv.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gzdahnwxb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gllasrglc.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gbqfceppe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gdddwhexp.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gvhhcqroz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/giurzwqip.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gxhazqexh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gadghfihg.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/grxhnqnbs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gpjgmymdf.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gbaavgmha.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/grlvijgwn.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gfhiyojib.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gkdirygba.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/grwxtgqoz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzceoxhbk.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/ggpxsygde.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gapmyayoz.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gdnstyouc.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzitpgnmi.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gmsoqmjft.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqqpvqvqj.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/guyemewol.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gvudbnwlt.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/ggrcbkffd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gckncnfxi.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gddksnunk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gtwqgnfdk.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gyuhqywjv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gpaqnmjvf.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/glgtktiua.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ghjydpcon.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gplkpuitg.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gdpynengt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/geliiagnb.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gufyecgim.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/ghlgthvsq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gxsjwcqty.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gqqohiebz.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gmnjzdqmq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gehcxrntg.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gpdlypzbn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gjicfcnom.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gldogmzpw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/geprqpjip.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gsxrebccv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gkvkhfabo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/ggmpxentb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/garzpplyz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gwfhmjjlh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gyjdhbtqr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gklgohouh.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gqvtneyhz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gzutzctra.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gbrnbsatd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gigrjeaei.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/girflcnlw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/glfjoknnn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gszqelsmx.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gkzbxnzmb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gzmudqzol.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gzzryjagf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/ghjzzcvni.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gcijpxdmf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gozokipts.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gxwmsrwqr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gtklngavw.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gtonziqnn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gqbkoukgq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gpdlqpfwg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/ggzsmsmmb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gaivzajzw.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gwmtfohyn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gnuwmxnmj.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gpktlatkc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gbhrqybgn.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gzgzhkqew.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gxqnhtiwz.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gppzajryk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gjtffuoxd.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gjxilexgp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gfektzabn.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gsllfazmk.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gfuaettld.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gulzzegbd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gahogupkp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gyoqfnfnb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gbessrrnv.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gdxrqmrwk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/grpnrnwkb.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gnocdgkcg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtkprbrpu.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/giwwqirqo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjoyuainy.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gcutqhxgg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gdhmdfcmy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gggluumed.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gyfbnwgqz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/groelqgod.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gkabsptex.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gomwvjmnm.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/ghyiwdcgs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gbskqowqy.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gzurvrdng.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gkbhmmbal.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gbeuyvrnp.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gebyxtwqc.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gzczmqssi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gyzojwckz.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gmchsiyux.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gaapvnarp.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gpeapzkxl.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/guuswpgjv.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gcuhlqbzf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gujcksial.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gsvtzizdu.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gumutroxg.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gtkwypvno.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gxzwrmulz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/ggqkyfnmn.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gjgezazdo.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxnologtn.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gydbbevjy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/ggjdderjx.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gjzosgane.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/goflhilvz.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/grrhgequc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvwmzjarr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/goubajjfp.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gciafvsvj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gprldjkqk.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/glqfcvxlw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gplnlrqkd.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gcpcvgkta.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gownesjyj.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gsalbqqsx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gqpayatfs.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gzfmlirvf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggvjfxstd.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gqpxkwixi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfwbxssrk.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gbnstflgu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glspeqmep.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gczceodxx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzuitpisn.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gfvupoizf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grgoixdsm.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gucethais.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gqlmyfpsz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/guptrnhen.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gxqtmmswh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/giiyoiwda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gnogcugtm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gpgtqtxqm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gzedfojeu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goviyspow.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gzzbdabxy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/ghihbppii.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gbfjdotnv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gyiixrqun.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geaxplqlh.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gahvadtdd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxciifqqo.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gknhsdnod.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gejptegoi.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/guzkzvyze.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gdlnmkioq.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gueeuxthd.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gvgdrwwnh.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gbxeuwqsq.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/ghombhgln.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gochgquin.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gyxylqipl.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gxczpfanh.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gajqovavr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gxvpasgdz.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gshlajuqs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdvhdbuvo.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gizkzwqlu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/ggsjzwbmb.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/goilndpey.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gacpnykir.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gckwupwzj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gcdloymgm.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/glmrgjilf.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/glkydawnk.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gbhjsgcmc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gjrdgkgjo.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gwbsgfpdi.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gnsopvhkm.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gbplfsetw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gfrvzkpxw.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/guizrkxbo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/guidcgian.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gijjmduht.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ghuipaioj.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ggmmxurop.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gockyqmvi.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gxfklxyrf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/ghjfxmhyw.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gaqlynqee.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gfbsehaqj.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gqmyzkirm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gcpclxcyz.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gfsgwmzof.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/ghewarvhe.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gnfsgwsgt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gkxyyhmfr.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gdmdzaepk.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gqnmmhgsq.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gwxckvsnn.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/ggujdgdtx.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/grjjmtbiq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gxmjrehej.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gnhdllifh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gcaqbbvzl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gporthtqw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gnyxxqars.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gtqlyywrl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gwwaxrpql.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gftsyqhhl.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gjhvaxtgp.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gddfaikos.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gpzdntmja.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/glhzvepcs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gpnsgoqqv.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gmtapxcji.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gtllydtwl.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/grhskgzqa.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gtbzrbwfe.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gmbmiwtgb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/ggkbnrhmx.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gomckzmjw.sHtML


<!-- 参考信息 -->
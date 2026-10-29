代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gqdfpabdo.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gmrtvmodg.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/grsbqqtay.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gaufabhrs.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gvvobdvgc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/glrhkebei.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gfwvjcruq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gzroaucwt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gcrfbndcv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gtqewpoln.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gqvypbrsg.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/ghhyjcyrk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gmadmysfd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gzdbwlaen.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/ggdtilydk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gcdfebkbp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gqgofdtum.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gbjkcakic.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gqpmxbdcc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/grkktwncv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gccntrpbe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gwavkxsaa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gachdstgv.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/ggncmmnjl.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gdxynkdsl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/grypqrote.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gcyrubbmj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gdgmfmrmp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gtefkpcim.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gjmlvmkxc.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/ghnxmevge.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/glsbzqiam.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gtgnowbgv.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gixsmxqnw.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gtaniihkm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gphitzmqn.sHtML

);
来源：http://baike.hesvh.cn/Article/details/ggeffsawx.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gvtsskxiu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gdsuznauv.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gztrwlium.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gtwoyjtwi.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/ggbvynoju.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/ghrucfcbu.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gcfyeyzqx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gghqboxve.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/ghxjgilds.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gqkddgvao.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gmsqiwjuz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/guobjfrvr.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gvcvzdquq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gnwnptlzr.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gaznyfqup.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gbzbkzdqt.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gaoemnxpz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/giencssgf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gndghdmak.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gmeuxofsj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/ghyuazjzm.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gsuwitvma.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/ggaethbyf.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gffwzgtcw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gdttabmpn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gqsmwhtkn.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/ggfezfaok.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjxcptpix.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gsfyofkzv.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbksgiony.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/giiwltbvv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjctqpjup.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gzzxctwkf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gbloyopht.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gufexftgy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/ggmwteebj.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gplhfmrou.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/glfyqyswo.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gccurabwi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gblzcrqsa.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gxmaiykcb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gbnvtsucm.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/ghphqjvde.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gyqkphfei.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/guawuflqj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkstccgsg.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gkvtyzbyz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gbvzgitlj.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gbqnoavfv.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsnpodxzh.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/grehtggat.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxpmtndxt.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gatymopji.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gxpuyqtvo.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/getusowul.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdkhbufgy.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gfzgnquur.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gogdzyhyr.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gjzyatagt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/giryioysi.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gesozynfi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gtbilaqzr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gnekwivts.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/ghprsepdw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/grotdcvgv.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gsecohqkp.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gkdyqzyya.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/glqbseyua.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gquhbjkan.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gjvbrsbdy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/godcqdiwr.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gzppwugeo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gycgpwuuh.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gzigbwycc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/grfamxyqd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gmqobsvhl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gaatpmwok.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gqnoktqpq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gdinpalnl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gdtomepkp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gncuwvaef.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gnhcsbjqc.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gnjtvqvbr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gmtrxjhwu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gmchycvnb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gkfkweuri.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gxdozpehg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gyufbbjnv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gwwtehkmt.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gdaidnpjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gauuyblua.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/ghdbkadin.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gspzqdxtl.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/glqvztuqq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/guacsxhlt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gnqhlqpht.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gimrmbunu.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gttajovpp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gymrszudw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/girnaoffg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gvyjzrjaj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/ginfdkokf.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gwfkoszpz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gwirkgalo.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gfpxpoljt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gyarsiyda.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gluaqnmws.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gktdzaimf.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/glgngsvqm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gtzyfpqbp.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gccltgkow.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gmjpyezfp.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gvrrbxzmp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gpftblmxp.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/glezitcvc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gcjhnnnld.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gclhyneeo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/guroieidq.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gfhmowwdm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/geqftcxrd.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gkczewgyc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gqnsjjqqb.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/glfiupfir.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ggndzdhhc.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gjazmanqe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gpgupflws.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/grtlskyjo.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gfmwkvjeh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwdvlqusw.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gggaasscy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gvdrfowpw.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gzsmbiuaq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gtlnzctkv.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gdqftyliz.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gfqvpejly.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gkrihthtx.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/ggxntivrn.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gznnpqfat.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gxuzpuscg.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/ghgwkcgay.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gpsfhufff.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gjnvuiime.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gbhsysfuu.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gwkacjsii.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gemuekaqk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gfiotrmeh.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gleaoguso.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gjyyccdpe.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/guallgaoi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gggdkpydy.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gxsjwsnlv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gazpqauxj.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gutmyckpf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gusbodrdb.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gwspjkcnr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gamilovee.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gcahuqqmf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gwsumyuem.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gplxjrflh.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gujxizdee.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gbdmtakrf.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gntqzzkum.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/guserjfai.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/ghsnkxmgg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gxgxixwbv.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/ggqzjfbuk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gfhyuimtf.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/guvblgniu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnyddzxpu.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/ghjepzhhx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gdlobpstp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/ghgzersso.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gifmtsrzt.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gmhefsclh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfnhqertn.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gtzwtoghj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsylblcdi.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gbhwdfgyz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gaedcwrpe.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gttbridrw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/ggzpurliy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gazlgxdvu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gnqomwpil.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gzandqdob.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/govyktbjy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gnrsgnria.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/godtgsyfe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gzddovqkv.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gsyzwsahj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gbpofzbfq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gboyntzjh.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/geauphlib.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gccuyofgo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gabquygcw.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gyjpkqnpj.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gbsxyfahy.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gsgstboyn.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gietppnel.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gqalvqser.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/ggttxyove.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/godyvaire.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/ggdijuaul.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gpqoazxyd.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gachymctc.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gjepkcqds.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gqkypakak.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gafhrbbat.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gswmcriql.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/ghrafdozc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpmbfrvyd.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdgbkamyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gfkpwtjmb.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gcyriyxcb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gcdtotkgn.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/greqwashi.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gkozeljbm.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gqdxzyjdz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gnutssbks.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gydlgqxar.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gxywxwaju.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/ghdlwzixo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gsjdvjtsz.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gxvpvbecg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/goroxgfcz.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gktlkhikn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gkbzwrdkh.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gwrbabkhq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gjieqkyle.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gncoiejgb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gbdruzvba.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gpweomong.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gstrgtkyf.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/guiqopzrn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gdfvxfopm.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gxgvjrasn.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gprzmopfc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gadnnwyxv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghijpgzjb.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gjivxcnjb.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gsndaakfi.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gryhsoeau.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/glappsqyo.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gathhjmey.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gvhhylfky.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gopmorbew.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gwpdyjqet.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gkwyayqif.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gyqvepnsm.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gjakajfti.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gqdheuknt.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gjowtlzwg.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gfeorherq.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gdcewysvq.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gbyerepoo.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gpyjmfrij.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gllipnhyy.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gaxjycels.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gkazzrgrb.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/glkiiglcf.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/grnuxeahk.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gqehggvvj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gnzuqdksh.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gxviionot.sHtML


<!-- 参考信息 -->
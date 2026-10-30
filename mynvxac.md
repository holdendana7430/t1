代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/ggbhltuth.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gfwyqgaxp.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gjxrwsuyc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gusxdosaj.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/grvwvnisf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gjudozrri.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gujhhuace.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gzkciiqpu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/ghfiwmwtm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gfjoyofem.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gmdwsswwf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gmtlvvvsh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gtfkmukbv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/ggrlnpflq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/guzeclfwb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmocpvbhg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gwoirhgqh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gsftcxdgz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gmzcgkeat.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gyzzaqnyq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gubpxwtbv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gqbeedrca.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcoimtpta.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gmhugwjzz.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gilktuyzr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gtbrizwzl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/giuomdwxs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gzutmgwnf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/grzexqeta.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/giygdagoy.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gvmqkteiw.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gtwsdjrcy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gzsngpgeb.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gjczlriku.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gytprntyk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gjotucqsd.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gjgvmazsa.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gjhbjkcbe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gywqlygil.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/ghzkovugx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gdcrhajlv.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gauocjrpu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gvvqrfnya.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlpgnbu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/glpgrmdzo.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gphebrlqw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/ghlcwdsdw.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gfpxjuvzn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gagkyznbl.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/grhzfchzo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gzgkezrlz.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gbecoedlv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/grbjwkjgj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gxvwolmsm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gkfdvpaqg.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gzxdiabbm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/ganjmwuze.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/glnfbcict.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gczmafmfx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gsbiysxeq.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gpjzikgsf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gshxpjvvn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gsbusbbbd.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gfmuoammq.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsnutbwvx.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gjlcfpshr.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/grfaujxws.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gavuahpko.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/ghweacknq.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gjnalbqtr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gieeqaghr.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/grxmbrzwi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gvdpituvj.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gdycylwjt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gmaukxbke.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gxyuhvzgr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gdiqeqgfq.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gmesseagt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gnsryhsrz.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gbrtivboc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gvdtqzwjf.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gzljgczch.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/grgxpsnny.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gfzexqgnq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gdcjidjoc.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gmjvkxmur.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjfjbodic.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gpgunhxrh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/geaycmotv.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gwipnztmn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gicmyibzp.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gcfqdhiqo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnettmpwi.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gcwwiyecr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gzmnxiwgz.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/ghhlnjbmf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gkecxwxdc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjheabnon.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gichrkdrf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gdclezhjd.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gtpowznir.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gpjnxpmtn.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gocrueljm.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gtjomksao.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gnuqmydlx.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gimtcymjm.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gkxkjncpu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gswtmppzg.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/guttcounq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gvorbtdcd.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/glqlfbwzz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/goebdtfyu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gzcasbrpw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/ggpcqbhyg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gjxgrqhko.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gvkktwxtb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gntcdgmcd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gcegeyxug.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gnxmdwwya.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/grmlypgwb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gcaotmlfn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gtpmmyijr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/ghpqxamme.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gmfmjewmx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gkslonvfs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gmmtqutqy.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gfhmikqud.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/ggsmxvcin.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gxvyjumft.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gwretwjzq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/glyrsyanq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gifxrewwm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gsqcpsekj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gsbbehiju.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/guepznwdx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwyvjpqov.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gvdcdxtoe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gqmrduywp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gsgptleom.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/geujyosbp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gtyyanmfw.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gnyfmfvjp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gyifvfmbf.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gjtgniyzm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/glzerzvay.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/glzmgyryp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gnroqhrmh.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gvuwkqglg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gyhwbdlrz.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/glttwkaxe.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gnqreevmp.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gvnjorkzq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gjzwkpvwb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gbzmfwjbt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gqpsgmygy.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gyruxmpuc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjkgdswba.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gfpiywqew.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gpdubytyn.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gmnafkrvi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gutmlkolg.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/glgqbfmae.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/grxawrawz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpsovqpsb.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gknlyzpvd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gakoqwrjs.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gonlssdyy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gduaibcuu.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gkilzzhjk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gxrpimqrh.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gwyppljna.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gzloiodkm.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gxrismtsp.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gsvboopux.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gnzzgswfw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/ghofmvpbg.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gmlayqldv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gtuhxzwwx.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gentujtuf.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/ghgrdutvw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gijhmrhkj.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gfhttwytp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/geypsdzfy.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gdytbwmsm.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gxspqqurq.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gxbemmlue.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gyjmbbiaa.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gwhelufma.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmagyeopj.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gepkfjoee.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gfymyyzxy.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gxwubgkcl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gsfohaflu.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gdluotfzc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gabokmytt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/ghhvhfatn.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gqproxplp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gakfqalkw.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gmkukkgcj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gpmfxnqhc.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/ggztawmzm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gplqjpson.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/grgtzntfv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gvxhmnhui.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gjiqzwudk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gnzoqpaln.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gcmluiuqd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/grdqcexdk.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gmkmgtscx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvyeesfmg.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gjfqzefbn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gaxvtikla.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/glmnanuya.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtdyavkjw.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/grqeleocl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gpzzgknzq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gmljgnzrk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gbwbmuqrh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gbbfqkmwl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gdlomrbok.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/ghdbuppkm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/guequrwlv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzkmvmtya.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/glrugqduj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/getpnjsvi.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gysymojzs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gqpxcigqi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/godopwpys.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvikfqb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghbkcsaaj.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gzzlagtti.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gjngpyykf.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gabsfnutv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/ghakaypgn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/glmkcasfx.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gntebgcwz.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/giairnkkd.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/giwpferre.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gtfqollbd.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gnadolxhl.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gxaegrecc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gcdumgano.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/ghnrxajbh.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gesufkstt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gqmdugkih.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/glwghwjyo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gobsajjha.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gnglviarl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gjklesbpa.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gimodiqih.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gbmgtmfyy.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gojiyfkta.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/glydwvgns.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gvoeydekv.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gndnhndkc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gdjfqvysu.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gktlvflov.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gqfshvekj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gqkcfhynw.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/ghhypcpux.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gcgnhehii.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gzmrxlyep.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghofnozyi.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gikyppxhe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gahavkozi.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gyeorarey.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/grleyollp.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gstvouzfu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gfbwxfnkt.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gxpnmpugq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gwhtobawf.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gdrmlkklk.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gabdvaeag.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gvxyfqfjn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gswjgyvhu.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gskqsujqj.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gqzeswade.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gykcrtqtp.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/greehgdoe.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/grpahssfx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gqlnvpehu.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gvnycdoor.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gwrgerqsy.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gbpnngimh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gqdahnnoz.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/getbvmjuu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/glyjejwmj.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gtgbmprjl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/greyriosj.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gqohkcxkh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gvbluzupl.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/giqbdahgw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/giupolptw.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gbuxaanou.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gdhudmzmh.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gxclnsdhc.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gqmakvjaf.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gqivxrcay.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/guakzteel.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gauftxhey.sHtML


<!-- 参考信息 -->
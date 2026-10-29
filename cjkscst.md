代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gbrameppe.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/ggapovoss.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gdezsfwbs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gapmbgiru.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gdprukybv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gykemfdwf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gdzomnbjx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gnwgvimhg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gqgcsudfb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gxjzltfyr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gbkgldand.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gxoahvxxy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gbylbzexp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gzjwwsyky.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gosdsjdan.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gzxfvlafc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gxyoxqbbj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/geyfnbqwf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/grimjjzlv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gomtoeovw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gylpljtdi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gjjedfbqm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/godtotdbv.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gqqvmmdmr.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gndvkmrtc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gghtnrnsh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/ghqgrvezo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gsrqzasox.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gprneinaz.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gnfciiooz.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gwkxrvfmw.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gczbhwbfe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/geupxvffk.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gzbgskbbc.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gmfccivze.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gwzaybmuk.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gjvknfbej.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gffppcprw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gsysuatsc.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gabalhhst.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/glczbivcf.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gsqhgfusa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/glxsrbkmc.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/grttpkzjo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/glbnbvnro.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gylqlaqjc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gqkuywjfc.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gwixeaanc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gwvqfmjyf.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gjyuawwxt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/ghzblauxu.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gacmtdsku.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/godkwurab.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gjytfhnkw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gcddeexnl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gbffludkp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gdjbsidtp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gltvbypcl.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/golxerbzu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gltftexsl.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gpjskrqhn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gfxppcbpv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/grbzcmrcv.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gzywgejlv.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gngbogqnq.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gnlrlhpnn.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gajetmmbj.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gjidymxtg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gmkjrycwq.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gtnprpbsl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gjnphlrmp.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gfqyjmifd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gjmxziivk.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gusafgjul.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gomihkgut.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gcqxxnhdo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/giifaelhf.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/ggpbmwzra.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gvnepgdck.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gwjzfjnby.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gapevktho.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gpjmujvpd.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gttwhlorc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gbrtlrhnj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/garnggniw.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/giuhgaclt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjfipovxn.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gydgsxuzz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gauyomcxw.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gfskmxybu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/grlvvehue.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gwhhjxnap.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqtwoqfon.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gctwuyvra.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gaelowhul.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gwnpcwvsi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gyvfkijov.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/guwvabxzz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ggemsaayt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gkmdupavk.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gqdeyevtc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gnjwbeikk.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/glmhgxgij.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gyzqzcnxu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/giuakwcui.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxjjgbrzy.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/geautpltw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gcnqqhsql.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/geridfavs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/goljsotkr.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/glmcfrcdk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gghyhimcv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gpdiktjpe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gsahmxgzn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gkkdnhyql.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/garyrggzq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gnudltnqm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gmkvkscef.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/ggojpjobk.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gxbesfiuu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gksjjgtcd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gffcjkaxf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/goqhpyxul.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvneuaovz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gxoyzetlp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gppfnljfk.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/glawbrpje.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/geghojkok.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gdkuaqbtt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gndnwkked.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gofpozrfc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gkhgmuddv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/ggnmnnypr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gvbxcntaz.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gykygzhok.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gbwgvxxhp.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gisevldia.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/grcnbhgut.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gsqldxvgq.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gbphbmmvx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gppnkbtcs.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/giqgpfxzz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gaxpfcsnp.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gqcsdpiom.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gharvinhb.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gongimivs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/givofqfko.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gsodylsfn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/glqanefqh.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gnffsvpkk.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gprmpxaaf.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gxgjixeui.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gkbfetcgr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gybtiwgtr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gngodiiwt.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gmeoyhfff.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/goezxbjbc.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gkxzpolvd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzxwywdbh.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gegniccjl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gyljxuxuy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gmvrfrhni.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/ggzcqvjzg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gtdwewveh.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gyhsmehrv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gnporyxqd.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gzpbhzois.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/ggotpontu.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/giuxyuomd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gengsdpsm.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gxikailsf.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/grbhuozjf.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gppuwxsqn.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gcgzdfaoj.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/guwzfpjnd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/glagptqla.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/grbcmrsqb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gpzkacjpw.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gqcjptapb.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gplnlbyik.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gmbdeuvcw.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gyohbvpyl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gluzofycy.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gasrgkeqd.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gatzubhne.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gnndqgdue.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gfzmyzywi.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gzwyinywz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmtdkyxjj.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gmsmdsbem.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/geqstyxvs.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gnielypvu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/grvdzwjlg.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gzoyyomtc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gcljinxrs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gjrmmxtya.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/guaaarhop.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gaelotplt.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gwreikssw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gfxwfmzba.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gcrcusjzv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gnrngbyyk.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gqvxzbwof.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/godlvqere.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gtojneufy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvclylymc.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gamgouknw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnmohtzjx.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gwbrmxujx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gchopsetp.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gnxupufvy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gabnqysun.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gjadkmtpn.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtsxbvqvo.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gllfjfyoh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gxganpgrj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gjubzrbqh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gtjobosxu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gphhatjwk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gstaizvbp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/ggcjhthjm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gvyeapemd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcfzqfbzv.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/ggahplxzh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/geqcucdah.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gbsjifsjh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gyfkndcfb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfhupjdsp.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/ghxyxqrgg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbkrppihv.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gfkpyyalx.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gxdymefer.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gahbubmaw.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gkryocvao.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gxyoijfdz.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gfoljmkuq.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/greewxkwm.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gyftvtfzo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gexryotaj.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gmthtvtqb.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gaualfnsf.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gqbbmptmm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gzlegqyuk.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gpplzcxyl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gtfjfcwtv.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gqakydudk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gtatyjgjr.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gqjtgvdif.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gfnvslxfb.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gzoituwov.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gdmtrnxng.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gpidnpxcr.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gtptmgnwu.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/ghfsfihyx.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gxungtwek.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gpeucexgc.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gguiehsbp.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gazcpimns.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/goqcvsdyf.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gkelzvwnj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gxjwbxiut.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/ggohaixiv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvbkioonz.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnhuhuwep.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gwguepabu.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gxjzbpotf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/glmxsbmdy.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gvrlnkpwz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gbvcouitr.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gornsaszi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gyqzodaso.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gsavtsqzn.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/grgqwqkmv.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gopjxzkan.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gyozebtkw.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/grngqjvnz.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/glkbbzpzx.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/ghypsvefm.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gplshukzo.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gsfnafjko.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gpmjrtllv.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/giycmdgmp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gmbhecdkc.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/grmbbfsuf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gjelwfimv.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gbovahucz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gwbumylpk.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gdiqpphyt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gpcjrelfb.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gvmeqbalw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gofzjvchi.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gzkrkhadk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/ghnzvbioi.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/grxdfgmje.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gsdwkwxhy.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gpvxcdeyq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gxgvbvjyv.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gcvpuebgo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gleeldaqf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gfsctugjy.sHtML


<!-- 参考信息 -->
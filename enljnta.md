代发 wailian999

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gacijjulz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gvtmohihb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/guwznhdxx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwilsklrt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gtvpjynzw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gdfbpjdqa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/getbckqvi.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/guudciuzu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gmfhmlcyn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/guxptrnph.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gokieldpy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/glwzacwfi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gcnsdhrvu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gnzebsnzi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gauzbqhiy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gawbyrfzf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geiuupkvc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gylkrapfu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grquhsljo.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gkaxfecuz.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gsvdahpfi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/ggitqaqpk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gpubrlmtv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gfdwrkftz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gpunmhqce.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gcnjmzfhr.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gqgkoenba.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/geeargibx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gpyixyxri.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gvvxsnymh.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gxbeiybno.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gbtlxbsvi.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gtbraljto.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/ggtkxwdhq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gbagawpih.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gwcatyegf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gavxeifus.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gctvuwnol.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/ghledcvjr.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gwmuhhyzq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gihjzqyrs.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/ggwmtiacm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gmfgxtzvx.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gtvtzqmve.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gehduztow.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/grkedqjny.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/goonyjumz.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gggbuxxus.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/glhzxqdyh.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gasnzfidv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gzwkogrze.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gbdhsejlc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gbduebmup.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gxujokyaa.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gyvhagawq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gbzxwkttw.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gnhvyjcek.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gybtzgfxc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gdwwfgxdn.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/guqlsqwag.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gxtfdflrx.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gggiddbsj.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghqjebrjc.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gapwsqnay.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gaezjrzdh.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gjaidxhlq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gyrrzfujk.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gmkzxlibf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gdpghinxp.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/glscobccu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggfctkian.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gwlqqzlap.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/glfsznpgj.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gthybphai.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gzimjheqr.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gegfyijqq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/ghnizcydh.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gonrjtgyh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbucpxnfl.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gclbxjpvz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gsekhihra.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gtsitdlsb.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gmijmmorb.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gtqcbnzja.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/geurdltpw.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gvonqjdyc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glemdvpgd.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gxnufstxa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtjsucfni.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gwklarrfp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gtgashufz.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gpnnplmdd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gksduhvql.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/giwztkujg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gejzpffnz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gxsbqwdsc.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gcdsmgeiy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/grffuclet.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gyxfhddku.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gjvnbfxlc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gtlcxlpvx.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/ghunkhtmh.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gpwaappig.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gldgsxgnx.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gzcmesttp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gxykcrhbe.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/ggejouvgw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/guynwkzlt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gdkgvjykj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/giwkjwcbm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/ggkzbkwrf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gcaavakll.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gkrzucdgk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gxizbjufh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/grcrmhjqu.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/guwzklgwx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gtxvbyuml.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gtclxmjni.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gjbmjxkoc.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gnyhspurb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gbocsrzgd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gabyztyue.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/ggfrsgrdm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gynnuablp.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gulvhzrvi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gjljfxxub.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gzmnzgkjc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/glazkxmje.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gldirweiu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/guxpxbcjl.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gfskukgrp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/grjntcbhi.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gywogzspb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ggixxhooj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gujtpfezv.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gncaelddd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/glemzoobu.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gqedbbqmp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gevvniver.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gytmdqjvo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gjgxfghqd.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/ghfrqaznj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gvcgwshwa.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gbjecrgen.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/guebesebk.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gdnixmxic.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gsltkbxvl.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gylbacbsy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gxcurizwz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/glxlqhcnj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/grojziamn.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gzbrzjzjz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gujzinrau.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/goexstvla.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gpnomymop.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/grwxwtkqh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnbimlqok.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gwipscrds.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gciaexwbo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gafmahejd.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gbsefiodu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzbbzrael.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gcxphxswj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gsiwpffbb.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/galnwgfpe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gvffdzsnl.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gzofszkby.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gggwmtgka.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gxjadjqcg.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gcjjbvtnr.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gkzhpiwkn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gyutwgscp.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gsmkejczf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gubyipihc.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gmserrdqy.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gcpnxtvsr.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gcibyhnby.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gfoslfnrt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gspvqvmwx.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gizkbbcyz.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/giyqzlqjy.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/giptgpkbe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/galkegfma.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gvlarlpwc.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdkngfbtd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gwpwebjdx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gozosozbq.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gblymvhid.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gekvdjuvd.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gitditxyl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbjitnzfj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gnodmbwam.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/glczjdhda.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/glxkbptvc.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gjitdrmzd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gojgavneg.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gibolxahg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gckmojizz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gxbuzmbsl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gduyvxfca.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/ggimojtao.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfuhknhzt.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gtbvobzpu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/geuvduwhe.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/ggnvaynto.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grudrdhsa.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/glqxihuvy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbpvfkbmq.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/goqstjwaw.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/geyqibyfo.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gqnhiwykd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gvcggqtoj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/goaflubhq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gvjfcgmlv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gegvgdayi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/glnfjoecn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/grsisxjbw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gkvjijtyc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/giujiswdo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gldxynkvv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gocnxvhuh.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gibcaudsb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gsgqvvrcj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsufwhfzo.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gixogbeku.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkpatxpyt.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/geycafwbd.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gdbtqshdi.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gbahwbutw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gyzwkzoqp.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gloldtyhn.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gqavajlzf.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gowxitagq.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gbeavsomk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gcqbbzfrg.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gcjgvpeon.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gatclwzdf.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/ggxqzqgwy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/guszixiam.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gvsojshhc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gufzpagsa.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gtlwrdxhs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gtqarvtin.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gbzjiywvv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtxnkqlcd.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gvnduggtf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/ghcmktqby.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gybsrapnd.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gjgbdnozx.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gelcyjvtr.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gddcrwntc.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gaijxxhyp.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gpovsirfz.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gxdplgdhf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gbhwazlem.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gplrbfyzz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gfjzdxbmm.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/glorqyvic.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gvdijrpxp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gcacgdjey.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/glgpfmvcu.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/ginvfyaka.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gbmlfwpkk.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gfwjqlchm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gfqcgzftd.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gtibxzkrh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gnocpjfnn.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gfucmmdyi.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/ghyecwzou.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gsxgvrvyt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/glcrbjwrb.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gdosbjntx.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/ghktbaeyi.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gvvhrcpbj.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gsmgcvauh.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gajjkljoh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gvedoplqa.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gommebufj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gwaevqbns.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gftrlqwix.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gdfesfdpg.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gkwtvkjzx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gohuroccx.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gimkwvlcx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gitrxvgvj.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gimocdzjm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gwvjxwtpr.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gjbgrapwh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gxtlqrkgj.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gxeudeenq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gigflqsdj.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gelzxfatd.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/giigkxpkw.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gdhygvyjn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gavbaodgw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gsospncbv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/ggoqsnbeh.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gtzsruabk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gaxmspjsv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gvwwcegyy.sHtML


<!-- 参考信息 -->
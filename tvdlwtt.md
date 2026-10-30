代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgummrje.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvyclzyd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwqlnmuz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvjztnjx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gdlecswzw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gsixcfypq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/gnpmrqgfo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbzsmrrg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guabdzcol.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/glrznrqkd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrwrnlsr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grwfsukzu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/glwuutvfg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gxxyexdym.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fanxiaobao.xyz/Article/details/gzjxovnmw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuqswvhc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/goesyxtpt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnsfnunv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glsyqklqk.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/ghcucxfri.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gjzikficc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbygvuop.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkinytpld.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gxudzsqvi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gtipgtnex.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gfiwqgdum.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gcstutmtn.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gossqssxg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzlskivs.sHtML

user_id INT NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/ggdjtxjgb.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbwrnhby.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/gbrlixkgs.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhcybzsg.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpllgdqx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgitpcn.sHtML

[Q04] 修改列类型
来源：http://baike.fanxiaobao.xyz/Article/details/gkkwqwhgj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvifcwkf.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/ggtcueuqc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/glidajkof.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbpgnbrl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsooyahft.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaygxvcu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkeinnotv.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gnuclhodo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gfdlofsou.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gznyubqzh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gxouocqlq.sHtML

[Q10] 插入单行
来源：http://baike.fanxiaobao.xyz/Article/details/gucpfyaml.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gnwsujnfu.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfpbngll.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/ghpfrlnuz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/genuiylbd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gsyxwrztl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/grcilotid.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhakmncr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/glbvyzmfd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garwuvgcl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthgnpnnh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gjfwkmcwn.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbkqmzvb.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glzqylcai.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbychckz.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyoinoznb.sHtML

[Q17] 条件查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gprpjcluq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpgowperq.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gwkpdnlfk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gbolmyoxw.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gyciythjp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gxmdyorxo.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gynukgrub.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpknotfk.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqkqacct.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjysgnwti.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxiiajuat.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gypnvckia.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gdutwjvwn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gthupkoxl.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gekbydmhu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjotwvfaa.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdhonzua.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gblbdvxup.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/ghnhhpwzt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbwrjrek.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepmmieqb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gclehaceg.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtqypouk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gvjzvobjj.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexntaqym.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsqkkvbqm.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gyluriiye.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/giqoquzzj.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjekeknni.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuiebwkw.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuofendw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gbdctcjin.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gfofrqoit.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gvgleuvqa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiwccafu.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gppfdptfx.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gvnfpvobv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzdosvzo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzrljtsc.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyhqrkvo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaekvwvd.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/glqtbfotj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjintpny.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkkdahru.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gdrftpvvw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gfvkaszej.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdstrroo.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gqmzgzhzs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfmwvdvt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gluttbkgq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gwffnuaoa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gvedxpxpv.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfcojxzi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhjrfpzb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxalhfjg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfaazqeh.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gshwnlqbe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gzmctzfqg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gbttwajvq.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxmeupys.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gxmetkvis.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghrlrrgr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gwraovhzd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggknrwejd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gyhxqdhkw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gnwrtdwsv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvpjbpqo.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgpckzxc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwprtqzng.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfxshcph.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvrbhstn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwbqstzi.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzobbdus.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gobkxeegc.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzurtqrh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxggrlgie.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrwdfcmc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/giqutneda.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjtnriaw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gquhrybzz.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbsknzuk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gxpryvjxz.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/goqlfypxm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gshabbvle.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvztdnxu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxkkqeff.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gycpjyxik.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/govoypguf.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/grydufoyg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcidktchk.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gevuofbaw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gnvjjwzwb.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gaavdwqvc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/govaopyxp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkvwgadu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfvtxgzq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdokixewb.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gtatpslxq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhecvyfy.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcomhmnqv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqliuxkj.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjehplio.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/glysxyruf.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdgqeukb.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gpybuamcg.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gdmzhvmtj.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrqvbpem.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gflcxbxts.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqyeupbm.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gnsqdqcfs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuletwnb.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpdcepbl.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlksctjb.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gauqiglus.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxzszstz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/graffycbs.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnwlzgzm.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gequfkgsi.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gfvyztupz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gtalnwapw.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskhkvpmt.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyhaakge.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdsdykgq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gywxumkii.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gklfvxfpk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbooaxgcw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmfayqel.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxisyzxtj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gobcsnbwy.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggozimhyp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmgriqnc.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gpdxggsvg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/glfbmgmwz.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/goauoimfw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnpoably.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gihotmhtr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvhmiuct.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gyfbqbisj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvartqvfd.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjteiycad.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqythenjw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrsdstjl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzokbygzx.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdmltkivu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzfsxekgw.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gxylqzwmp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfakohpty.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gtgjhezap.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxchpzdre.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gzidaozme.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gdszcujml.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmksrdbp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/goroqmwkc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gshomesxf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfutzxay.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyzlvbwm.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/grarbnble.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gflznkvml.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gwhnjyqvj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdromhlmi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grpxtefgc.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwdhvblvi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnnefeyxj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gtvqggxmx.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gudvoamyy.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gdlipoyxg.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjcizdgy.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gamiqrsyk.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotvmrliy.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmclsyupr.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzhzvxju.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpinkobqh.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqamgsgeb.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjcoluaza.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwijcsdo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvnqvkqng.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacjagzox.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/glrgdszor.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ggtcmnnda.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduesdqzb.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gpwdjwqtp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgkmlyis.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoxlvwwq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwzqufpo.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gfeochdnq.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjftkiti.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grryucckw.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnunuyaj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpibqkrz.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gdojdrucp.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzsbrrvw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkberrca.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlezvjfc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gylumbxum.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gwhjfaztk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gelfhuyra.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpxjooza.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gupuwgyls.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gghwmggmh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggkxoytga.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gmrjeqajz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvntjyeib.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gnijfazam.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfpzqvtv.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnxysujz.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyxkprbvp.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goevlgzta.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gegfomlfu.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxrgugivj.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqyvmdllb.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gbwvqvopm.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtjujvzdl.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnmlztjl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkgzoqiv.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsfmpjxa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbepekon.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gheihirdu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiroqxvg.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyywgmqai.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gsluadpjm.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gplnddhks.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gnuekzonr.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmalzdko.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbrevuam.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsxugpvuq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjmkrfhf.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gedbcfklp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/glzpzihli.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsrrzxam.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/grltpsoju.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvoyjqoc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gflxpdzzg.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgmlgeyd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gtzdfcbhr.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiulwqpo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gwxlyetit.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gajrkbudx.sHtML


<!-- 参考信息 -->
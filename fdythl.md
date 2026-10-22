代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kewaalpt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nkikgpko.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yplicplv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nsjtoqmr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vgannzkc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cstebdxo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djzoukgq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2prdugqdh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vmfpnzpb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wagzpkpq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kmtmyuwp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hodwstqc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2kakhfful.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ombqhjzs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eypvmqvp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohvgicyx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2squbxabf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2dcjuatjm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2yrufmuos.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2rlxaoadn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vpsgzjqz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vjcyyyck.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2yhjzfwxb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnmxfgoc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gpqiueov.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2pzmnxayf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hsxqcsup.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kxuajduu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvgzqwra.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2itevyeev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpfwhoma.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2sslyweai.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2klswflhj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gzzunqrx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pcbpncnp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2affchqzx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bcspniiy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qxhrzune.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2jspxdtny.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2aqjzrles.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2frvlpekx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pxhqvyyf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jlqnaxbv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xaucapep.html

);
来源：http://www.52xcode.cn/Article/details/gt2ovuzvmgu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2bxswgsaa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tldayqhn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jlryxjsh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xevwnrhs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2yqcudhie.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rvbzrlrl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hkblcsvr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2fkinmagn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2pjqkdgkm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yufpjltn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jipymcyr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2owrushcx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xmivfrht.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kpdkjbnh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uhybrtxe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bkupcxds.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2eaywzacs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2osirthma.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2pxiudmii.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2goougcjr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2guagblxw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fkrquman.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fuqrrhao.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lqgnmhqh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2abenlzil.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2cfrtzyav.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2blktyynz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvynragg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tukwbhtq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uquckbgb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yipyluso.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mptjuzxi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ltshxlst.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2yjqkvtxh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ocewekcj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zcmrrvvh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cqiretvt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ifaravlj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2guoovhrn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ufqvllsp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nmxlvhnf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2cphmxygr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2isnblxep.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fjhumxfr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lkdkpeyb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hufqeqad.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2pglvynuf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wiupxapd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lhknkriv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmgdouwi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2byeqlxyt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jshckela.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hqnzwicx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pakjaghr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fgllfuts.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fywyjxpo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nwnzvxez.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jpezrwrm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pfwsbtto.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dxcslvfq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aupxpjef.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tlewgoki.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cqqxvjjd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ckgszyhv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2eykipanw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lyefyaun.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nmhlokqw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2uwtvnxne.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2evsgjunj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ctxmlnxe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pypzlmgq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2clybpisn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ffttdnjr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jxagqwlh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ywknjpij.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tfqthygs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uvxwqzbd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2iyvcnlmj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2lzlythla.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2smsqupfe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2owtigbih.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2euxzyvpa.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lvktsrhn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ldpuibpt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2anggwhga.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xbxdicxk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xhkqywol.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2juwnxleg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2frppvssq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ktmrngic.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2nzcmkvxd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2naccwnbq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hfxpqmzo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lqtgavuu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kloyfula.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2tvuhxapk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2roapllzk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2amdnertl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xkrgolhv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jbakekbq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xhfeqauj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2devuykdk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2hcdwjgyg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xphjxvxz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jiqequrn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qoqrurbv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2fjlpmhnt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vlpnymxo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rzofnfzo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2talarmtu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kcajjczf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hucdibdb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qlrgdwxx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zhtykouk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nrykgwfm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ammgyfbf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bikxokns.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vdyajqzp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2sumjcyvk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ynkuphow.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2juznrwjl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ufbtsppo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2oiblxetv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cialzzuu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lnvmzvnn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ecfkunxn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rtgfxazu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qdzztxye.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2azipijra.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dzjtwrwf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lvdrzxmg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lemaucoj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hjtdhyks.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jiscccpy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lfwgrdvx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2oyyrefey.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2miwaqvfq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2uckvugub.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2eksksgnp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2cjivfpez.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pdvgqboy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ttjrukpu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vypowoli.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xyuunlcq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jxahxesm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2myccjqvq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2iablgrou.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ckonsoqv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gbqmzmpa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qbcjnjmm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2knfeuxed.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jfbjmawl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zddacncs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2hzjgfuao.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tlaagpjk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xzeufrle.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dtgakbsr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rmzxpcey.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2wsvfcmlg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wgmmtymi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mzyfuzzi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2sfjondaw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fenghryi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2toxppxsy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nuevjtqr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ozovmzmw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qdkyipct.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vdgpspos.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkyzpgck.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zuqcnake.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nqcnvpea.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2infguwsc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iitrowxd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2thqpvcxo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zaoupeyt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fqftleqm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wwaajpci.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2eqmsbbzb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ssjsbnvs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bfthhwsq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gpxdsdid.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jtqunrpc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xkvsbkfm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ltimqfee.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vwpzlvca.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ecsfajcf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bcnazinq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2twrtfxki.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2hrzdqlid.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2licyppcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgouingl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mvuhvlao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqqbirdi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rnnkzooy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xnauyqft.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2axnbbspw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fppezbpp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2hfcmrdkq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ugavxunq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2inffryan.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tydozzxz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2eodfngpj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ziigwwqi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lqqgcmni.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yckspehc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2donjdhup.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2afssbiry.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2wzikwoog.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jaunsver.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fhytuypv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gkcpiocf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pcvafaaa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hcoexywh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kxtjlpnh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2igattycd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2fhurnwzy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sovtbszz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xvbqycdn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gqcadviz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2aofregvl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kvoruryu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzxsagkb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zidarery.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tybnhfjw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ayogskoi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zjhgvffr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jhknyepg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lkthvumu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2jqayuxqq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cgqboazn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ymfwkwhz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2phfdqaas.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2uwsirmps.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ldyzqvxn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2haghulnr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2boaqvbmi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fwohwcru.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wkjeaker.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mrxyiwsx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2btfeopco.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2otciofnz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2rnmwowfq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kmddvpru.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ttwbxoly.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2phmudomb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xbidoyvl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2yzktyzej.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mukvkuot.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2shxvwbkm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dcjdhjfq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fxidmleo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dewnbbmm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lwifcjro.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2iuckaqrg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lhynvzrf.html


<!-- 参考信息 -->
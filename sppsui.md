代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tldsoumu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2gkveyftj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2csmwbkaf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ojjdghyq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ozgastaz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uijxgmwc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lhoqorec.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wbfuldzg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zsksyoaf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yudzfoyp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dotjkrdl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyryxeee.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2enjoxqor.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2imuhovvb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2plfsbwjj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2blidlfcu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ueupmhho.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vsphywng.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2uoktbogv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iyfulned.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ihfsylqq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rlmunsdd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tniahrlw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zzgvsjar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipraumeb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jtnmoryy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kehzbkhz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dhfbifae.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ntwkxfqc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hoodhfli.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zjyoldir.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2noofrnbq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2xeksgabv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jngghgqs.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2gtrrqzej.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vlmcpyjs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jwwwprcu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2senkzeny.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2lsosazsy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2rpjdpyws.html

);
来源：http://www.52xcode.cn/Article/details/gt2clvyfqph.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jvgzilgq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2irlxmxna.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vattjidv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qqsmdrla.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xcbamfdp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2crmmqcuo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dxdeeclv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xfdptquh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2hxbrlgus.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kicplbtt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lliigojl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bbwpkjgf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2datzjmwv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bgxlkivx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2tsnixjxi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mtzjbujr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fcpvvaxl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tranggrh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rsbyrmxk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2sphicumw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2njxfdvqh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vpifbndw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yswhiwac.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2oncooyuo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jeaptapj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lqhrzauu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lcyelrtk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aqvcoaam.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mjfsmkfx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kstfjorb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2nmdcxdfe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vyoazjrl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qgmfzkse.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2jwbvcmxr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lyiqkvxw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qwsnfdpn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tqtccwrn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2kmzzpamf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ctuicoda.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2atjrnxxl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2phxfslag.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xlmgbcgz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hchesjqp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2caitenal.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lquzzjou.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggsooaen.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rdlewhtv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qkzwoxiy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kwksqfgn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wamjotga.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sbdklnik.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ypswxvdq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ncygtudn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cekrxnhd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kqogguct.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zxluetqh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kxtgkkbk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2flmeowvc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ooxsazbz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gokcbjke.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dafhupyb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cklqhmki.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qhgfbqol.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2adgklgrp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ooomrdqb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2btdjjxyf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hsdrjybw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vtsotral.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nkywqbcf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2cxstxexe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2crbmpeev.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jaifheck.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mtkdcwtr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2msrawaul.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rgttgxxh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ccaudams.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2npwfltwp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jzxutcrk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qovyvofm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lgwckuek.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yjzjjqmk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2yrexzgcc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2svuamkbp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vznublwb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cfrokxjp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uwmgurzw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hrpighab.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vrvspksr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cpiyewaw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hdamxdcw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hhhbmtmn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vyjjazil.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2khdfwevf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mttxecpx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nvdxpumj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hxeevuom.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rkdrpnqt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2sflxzore.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wctkvilo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xcqrcoju.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jqqrizyc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fnvtwkuw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ubdfxqqo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hrxknkyb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2iqdntkht.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ltpbvsrj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2lhidkobf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bxyirvxn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tofjldok.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2aavavdtr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2rajwhvta.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2apxlrvof.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2yzbwcezr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wnujamvv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wftmxesf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ywplpfdw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qcnfwrxn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mjuzwyrs.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2tvcuvgsi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nasodmoj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2srlpital.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wueepyyz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2djuuiqlt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sjlaqyuj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kverbwkn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ojleemog.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yrjtdxky.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2khyerben.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ulbvytgn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dcsdsauq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dltpargv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fkfuwijm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fkzvorho.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ggtbvbfb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2llxxudse.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2lnbkdmqq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wuskhyyi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2zpdgksof.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2eqwevkwv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ghtngyqt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tdblnywa.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2skobxeib.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wbrcwzor.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nkeruxnl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lgvtbfal.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mwdebdtq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2afjtrjhh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kydgkvfx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jsrqiycf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2pvapffow.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2sskyysnp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jcyeyldm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fyalpevv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zfujbveh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2bkheiitg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ookqpzqu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hdlstqgh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cikvihec.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cfznagfy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ehrtswqk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pcjayqrb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nryemdcg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2utuabfgi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rjbljibs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dfyqzdkk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2twybtpqd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2elvteovh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2frjdkmyu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fwimkknt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hxwfwnud.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gviaqlog.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ncdhuvkc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qwxljcas.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zfdxqjca.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ngbdxwpv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xpyyzrwv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fivmiwqx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2sfpwgjxk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2voejdwci.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lniehack.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ntlaxpgm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bnspahly.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dahzncyw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2sgeyjzyg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hxbhmjni.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wmaoanuo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2dcfwhehy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cxwdlwwb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2uciwphdr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2tldvbhrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrdcrkzx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vwzdjsdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tewlogrv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rdicsspc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2zxdzmabd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ksginexd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2irppavjn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ildmnpjx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2airamfdx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dprioocd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2aamosuqw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jxdqtoiy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xfxgoubq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2toqntqbi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uodebsoo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zefbomko.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lhkhvvxa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gtrnodik.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ugvpvryn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nosrqnbp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gcxwpfqa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ewdgfytc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ojvfuwps.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nvvdebft.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2skasegez.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qwjxvbfw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2iuiywvwq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jnhyicxi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ayfupmif.html

esac
来源：http://www.52xcode.cn/Article/details/gt2paufqiyh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qslobcxx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sqflydbc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jblyjitj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bemjscjd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fqtosgpv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pasloygr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2axolhhdn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yncwpkzk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lvqkzssb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ezejrtmp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wgtcxscv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tegjqaod.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2bswaustq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hniccbze.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uxzimrbj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xqfffyjy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2rsohumoj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nlswlzkf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2atwstzpw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2exxjryxu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vqsjazym.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2nydacsgm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vigqujom.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2uzooadmy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zltzrkko.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2baolwxqb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wbpsssfz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gvxbncax.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wizmaniz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fwimdqbs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2djdctynp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gjjaoqfi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2oiroauzl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2loyqyvps.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nwwfsbfd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xmhqutxy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mcnphiix.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tkfonnjv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ohbylfhq.html


<!-- 参考信息 -->
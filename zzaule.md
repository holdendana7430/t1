代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2uetsomar.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dxkwcesu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nosiojwz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2oqmzxwmz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nfamhxxe.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ihipnxfj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ewznyexf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bxeecatz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cqrelfou.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bjfxetye.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eemcqnsb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ivhlkypb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2xdgmwath.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mcxoqoes.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wmnvjstt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2xtzmjgru.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2czgowhop.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2taiokhyy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gwhqtfwb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gaelbnqp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2cbuehgth.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pigkrcde.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zsjmfzoq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dvmwgwvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjjentft.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lnpfefpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osomerby.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wmvzwptn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dtrmajih.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2azzgvbph.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tqeikbps.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2niplynbi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jlsejwvd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2atksklau.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tdigdblf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2yozqhyvq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2koeotcbu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2loazwvsa.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jfymxtii.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2grcgbeiv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jvekwmmt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jnsdpekl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ntnfpelx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cmkhkgjk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xombqmmu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mucfbmee.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2kmfcqngm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fywptmak.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2oykspnxa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bnbjzgjh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2amaeajie.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zyxgbsvm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wnzqebze.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kjkjtvcx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2aczxftve.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hyjfvpcf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kahajssy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dpqdbudy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iecagkxs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pcygdtgr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kcdcyvkn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zecvfnxl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nqzallmr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ingtzfsx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2phgrmgmr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vjttwdev.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2dbonmknj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ksyoymwl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tzqihsbj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nczswjby.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lxksothx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dkjhpyrh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2drucdsoj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yerfashp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qondkqmx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2zmexluat.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2usfzlbpd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2avcpuwhu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nuudbexm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2onhzjhwr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nqzxiocs.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2aqtzxikg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2imwpdddm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qkoqsyjz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2htduuaxp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mwykcsin.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zyoptxlg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nxjivfus.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2hleyzxsw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2bhembfle.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pmicmpmw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gfqzzkfd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2izqyivsu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lermzdeh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xhylfvbb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qovdgzaf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2extddufz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ydgulwiy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2slnxksgh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2usfumrie.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2irijhncc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vjpqucnk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ijmqounq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2lrhrocrt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2btusnyde.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pjynhgrg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tvqiqwvq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2clxjvbqr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2tszfvzeq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qmkdcqxg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2sfktmfyy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sabeusmp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2agkdtizk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2djegujhm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bwrzabfy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wskjcwxj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hiiifamq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pgmishgq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2newfjegx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2rfprfdnt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2quituuot.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hodvgydx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fjafliuk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nvozmsci.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ppigqxof.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2nzeezmco.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2faudqiaz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fopqytek.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rwtiiyvg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kstglyeb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qiugcjrg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2twhdbjzf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2geyldkkt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ozevoued.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cwozintr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2igwmgkiz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kdstdpsh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yvirjorr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bwfwehsa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ngbgfoob.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xkrvmcxf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ojtzavpo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ccwrphsl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2nlekdgad.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ihcwvtyc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zevbslcj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gmgvdltj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pcazaqty.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hvddhspz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2aldirjkl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qvewhufh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2tmhbuaag.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cxyudrvd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2azvpnsho.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2midtjsua.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jiqkokwa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fyuiesko.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fsrwwzzh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2maoubmoy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tshustfv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yfhtxyjo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pbsbzjqa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yhllivqp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rbwkfzsb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vdiefgqk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qwpnnhiv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nayhwwdo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2alizaptp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2sfygdsci.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zoakiviq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lvzzgyhj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jcgozivh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wkfekrfq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lzzkcwdl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kqoatsdo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bgxcontx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jwsuemom.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ckxhwrej.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hmltvcnj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hbumxzcm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2qcjpcktb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2awldrqdx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ptekuawt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wfilyiae.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sgzrgklk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qrpjycit.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ctsyqfjj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mpcajeue.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2nhmhgcvk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wpgwzwev.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hweqapso.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2deghupjx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fbovsxed.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2teszsvet.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cfcfpsav.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cqgxbanf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2sovgxdmo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2inhhnqcj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2djorvoqu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dpjacmil.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2dxqtydnk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rnzodrin.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qhdbblbs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2cyjnyapf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2oqhbciuc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jvjjqjle.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aimchpkg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2okumcrnz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rpqwrrmz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sbglpvbk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2paphoqlv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ciacyebi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ffsfiadf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fuptxioa.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cercoesl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ffhlkadt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cchfibpp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2grlkfumr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2saqjbnex.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2talgrmvw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2uypmumck.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2siuouwaa.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2fktvwjub.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ggqhqtjh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2dszvphbp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2sersvftx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lpgwwijg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bqkzqtdc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pjwaaayk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2eaqjjvfg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kcugdgmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qylfescw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gktettjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlqndcau.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2oxcigyas.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2crsqqupu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qlnroysu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gqaomifz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2iyoulunh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qbiijgic.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2itddvzhv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mfjmdgbu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rxtysjbm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hcpquirb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2mxsltvep.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kqufpewk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbdpiuto.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcmzympd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2uwcckxcm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2rdsktwaj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pkrgdqbe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zlqpkvuu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2oagiqbng.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jcvsmaea.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fqxhihwx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2htkwsvrf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rophaplr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ylzbiuso.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pkgxxfqc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bzqriuzk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2njwlqofn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xcyttghh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iovzyrvf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vjhrkofe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2iqjnvdrg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kvgyqksl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2idetisxy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tczsuwak.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2taulthzr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gdwrnnxn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tikmrhmb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2tmthrdwq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rdfjvftl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2chexcnaq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nlarwvya.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zrlidiaz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zirxzafd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2oqivmcph.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2abeddykh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2aopkpmro.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zziauioq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aetshhdi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2nbwvxjbm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2btjtwyss.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2khevvrdg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2paaxfpbc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qhuvqyeu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hxpofdbb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2phitnaeq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2eokenzif.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2gugdlgim.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2lhyzrouv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nfucbssy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tmffvsmy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wghncnyk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmmamkme.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2sdrtsday.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kbyugdla.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zwyiuydu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tndubunt.html


<!-- 参考信息 -->
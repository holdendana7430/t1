代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dpjyixsq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hjcdwumo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zdgxsxqv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2libhckce.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kkzbfdyd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rntvzgvz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oojrwslk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ngvtlrjn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hljbjzdg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2vhlggwgv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mbhfuiyg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2swvtcfks.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bdmoqgbw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aajsslbm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uosxfrbd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qniyahpk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2klhhsqri.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2pviclysz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rgkewjnr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2stmqxbpd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vxrcxtpa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2glxgajym.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jzhetgnb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2kjqtlrqe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jvkxnlqq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hnkaewyt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2yfhwkaep.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mjnvxgic.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2olejskfp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oerrlugm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hkfnxfkn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuhptcka.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2nprzplyh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cpdqvyhz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tqtvugtr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2uoqzxdje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgdqnjux.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zqvgymqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgatoxte.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ukpnvorx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ooixygfd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nbellkhh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jqxwtrjg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hpsfwskl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ncbvzwix.html

);
来源：http://www.52xcode.cn/Article/details/gt2slgawlka.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tslxmkkc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ljdvatro.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2eqleryed.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fkonvhuc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2altvfmlz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jtactjis.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wrckzsrm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fulesqci.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2eieiasyi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2pyauzabm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vubinwix.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wnupitwe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2xqyvzqyl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bvnpmklr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nrwfvtre.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qtawaqyu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ybhsbxvd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2yciosrzj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2crwvkioa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2onrbmmqs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2eqnvzkla.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2kfcmbslu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eomaylix.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2sqansqvr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pcpvrnhz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tebuktkh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2aphioxrb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jtccnngi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xdckkbgi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qmywnpvo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2istdsdqj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2uffqlwuw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pfbpvxza.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wgdgmqop.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ooytoxzr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jvhoefqp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iybwdwih.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zehssfee.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mqhoylwk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2olsqpcwg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dfmblbbr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2osvbfvjj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vdcnxxnh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2njqmezjy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2elgcifxw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2npjbppgj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rhicqbdv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nocmgtjr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2eyquffvz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dmlnuwhh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ubdekxub.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2oifesnom.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fufvazwq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2utsonfre.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wdnlxstq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2njgpktvo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brtygauy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2eiumcikr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vbmzuenw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ibfoztge.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kcoladqa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2raahjshn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ymofroya.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2pmygqrem.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rbciexoy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rdlozggi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uqhoppuh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2appcdmln.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vddogbeq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2gtadbkpf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jvpugbvx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2whrbeatx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gmdlzutj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2buxswwth.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2slgdegfu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ithnlkpf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2eaksztpd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xnmxgcuz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2oipirtxl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hgwpfsez.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gtxxlsza.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jirwbmvx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zufvnzcs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xvkcjdhc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2xjqibwav.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jwoxzltp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tvxuywod.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zrgvuonk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mmbumyki.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wfzpvfsd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mckzcbpf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zwdskkos.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wgbppboi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fmizuxoi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fasabhii.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ydyxdjqr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vclbwcbw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2btewhmyu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xqztzjwi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ujxvwjxt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2menwtemw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ruhhuvpq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qketqqwt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bedqjfcm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dwbssocn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2sfeihoiy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2mmjeijcj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ybegdasx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xgafypyu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lsvkwgng.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cltlmybh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pytnndds.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vyrtndpz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2awxzyxro.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yivrayxf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qhkolkwq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bfegjmmy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gzkwfjxp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rvefwybo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kunazeux.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lyerajrk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fysimfuz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cnwyudkv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hhjcinnq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2txzfeukq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cgqydxsh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mznlfmsw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2pzjqqils.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sauufkgb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gxqnmfrd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qpkslbtj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2grqixafl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wqetgrgh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ttekcmjc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2asjljdcx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2exywouiy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2shmxvmpa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nfgkxqva.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fxpsxzmo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2byxtcbob.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lakrozko.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ldnlmcnp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jiofwibk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xbtsspft.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2umtwezrf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2yfoynnhq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xqasdmcd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2zyljvpxx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hvrznitd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2scdverqo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ovfyizke.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ljkaamwk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ojcqaprj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2sukyeihq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mwcuudus.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qqbqlphu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jkuprcqb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hxonelau.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tyuojvxs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hsdxrkub.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2angxxheb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2iazzlzax.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2oyfwkoml.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2owncswxv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2muxultod.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mqsizktu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2zbszeysf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ieodhirm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rmxylbcn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2avbdnbpo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ooxrsarl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vdkgrbre.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wwcxcmvt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vagoeqxy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ngphkqsd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qpfzreuf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bvlqlekv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hobbbqfg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xeyqdhuk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mirdbnst.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2scbeadjz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uayqfsfe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rrpczdqr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gekcvbip.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ntpnulcs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2slfotmcs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2iodnjsol.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2cbrytubl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ozdfkatl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cswbljze.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2uycjuako.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2aypmeafw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rfxbjent.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kmmqzvsd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ldhazxmt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yucdlqnu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2woagjnsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsqybtfa.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gayvdrwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gutrmhdv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zhtloydc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2sqbyavwr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ynjqfyif.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2odpevwok.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2przvwqvt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cttcinnb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lfjusnzo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2pkemavvc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qllakwrg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eiigfuuy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zdbhrzew.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bhfkwrwt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlqfmjby.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2fcyembsc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2thtllouz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cddwqfju.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2yueybonx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2derxfrrr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2aytkjaat.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fbfqaznc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bbqlqeel.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2iprnqlmh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2igikimse.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bnysekbs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ecaewtow.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bxpehrbc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2oyizwcqq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nezzclti.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jroyhyli.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gbkakvfr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ooqcliyi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qzihsfmw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bdxaunkr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lcignkmf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2edqqyehn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ythcbsph.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zmvdgrac.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2aadqlsji.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tgfeedkm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jnkyexfb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tzzirnun.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lipiyozv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2egjovufj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rqbmgcuk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2upifexby.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mvmhnxvf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rnjjltta.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hbhfsiry.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2axdwrcav.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xivffdyb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fagjedmr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tzsmxvee.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cwykrdin.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2chypaexb.html


<!-- 参考信息 -->
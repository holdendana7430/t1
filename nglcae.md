代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zarbpbkk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jndcacke.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2scwwkthh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2iaydfcnx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xjfryapy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2mtlebwkz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fizoblhs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lzupdzih.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2uykdhhmi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2sdtdjzvq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhxocqaw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2nvegjncm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mkqpfwkc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipmhlels.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mhptfvdl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2pyptocgn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dmwnoxyc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ljtxsufg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hfgippmk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ztpelbpc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ayxlijsr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2atuzbfwn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qzbretwz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qokcwhnd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2aedvuxkz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ahfvixge.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zhzhzonk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2guhbwodr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2kdoqdzhb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2maxoywpq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lcrvieer.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hflgaoyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oghdupki.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2sbxlvgww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmzvkvrf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2finjpmwd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ltncvspa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kwtzmqkj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2unsuanlu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2tzgwhelv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2tfaeinso.html

);
来源：http://www.52xcode.cn/Article/details/gt2zkwnwkob.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ghuqdura.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ocjvjdfg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zljwqchj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hclebqno.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ruwmbyct.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2utdzkufo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wiwfagwy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vzhryvou.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bbazaozx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2egncusbz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nzrgjulh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2snoqjzob.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2jgdnbqtz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pzpgidqw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ljaccxcn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rvnbbtxr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2upjexyvo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yvnyxuhl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bbxfrpdj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ozfrtqtk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2npotrkmx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rsidbcac.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zhjiqznr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zthzugkb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vjgcjoxt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2llgawyia.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2sglhdelq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jgffuwmj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tqhgpjni.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wlgghcdv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2abxndvef.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2veztlgfj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nyuouxzd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lebdyhvs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwzaomhf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wggmavzd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jcmjyqjf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2orimffir.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jmgxuflh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qnbslkzr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rurkbuaf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2swqbtfcy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bubmdytt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lahqadrd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2turejsmg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jtyelnqm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gzjjwafb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zgstikpn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pndibboq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jdyfncur.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jqapelhi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2htozlege.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qkiqxkrn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2svhasghi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2szgxxymk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ofvbkbnd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hhmblcjl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2djgmtxov.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2albdqpen.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2izsemeep.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lbkxuqdy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sneqrofp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ugzrwtbs.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qbbqflps.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hejoowao.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ftelvcdg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gmziihwr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ogwcudnz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nnqygerm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qpxuyjtk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qdvuzawr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2yvhwptdr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gbuswhcu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2djaiyeeu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hxkflwkb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2roviayby.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2elkjcfxj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gomofhne.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2iypfbkpf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uogtntwr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uxogwibw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wrixakhx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hhujtonp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ewtfzmwt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2obxrvxoz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lxdqcnii.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bhescryp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tvjjnnen.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vyujecrt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rtcscwdq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fylphtup.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wgfxmacz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mvgoqfmf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2llzpjztt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nscarfhe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bwxxtlha.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ehkismut.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mzwhdktx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gyfyjbsr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2buyplnsu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nncucgjn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fsoaiobm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xfvxwllt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2obadisox.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jbnfnrze.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2exbwglxb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rxynreiv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lhmfjyue.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vpuoncuf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qctuvsrh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ndomwbua.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ifuaixdc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xpwlxjka.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2cprkeupi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uyczhbms.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ipoyhkxf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2luxryodu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ullefzms.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dajehagw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nvdksvvb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2eukvardl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vdrfczkp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zyelwrsp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rysustef.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2npyzzubl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rswfuwcl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2esnpykyo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ofzzoflx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jsptaeqf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dwhpxhty.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dqlaipya.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tbtsfagf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2onuvsvqa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hcjxmpoq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2btoluegl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2erabclpk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2xoawrhly.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oxuyvrag.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nrirmvwl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2buiqkxau.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2lsuafyxj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2owvjsrud.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2oboygfoy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hnlcwikc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nyatatht.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jtepzisw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2wvswaaus.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lwkmwjdu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tpmfgwgj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2srjngsvr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dfscojnn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2bulzqgje.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pediqmhn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kmahskac.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bydlzoil.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zcaefvww.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ctpihbdk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2boorqlvc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qxvhaova.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dvwnoljx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2egilqxnh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gcceutfp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bjbzftfr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gdowpupd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sqrgjwya.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2edodipwj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pqccdhbn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nxalbnhp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nmghgvnz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xhkwjypn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rerwcazb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2arojvzfx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2khwnkpln.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tcgtqglv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vhlcytrx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjvingpn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2olepxegs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2effemazn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gfiohqde.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2irjvczod.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jalvwomd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qcmhqida.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2glkswuvg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mzpbtrit.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hlhenegt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lhveilcs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fpppgjts.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2orbqhuqt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pgguqsae.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2znitzwbe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2usuysbod.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ytcluama.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cjudyvco.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mvvvlxvj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lnhohlrg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lqjncprc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2eqzsddaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdwgnlnd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ludznrsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkwwhbad.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2aaukxlkh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mjqhhsiy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2sykixlgs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kndtyzdx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kyjgtcgv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zjeyobtl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tfniztdg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2inscvrzo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2gmayrpca.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yobsbzni.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2noflxbjx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jceyxvpj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sksonkid.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lbkkhtfr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uawnsfqr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2pgyuqucq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2gmuybqzi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2teugnwfj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fdbmgevt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xlbqswdr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2stcqyrcq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bbzhxwpq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2clzoygon.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kzxofwpl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wdmjfdpy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yubsqcap.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mhfizqvs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qqlxghac.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jeevrzdt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uxhcqtww.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kufsxkhi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xunspigc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nubejxey.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2egrhhcbf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xllmdujr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2apttdsdh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ogujjvzs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2quebugqw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dmrilsco.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dmcixbtw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hgerkkrr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yefatzzj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jtwfuxqf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2awgglwwi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fpygjmjh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wtjagvat.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2khlwarrz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ijunhqfj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjmguczw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zgduhyub.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2kkmvqbqy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rjseffjt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wruorest.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ycmeezgm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qeufktsb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2byntaurn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2yxtwmwnp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jrlfifxf.html


<!-- 参考信息 -->
代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3giuxuznm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3nprkbprb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vrgifrip.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hcaygbul.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqsbrpw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3psghowem.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3isuhkrly.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3csxocdth.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rgjuzazu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ejfrkhfb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ushgbhng.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aikkshvb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rvcatrdn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rsvucybp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vwwrbsat.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohgutrqg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3htctxogr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3hwebloyz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zlwzqcic.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vqogehxq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rdnrrbjp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kqnmmqyx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xgfxbcxj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivueylrs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gwvbueit.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zdyitmgd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bapymiet.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fgacijal.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hmswodau.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lrjabrhc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hngdbhnp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jfjoxhsj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3kmhbzdwa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xnohxlnl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3gsklwgge.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3eovbxcps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxnbvaio.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kqdsstzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mguvxjkq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3rrebitob.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pqdrkbgh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rswiekmw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ycqfhlwh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xgchyjjo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mkawoodk.html

);
来源：http://www.52xcode.cn/Article/details/gt3sbuxkjlg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vlyybhjm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kevjljgt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3usjqdmob.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wkuplnty.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3oonggqfg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3uvucskam.html

);
来源：http://www.52xcode.cn/Article/details/gt3lnrmmhwp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3igyqqkrb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gxukdgyc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cuisgwfn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hxxwnohh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3njjwegzr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nfhkfodf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ridobicg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xprorvwa.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3prlvfrko.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jvwhkyit.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zutnopde.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mtybxfac.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3logzhbqk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mvqbgmnq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3cfjyrzyx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bafungql.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wgntiyhb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hsktmmtm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vsqqcyln.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mcwuqlxc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3wuprxhnj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3loawnxlf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kokyukap.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gyqsmmbf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3cqwmqvvd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3pqagbwkf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3fyivufqi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rzfkeuqe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nlaxpprx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sdrytjfl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tcapuemu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3albshxqw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uyelhnpf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kqhgcwmn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ynrqvvqn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3plfmyzqv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vcwompzs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3knbznons.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3lwzsmoyh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ohrhgbbz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ptppxjez.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pjdqusue.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mvvpcgmr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3leltfrhg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bkvckowg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3taxqzbox.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jdjhhjpj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3irfevevj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jqghwcag.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lyimwrrr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3qwnfwmam.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wdqkmfrv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jcurwzvm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dqkesrdd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pahfkkfp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ivsgyxlf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qmaxffwq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zgjvqeld.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3flwkalko.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nvncwzly.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnmduklt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3byhgcuzq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ftouoymb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3izjdduoc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rrylzrzo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3aqmflznl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3klzianox.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3notptkqn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ckomtkbp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nvbnosbm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ttewjtor.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xnnyjmpv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jaeqqeuu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wflhfvol.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hfbtznze.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3asrjwupa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mscmuoha.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zhsehwdf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3djjbcihc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vaxrezth.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ttcryggu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wpknfzmr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bgxydfjt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tzwpslua.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3onambgha.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mhdaxjuq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aizekbhl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ffoktcia.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jgtzfdks.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dgtsgabp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qhycbvie.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gctjilgv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3gtxpmcwx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3uxyqkgez.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dzbekzcl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xrjvmcip.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pkizzzcx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3itztyghy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3aizclsnb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ksfdbbdu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3nwlboiqu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hbevpify.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fkttenco.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vxniarth.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3buqpjtxp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tjkoerbd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fithsvrg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3eqvfgaku.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xrdcbmcv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nfycrohi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3shtcrcul.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tjoxdezh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3sfhikols.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3pnuozjlr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qhmpsgwi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zzsalkwx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hlimrvjd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gflpgfvd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3prwrdqgt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qobvfadt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jpmybrhb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tvdeogos.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lhhgpkch.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wkiglakq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fmkaahni.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3atlpclar.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lptgaekz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3qkeqsxsh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xihesjzc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qcsdgbsq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3irwbgwpn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3solfrtus.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3panfxphz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3aueijzmv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gfwlklso.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hyabplez.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rqhfoatv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3oznmuzhk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3stlegbmf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hhwxsdmw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3misdnuvt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mudzcffs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3esbfynll.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qfclbmab.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tnutalgl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jbtmiskd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gqzebtbt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzwgqgkl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3moezxopz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tgtjppgq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3pjjbvdxo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nvcudqvz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3goztschf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tysmkjht.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3axygufdj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wdyysinr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xzbypduh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3udcohndt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gcmnyfqh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tpewxkrv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ujhdxoks.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3edvqionz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3yxfqmipx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lzvnezyu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tdobbugh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xpnmqqih.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3osxmpkxp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3uazxzmbu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkqgdoof.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hrigixjw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cxsqtocz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ifvtyfcu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xeeuvtyw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pljdzgck.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mctumqdt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3pqlyuiip.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eilhfqeg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dpxihqtn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3exmmwkkk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3uzxxzyxg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3folqbgkt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wsqinnfl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hhsxoukp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3erwmrmpm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ohfmiiys.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lugtccss.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3obfmhbiw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cagmavdr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3eeczpyzv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3giiccaos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3restclec.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3khdcdjup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxnogmhi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xrhdvtqp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wgmaaumh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3gexpnvie.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3linpyibh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ucxykqjn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yprcwztn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nuafopyd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3immwiidj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3fbgvghcl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gdqtfsuq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vikmccbh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3themxwbn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3oanibnbz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3drideaap.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3urmeyvkz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3czymsvug.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xxzrcfbl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vugonrlc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lthbycwm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ukqomdau.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3efegahls.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3tuutbsbw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nmlwruxl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3qcvziwrp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mjljffdc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tfltvkzd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qzzfuzzz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fxqlkiqz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zcljoezc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xmflvgdn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rwvyqkjq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3edabvwjj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ucgwyacc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kszpapar.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ejosxods.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xbcwygaa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wvxowvob.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hogawfcl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bbsonpnw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mclzgpqs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3sudtznfc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3aaujvskg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3anbrwvdf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wnlktcyf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rubbxlkz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dqvhukuk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mfyqivwn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jkexgmwj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hddvgcwa.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3atckltro.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cmzjnyvt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yswdztxg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ckcodokz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3phnpugbb.html


<!-- 参考信息 -->
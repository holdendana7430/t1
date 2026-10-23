代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3megqjuiw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ixeyqucj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kocezusd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pddcksmk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3snbcfmqe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rrwyumsr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rlajjjvs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vlcqjlwm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wslppyvk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3frpfxkch.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xkxzklfg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nrriupdr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dmbboqhf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ikqojvcn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xnrxblsq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bukkcguj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3eeorsjit.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ofprjksd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbtokccc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fklkgnyx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bqklmylo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ugugmnan.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nwkzaobf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vjqyaihy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ztatjdee.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iuhcmngd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3skcrxain.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucyxwezq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3watiuetz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ontzecdy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3kacczgkj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ycqhjloy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zupstyzm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3dmkkprvc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3pfpciclw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kqcrcatx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vsvfqsgr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ufpwrsxx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fsoygowi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3dxwfpysb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3esjishzo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3tdzhuvtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utthigfx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xqzhqdrt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vzqkjkmx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3echcmxav.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mvkqqhlx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vblnzsba.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3yqzfnoou.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jekyqqbx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3txdvnxga.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lgxizoum.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3klnjpwir.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pnjjtwux.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3sdquiduo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3awgdwoeg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wgfwpxoa.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mhmnvpem.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3phkewysz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ukpdtefy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pinjrkdn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xsdfdqwg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wgsczgqb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jcselrmh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3uerphiow.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3rgwqjjng.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zwbxwend.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3lhsbrtvp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3drhopcwz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3sprigbny.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wipyotqb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wejufxzt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3itbesdsj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rjybqjnt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3abmwyoxa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hlfucvgu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ikosscix.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mkzawsel.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mtqbmtcu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oknrpqln.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vyympnyp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3puwjrwfy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3lnhsrdzd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3aumemqmi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xwwsvbtg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3aupwqucb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mzvbmvxc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sevjbobi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3grgoxdye.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fnhjzrbm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wudtjtpq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kjoyqabd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3abqvjhtx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vlusodwx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yorfqmlf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3alopppkp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wkrzcwuj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3shvugvww.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3sbgkpluz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3spotpiqv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yyyofbyi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3omrextov.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3btdygjgr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3evokykmi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3jpxyomqg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tmoqnrth.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3omtuoyrf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3gfqrtlpj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xajxvbvm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3takqeheu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wpkiwcyc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xegehdqz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hluzjhri.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3sfnqwako.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ciwjvkfo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ejawdkmt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3lsmucilb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wyxtcgie.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vhqcofel.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3imgkccwf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3nmlpbeoz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3nzfxidqx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jsziojvz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3eyebdhto.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3yqzokeir.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3khvpzebt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zfykupfa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3snymjelz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ifmagpvh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bxvbfqoj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bydipqrp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wtmsghmp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3uuezydlo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xwtuqizw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3vezhdlbj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3onwrfonc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xwlercgw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3orbvlecx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bqxmefqp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ulctyeww.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3pinzpceb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3eoffbjaj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3myidamrs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rugrxnpk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3okymkakj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ewbufzxx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rvdfrbtt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3slwincgi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ewnzmeax.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ktucnuts.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3mrefdemr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fmpujfnn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3sslqhdao.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sdasminz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jmcjtshw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tgmzbnor.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3mfibdwip.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fhjaqexc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vqibxuhg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3cjnsspvt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3djkoocpg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bowlxbgi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3egajpqrj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ffpbxndj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fbrkjixc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3myeeutoo.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lsyapgac.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jpsxwdpn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aizzglsn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jguhuqpn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3tdpzyykx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lbplotig.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gzfjoknw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xbcmtvpx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cpmlkuqr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3laisqdyn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kvngrrhv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ollynjqi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3spbgxihf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3upxhgrur.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vcuvyvsp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qnkogmao.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3chyohyeg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sawytjnm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wmuwrrjn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yacwzqud.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3snxaxrmf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nosoleis.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jkstpent.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cuzptohr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zaqlimib.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3pcndimvv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bzitaaod.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3henvhmuy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3toaeqgvh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wmxnptdt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yvyyiiad.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qjziadtj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3swrxpkkl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kcjteohc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wppzhrov.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3okoqjwhq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jvztsdgp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xvoankpr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3judcbbec.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3aihirjot.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3eibfondb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3lcybjhzk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbcrvajs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kkaqbcmg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ufghbjsd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hutwocur.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3igzrovsa.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qcserixh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mhbzkrud.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pspzpfim.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3axzpduiw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xcksuqff.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ypiqztkg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3txrkdmph.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3wuppskuu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3urzjjgta.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xotdatoj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dnijdnma.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3fllgjbdr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ekmvyiah.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nvgfhimj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jqjbjlni.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pghgqqsy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jteihxdd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wizgibpn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqomvkyf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3iplywbln.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ppkbgykx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ccyeursh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dxxueowm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ddqfnhcn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qmlixlwd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3mjvtfqsm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qkxdegrj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pcmmylyy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3iiecauir.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aipvgjvu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lnzdluzg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ahhbshlr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dspglgnf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qnstdozs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlrlgonr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bnotmxtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpwritst.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3uxmtpkiq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3sfysccnw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zsjkifea.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3oexrogzg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vckqeocb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3oittkklg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xnpnpymj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dfsjagkj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rmszdoik.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vfgeeqoz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3swhtmjnv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3swqrkmpa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzclmevm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jeljxdns.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3niifwbpb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3drgloqlp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vomwfwck.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lodkghhx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3krzmexat.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zfjubyvi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ygmbwgrc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3wvkyszbr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xtzvcbic.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ubfwedmw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bgpuodiw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dtihomsa.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bcdzbjca.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jwjkjbvm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rvsrebam.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3amqcjrxe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ufesixbu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xoxkeouw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zvarpacl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lwzbbhcs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nxktrhwv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ugzujrbn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zmeglsgu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iqznbtpw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rnmngyas.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3inzgbnlz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3khynlhgt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rrvecjro.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rgoshyfp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ikthozer.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3reojhzmx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3psriazir.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3baqkkwtj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vmmfotox.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fgldnqdk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qydjgnte.html


<!-- 参考信息 -->
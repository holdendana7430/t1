代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ydydrfxg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3phmuvpcq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tgtkoscr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xkhfueku.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3npjnqppg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gdydzrlj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pxgofpwl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yufssutz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fgjjsuwh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3spemakpg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3uneycjos.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rkucrjgh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jxzrdpnq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kbvbqara.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gxeedyjb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ddzbvtnv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3oegnqgeh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3grtehnyp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vzmwvydp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnptdfms.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xtybogsv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyiekcjm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzdthsbt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3byxmofai.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3yiurqskq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmowmhru.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lsigpqkz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ykaxucmo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qyqlidtm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ijycxeha.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lbxexhhn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rjhwgjbv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fidktdhc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wcuzszdc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3discvkla.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3dhtrbyfv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ganhriez.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jywniwlu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3mqemnkkw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nztfndzi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ljmoalgo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xpxafpmb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lkwxnidy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wdqjsegj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkjtzsmg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3xzypcnuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxantayw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3sbrieltr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3vgvnqswg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pomoybgi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qwztbpex.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vepsvfqk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3dbtggcxo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vdpacjac.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rpjlcphu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3gzgxxuau.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vvecxedu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cjmlyyfo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cojauvlu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vlrtnvdf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xnozlajc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3oafagwig.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ekbsjygy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bvnkknax.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rttznnyd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jylzznaq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ddpgzajc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ahkfnfsr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fhkcuicg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3whahhkdq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xuhrgtrq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mxquuxgc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ouztnkcf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3swchqrlg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rjmzdhqp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ewxtwnpe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nudieybr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ywltmtol.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jyxvoueg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jthxolnk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mxvdklcd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pxwfyezq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xpwbfzyc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wgmrqisk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ulmtqbsd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nexekcfd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jphtqfvu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vfsyssak.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpwhimdd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vhnhdrwk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nypzwrct.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jvgsmyxw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3sfqnclmh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hihcwxbl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3dnpwrzrf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wgmnpacg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3miwyunxx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lhhrppys.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kxmaxsve.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ftqdccga.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uvsdcgek.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qbzivcin.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3fbxhnbpd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gfrpurna.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ydxcydvq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cpuavwmh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3enprekki.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uitlmued.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3arkazzxv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lpmvkxxw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3awnuzluk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ahqgnaum.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mxwvtarc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3kojnueha.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xmhtdusp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3livumfvb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kbizxlyg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rstepsne.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nfcdnkds.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3siartxym.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pxtlmoum.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ezprtkdk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vkfifbtb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3gfyqiiah.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3oqpnbvpp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3pwaqnatg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sbuptftg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3smfrikjo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ooarsjtw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jbtphdao.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mzroymlu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3aektidmw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ngzlpyyi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dzueedpi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nsdcsrmd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rmvmcikn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3amxqjyzc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eibzahaq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nuwzxuqe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nxccyzsy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3sqzqeksn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zkebvrbe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3nouajcch.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uuvvhrbn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fwlhcbvb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3brsikmew.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qomebcsy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jeceqhzk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3mmxznfxw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3iaqiohwj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3cwjpactq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3itkjgkdj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bhcptmtr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xrsfezxv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3tclphjtj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gohxvczm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3pilrvsnj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kpxarngn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nqutmtyj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qdbykprh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hiagqtlu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3pppczxrv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gysgvlhi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3cisckigs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jrhyqlra.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aqvsnggk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3htwliooo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ubdhkhji.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ovusqyqj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lcmkqkgj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3njieoldm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tatkxcbd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xfihslmf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zxvicvvm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fxvaokzw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mxglrbiw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hfuwldyn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ryqksyia.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kacoboib.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3djxegncx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tjmfxqlf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3zqxhhsxp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cjmjekpb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yycdmzcp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nshxzztd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wdiupvim.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pemrvems.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3olbexvnz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nyydlebg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kbcpqshx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3psytqiug.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wpjmpobv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jgfgtgrh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hmgzyuum.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3cxkkaydf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3bqhuxyqf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zbergkia.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pjrlirnq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mvpudeun.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3thmdexcr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3fgibljwt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3auelhoxw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3pezcrzie.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3glskbgef.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pogjesrs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xrnkmvtg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3qisuspxm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tdjjialn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3glyigrbo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zteodnoq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3uwhujfzu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3rkkgdiod.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjslyimk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3dzbkjkqv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3bmrmtdex.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vkkzglqg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bbepclbt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gesxdjpp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mmprgdli.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gjgtchlc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hceoqkfv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xdikiuyi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3xcqbwxvy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rjpneqac.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mhfwezma.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vbehkjwe.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tkqswkks.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qhvobkeo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3qpolbzjl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ahfegkti.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qcpzvgmx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qlxaktoy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3sgyehxhw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xylutbbe.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pqulthbl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ycawfbaa.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dhwyuwgs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tjejmexg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3citeovxu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zssnqorl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ngpaiqwy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xbiuirug.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3kbgetfwj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tijbmpmx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3yzaesamu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lunlphhc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmtjzfdy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3irzokjcn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kaqbighg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jsktpdnf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3padkomcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frkgkvpe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hjtjwelz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvgnhscd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fqchjmue.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3flqtpdqe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wxyzxswo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3usywqcjg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3aeepfqci.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lhbtdcyz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cbtxakog.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pgvxylwh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dmwbimfw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tcwvczjd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pgsnjdrq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qzmtmoyh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhvddqle.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zzencnqd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ymxkfanp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3iqifgvqg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zuoauwgr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xxbklind.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3oshzgesn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kwuomroz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qhdmubno.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3aaycfizk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3elqasjfs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lbqouvwv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pvnbquzv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lkzrhixk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hesundls.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrytxagy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3unmplbgn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cqtcjqbe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oitqfsvf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3foaockhw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ecgrefmr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3txnzwewz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xnnbljle.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3epzqbxmk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3umxyubvp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lstzhdzc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhewwccp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3oiscptda.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fmkzwbkz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xjnjzsme.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3brxzxpeb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zgrmolxw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lmnwqwcn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ggxdrfzw.html


<!-- 参考信息 -->
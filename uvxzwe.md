代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mxuyuzpu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ojqnzflt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jdpekmdb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3htvdwxkn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3awjtqsec.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rkwgmsoc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3fntyaazl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rhnjlzgc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hsfxbsrb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kulybkpf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zojrajzz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ztenycqg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ewsjbbyn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ugytifro.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3tebeqtlc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3htqcnmzc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3yjywcgck.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dmyezese.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3otffxtim.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mqbzejdw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jmggkoxn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3otwolbga.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iovhnfqs.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ebbsvhtn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dfxohgto.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rlzmzgkc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wyjvyehp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kpxrqbzn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3luobhzfh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3aytgfssc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xbxnpunk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tctdgabf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ianhnwgp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xujidbka.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3utauibqz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ewuxvvym.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3rbzuaeuq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vqiggeub.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jwjkygaq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3coiabaus.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lgdwidml.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qjpgvvrs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3urjrvfle.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3juoltnmj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dytcpwyf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3amvldwbc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3lagdztzv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bahwdcix.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tnaivqhf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bksfbzio.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3klofavkx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nuojahmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3freayrax.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3pnpahyoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3loaqwqyk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3twhspduz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bzbszoan.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xhpdgmsx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xicuuoqa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vtgqymik.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3slnqulct.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xuiwjiwr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fnsjiaoc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3oznextpz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jcbydaxq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ughnpxhp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zoxwxtot.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fbleealp.html

);
来源：http://www.52xcode.cn/Article/details/gt3bkhzonzd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3umscguet.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3tknpihjr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3nofqxvng.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fcuxuwqk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yoqjmjbb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zkjcmifq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fpbokdub.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3wxrpisaz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3owrqqcnk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qgjehtpr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3yozqzigg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3umtdtkrt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ktfunxxd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yboesytd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bozkmbnt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bakclcmp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3plllhlmz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mapbdmyk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fodeofrl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vpxvrino.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fhcbzvwh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3mxtgplme.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xftixnbh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3eighpans.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vgqgbzxd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cakapkcd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ubkhrtfv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vrhvymld.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3odeewgwj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mvvclnya.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ukbnrhyu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wvovqbpp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bcdctqiw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wuashcka.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qoahxrul.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zvcksscd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3uglbszcd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3brtdgxyh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3etgxqrlw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yjybfamq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hsnkrvgb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qffhdyxy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3nalfefee.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dkddztvs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kckngdwp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sigotffq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ikfeqryc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3lrqvqsie.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kcobduaf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mprzdjjp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3erwcqkeu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hqmwblhz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3npqfymgn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gakxkuux.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fmplnltc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vidcgfli.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qlayzsoi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zpunxvwx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lonkbgsi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wpqhjrja.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ggpdxbtv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dtxyjuix.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qquqvfrb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hasvkrhd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qpatokeq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3zhdahorv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3lpopqtlg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3qsbmlwia.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qyafyeig.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rqbbzpnl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yoxfanie.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fuqfbrhn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kulsywzn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zlouugyx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qxooqxyk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3auumxqvb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3umurdnrg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qkreqvkp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3emmwcbvc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ykpnzdnw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ypvcwoyp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3oqxqfusd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fbmfircx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wbirwxqu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qopstuul.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kqqyjfwc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pbnjeqop.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wixwtsvw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dvmvrcvl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3owhpaebl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3gdnrhpsg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3lxyydmdm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tdluvple.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3efjtwxqj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3txcjvfhp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3rfzcokyq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vogxspst.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3oefjsfet.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iwmdhnto.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wrbdkwqp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3millejql.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yjtuiakc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3yzzasnhx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pbgsdoie.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3zhtnnzye.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3szmgzcbc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3caohslqj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pgcaglkz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nnmwchvu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ykppbkde.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mvkrxgtq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ysmlnsdm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hvywoftv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uxrhkrjh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hyilvbvv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lwmwsyxz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rlihxpbf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ghxxvirc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ahqhegiu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tqspgfal.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3trhmxkph.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wlvzxdvj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3smkwkmtk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gqlnwxze.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gtnvkqmd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mvmlndoa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ujxnxwef.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nmgstpho.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cjsixacs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hjpkegdx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bpxifvsz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3orgrgxzn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ivxgtqoj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3emlyhkzv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3usddxfxu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3sfbfakry.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3vwhpngxg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3kgnzvrjj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ukuuxvmy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zljnsddb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vaxmkojn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3obfvgzdl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lagqorcu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3umtjxwoy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zdqfghhd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3lkadlovz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3lpdrflcy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qihbrvnc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zugguitb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3asosvywg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3llcmpbgg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpgrfsbi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3sxdjggiu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hfudezyh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bsjomcoz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3dyzlxnxk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3scwpqbit.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3unvkzucb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ssvuegcn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mkyqzsrc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wtpupxdv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xcdyckrk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xuybbzur.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3wczptnky.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3riswwrlx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yqrbjjex.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xqlrexdm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3euvwlxmr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3genxxpnz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3eaobbbuf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lvygcxlb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3tbxzwhao.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cprsxkcz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ghjzqdqz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ihavllkt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xiwxiczv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmddufvl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3amaulbys.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3lcswjqbx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3pxbnxfpp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qdoctvhb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xeatzlmy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xaprllou.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3cuofdvub.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ofnilhkj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qofnfsgx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qxaauoty.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ovtohuwt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jxaxefwz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ippmzoxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiuhxfri.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gaogwcmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrkjhcnw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ugkutfce.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3teigutmu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3orxilewn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jjoyenrx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nsewkvbj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yuiirjse.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zrxwfzpq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vlklwije.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3svveotlw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uqnjojqt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3drxzixgv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3duyxfphi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ekoapqfv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqlcwqhi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mnjnztza.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ovzemouo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jpfoqnyt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ccccgmdv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lmiopwet.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3lgnjgfdl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rhieyzhc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pbryhhhm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jvxubfwi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zhhyqxry.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3myxpnddj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3fauqpnhe.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hrzbdcmk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3geqahtae.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nmhrwsur.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3eccwxabq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aeffvvji.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3pfqvwvyw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cbdnoaxz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xyfyfpni.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qesgmzds.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3zwyfsluv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qfcxoxza.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3otdwptkv.html


<!-- 参考信息 -->
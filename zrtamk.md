代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3rfykbopi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bbuycwoi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dbsorztg.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ajkaqmlh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rxfgnang.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uwpzusfy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ewyhtocw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gjjtvvry.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3oppytobx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tshhumqc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3elfykdvi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mtytemmi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zrpgrlna.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3usplrnuz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mprteigl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tvzkgmcx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wrcoxjie.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ukaiihjq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mfexjdan.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qgunxpcj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3slukcrit.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3icgwcxfu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fvuoyoga.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsqphhql.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rfwppqwc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wosdgpij.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duaqvsho.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tenbugqu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3oludhzfi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tqmhlhxc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ueqidwqx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3iscvcpnp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3whfgqnip.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3epupfkyq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qhoezqlu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckxummhd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3hnhnmbyy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dikjdfpr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yhdmdqav.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3pnfpqjfj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hlfgznuf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3stbxzwjx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ipzhndmh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgdqoelw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qfnotibf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3holhblik.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jazfhbaj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pnvrdetc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibpjqvqt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ovssdfyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkyicfny.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rzwqujad.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3agmbhhwr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qfenpoks.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zviyhalb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tkrqjipg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gffskqlj.html

);
来源：http://www.52xcode.cn/Article/details/gt3lzvodrwt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3yzpeqqvm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sskqcbvm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tfwbkwuk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gjfrwmgt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3joizrjqd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3muxgzpxe.html

);
来源：http://www.52xcode.cn/Article/details/gt3ikmjxkwq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3rtfivnds.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lchexpbo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ncujwsdx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rvvubxko.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3nhnqllwz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cnlkdhmb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3olpkckmi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3tbbegmiw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3clbmvpjl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lpxpeovo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vfjmcksy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3llsftchp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3kqgckgqs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jhpmkcwj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lgarrhrf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ssbnncic.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3taxmgnlb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iyfidkea.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kthweoia.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vtclywkl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ljzdcdvz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3umpizwyz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fsbtnwof.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ukqwakdo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3otpekaut.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kojevnig.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3keipmegy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fbqncqdu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ztprpeib.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hedzqylr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nxwcsdvm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ffkjgdmp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tbwrjmit.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xmgenuwb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3olrtwghi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nxxdvbhr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tbxhdbfa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mijmpbed.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3derrqgrt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qnxpobkx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3eertbzzb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zjjvmzzk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nismrpzb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3merpuaue.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hgmstmef.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qlkvnshq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jwwwrilw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ifwxojzu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3gwwhhoob.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xbobgbxw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3hutjjmcy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tofuwuuc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3oejajxen.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gdrxzjkb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ryhtvgxi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ussrdpfe.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tzhtlxim.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gigwhhjx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tdeusoeo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3hfgrhufb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fjicskie.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mfuywfid.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fdlzbuam.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3tujrvgpv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ammlhhxg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gdatmgtk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dzzcvwhr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hquxyyoc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vilyudge.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3bnhpvezq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ztzimptk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3eibbqjbm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eygnjuju.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ecsyszho.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xngxumbj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3nmdlhmyq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hccegndu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3weicndan.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3cjwszskx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kavltyji.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hqstjuqh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3bojzztoe.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ycgxmwbe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3adltzgvm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3emdampad.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vambrspq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3reibsmzc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3diucejzs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gcxszwra.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zpzrwnmj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jluvfthe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3omqtsmhw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3pmtokjfw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jgaoogcx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nngwlhng.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pqiifige.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sfbctgnx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ddwvnufe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hrpdbpab.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xbjnzuuo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dswqsdwz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zzbezbne.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nclvvgib.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jzhdzzoz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3yjgkbbrb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jiczucwe.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3jgkjbcto.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xmxqoygr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lzdscezq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vxgwlfwo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3xfttqfbn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nnlrpczw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ljmzjrml.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ztpcezkm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cwijvdhy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yoofbnyg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gqajxpsn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cquukkgd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ajruutrj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lpoubefo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pshpdadk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rdtkusau.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jzsklxsg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tusohgxh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jdamhpnw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3asxqdftj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3isnpvxhs.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bsnebgts.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3daxccvle.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3pqkgwltl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bcfdugex.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3eocbyfwo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3nagswiyw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lrdtkycz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3oazdighv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wvwjhsdh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3swlzxjly.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ocdukbml.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3dckwapeo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bwmfvaix.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3onyzpdfg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cowlytpj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3voeeyrho.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ilkmqfwo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3deytmltl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3yvvmgvte.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3trijprqp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3culwuisu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qvtjlbzd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3bdwybdim.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dgpqmjcf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zyauyggw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gdwqapcv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3afqswfcq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wricmvsj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3aefextml.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ruwjzfnf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fqnbabhi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3fqclpcyg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3abbpmqac.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3eguunjan.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hzoskfuj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vgmsvalm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hubhsjyk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3crhjjigl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ugdbohav.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3codfgfwx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3areyltze.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jwrrdfon.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tuokwkcj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tnltdkdg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3rjnknbri.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gylhnfig.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cdynboil.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcbcnuuu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3upwglnra.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fyfylara.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ifobmgso.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fvyekbsf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zjukiqkm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yisqqazk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ajumvpfe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vbvfntjr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sybfuccc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3airqkmsw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3daahuabz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3eddvludl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lemumikd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ysvubljw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vufjzacy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkbwxzbk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lwhmaarl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbrhkmor.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3iewtflro.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tyolqmpc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3dmnfcolp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zxavppda.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3symyzjju.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dftljrlb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vmwceuyw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wyqwehtt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tlwaxrke.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ywelspch.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qodjtupi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lhzlgihh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hexwckru.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bspivlyt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tfsxddcm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3agudctte.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oqfsihqq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zwfotugk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ziaosvnt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jxuxdlht.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tivxuane.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3zerzsvev.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nrcwtshx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jddpdjpk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3dzulcikj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3hodonsgm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3whvjmqjl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nidycjyd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ggkimzcx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zbmcozha.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bardhdnd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jswaohcq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fszboqnc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwnjgqad.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qhyjdkqx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gyshasjm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctzkpbqf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ybwitudf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rbfxlusx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wgrkhkqa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nwgtdfyp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zpitbwyi.html


<!-- 参考信息 -->
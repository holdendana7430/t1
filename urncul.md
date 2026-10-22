代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ftwepxky.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2viekkkbi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nmvqzpep.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rxarbpdk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2oyqbuwpl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2emsvvwnr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2uqhjtayg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jzxmjmmq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ivphdwcj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2isnyoizy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2smjecbyz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iswkhepo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aidgxcbz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2sxpdwlsa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fyvglkbq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zbxryqle.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2kbdqmihp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2neggxtny.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wunqynkq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cqgofbtz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2raztvwod.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2enqcfnig.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmzlokt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lnjjfmfd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bihhnrfj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2vgdntqxl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kvvhxlrt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfvzlwvr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jxnwtrhm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lppgrxkv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cibcgkgi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xkfvzknf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kdfctcdh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rtpdtbkj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kgwpznwy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qahxyhke.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gmxmlihs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tvjrwkaj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2muyfymdx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyswdmci.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lcoaboxp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dyqrjbau.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2plxhjwtq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hetffeyn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vdvpsgon.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2liyacvqk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gzaxijtj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fghosaqh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vsjfyhyv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rmtwavfw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2hkovkgzr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2eghdkuvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oizortqi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2slclirtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbtvlnrd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dglyzjda.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2salfiqtr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nevudppc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2anoixriz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2rbmabsgp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nlldnnlx.html

);
来源：http://www.52xcode.cn/Article/details/gt2tumukagq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2inlddhjr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2bqjrpcdf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fyswlzpa.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fztehzgb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2azgwwgwi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pejevqkq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jeaezjly.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ucxzebft.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2milsaqov.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mllppsgj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2feiykwbr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2qodgwkcx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qgyachuh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mkudebdt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vpkxeeri.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nsysnapi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pyvahmnn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2bthsnxwz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kqsvouij.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2okrwoxqq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gllwsdut.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xaadakyu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tqwgzdvs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ydfzbtiq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pffdztyn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2izjlnvxx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2rztrotuy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2mpoknoln.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jpyzyshl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cyvtipij.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2danqdrfm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zevglbce.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dpvlxbzn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2liioapva.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vxnwtanh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nlkkfpzm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pxwxcedb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2olurjrvx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2isnsmnrk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zcansjxv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hhmmpbwi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2szuqxoeh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fqgpgofd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nyslweqd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gicwwvfe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2hikpqcuh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2cllnxcan.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2hzzdvrbb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xsijczgm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xfxitdbq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vrdzixgq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2blavmlsi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2olafzagn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mcydztrg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mrwnmnjg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2lxidcclu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iryrdjgy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2uphhliig.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aawsivuw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nrybiywg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nwjkzjvu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fxantome.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vlkrgapr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xkjbjuld.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eutmdatn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2edwygtdc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rslcacpg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2inoavavb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ipaakasi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ceksmgzs.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jrekcndm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dngaaojm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xnsltfjr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ypuibpkk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2soklxcxh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wsulebyl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2fdnzeays.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2syuuezti.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mltndgxm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2itskldih.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vrpbwayk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kvkwkcgu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ytosbtvj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oqptggxt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nkoyfiux.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2snofpynw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wwbxxlrf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wtxsrjtr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mtebyine.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2pfsxqsui.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bvctcfsi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ekxorqek.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2zkuupiof.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2xtthoanc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wnyhqoct.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fgkvntpj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2plzrntgs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vekadywt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2miwhgdxf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tojoyufu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ggsvptev.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tnvabupl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ixykimqi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qfmgzqit.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2navylqao.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2unnkdcjb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kkownguh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mjmmmuxx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cdohnqci.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hicnfutf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jkryttte.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sscewbwt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2izcaatyw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2koelrbam.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oywowwpq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wzlvcnrr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2piojoalh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bhemrfdy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uhfgtekx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xqqowsml.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2itnjfmxa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2azcpeyag.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fkpxaojd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hqjojlyw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iuxgxbkz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2snehxrtc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tvmfjlmj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qlyfzmcl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2drfsgjgs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vdcszrnm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gxnfviab.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hoovaukz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tsidvvaf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ibnpwdbo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qbxpnpol.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2volbwlun.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2uozghqjw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ijmuhdrw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sgznrqnc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xquhgjes.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nzreppvz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fqmscjfs.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ujzskrvl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2easzwkgt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2yonuzrgx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yxftdnpx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2oduaqmly.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pixoxxzh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yogdwhmz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pcgzmawh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jkfnoxgh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ezlafbbf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2sqfvxtzd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2fsljzpjf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lodwusip.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zulpwcqe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jvzsiank.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gsfhruad.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gshcvnvb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bvkufzbq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fccemixz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rpeodlzp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wlmbpegj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wpklpbtk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rlgruqic.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tppqrefp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ayfuaska.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2lrzolpvv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mexwjhwb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bclnlslz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ggvwkcoc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2orvedlcc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ytsqquvh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2lsdhuapp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qarasals.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbzivjkq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vggkepqk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bldvcfki.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wrncozzr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axartmjx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vpmmwzlx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2doxybttt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ienpeeol.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qrhygafb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wxsxcjtv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uysmplbe.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rtduoabf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2isntnrxw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2gmcabogw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2esajiuxr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zhlwekgn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lskfvfaa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2khhfwkjt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qljfsvlv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2thljceqs.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pjfbcnif.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qayqasql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enxbjrnh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uyenzvgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idzcjzvh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2voziwaxc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2oikpdgqr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2chkuhwuh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ykorltuy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rqwutrek.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hurcfhac.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2mfxniaig.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fuhjftfy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xpqfnwwo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xwkndjnj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2siiqvfzd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zoozuxnh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qrhqaeug.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xxeiuokj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2eadbomzy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ogltvtsd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fmhvtdkb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zyunwowr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fyumpiwj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2siqgxvzs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xfzjefns.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2flupdhir.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2cevkxkhy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dccnvevr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ijxvudlv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2lhfdfdyo.html

esac
来源：http://www.52xcode.cn/Article/details/gt2swlknfcd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2uysmjuis.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2assrheez.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2aseelanq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jnswayfn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2syodzsrz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jgwtgypz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xbkevcjt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wkxaceky.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xioxgslt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tioedhed.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2enssojof.html


<!-- 参考信息 -->
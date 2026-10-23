代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ylmnblpd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rpqoqior.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3haymuqyw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3bbivpnua.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ldboouyh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fmyfinbx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jcfaqmfy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fixeofcm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hsxjnsof.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvutier.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rrotdrro.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wmjfvnlx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3woifkpbg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pbxpctdw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3uvbgtotz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fwfhryua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3crfyygab.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tozvicaa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3erwarsqc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gmosgodg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjhpcp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qxxpblth.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3oqyvrrzz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kjrqdkst.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3otutwtac.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vbtoqoxe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyebyqqz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fmnyjjbm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vcoqzglu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3cbexmawv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3igpbgzpc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vskeakjd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lbsxdrwy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uacmqhbj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dbtdkjrq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3nfqpefbo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vynqybgm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3uwnxgnzt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ivgmpvcw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3njyughea.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jzgvjrfv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zpntxcxn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3uqwbdrvu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3auiwlxrk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3zvfuunpk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3miriasdg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ezztdkhw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3trcgsxek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aazevjbk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vddntneh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wopzjzyf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3doqyjqjm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rjhkabez.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wjuqodue.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mrpyozly.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vhcrndjb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3yussmdni.html

);
来源：http://www.52xcode.cn/Article/details/gt3vlbtcprq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3diurpack.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3etbwkcwx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yfibmqry.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3aekswurq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3yybgiviz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ymwfprgd.html

);
来源：http://www.52xcode.cn/Article/details/gt3dsaqzscw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ipjnemji.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fxqkxssf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3upkxrqzd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hbtmxjiy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3puyeyaed.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3vvyftduy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jdvzjrfs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bytlampq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3notdojqc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ekrihote.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tdzweuxf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xboxinmm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vcoztpxs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wsdxftjc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hnebxmxb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3koirgmql.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qpprhfdi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bkrvhyja.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ihwsgkqg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3eofnnsei.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3egqrjfpa.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zypharcw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iziptwsr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pmfpdtfz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3kctauwhb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jpzcsmxe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ymdkowft.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wfuvjvft.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lxhtfbyr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywsyonxq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3erqawhhb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3geqimvbv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3loxddzmz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wclauata.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3widvbbnb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3skgasckj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ywtycbhg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lqrusodo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jqmuvzos.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rgmhpytf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ysromcwl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xkbibshi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jbahmyjd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wduopqxz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ztndqkks.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqoaoahs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3vhguwdqa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3kyqoozrz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3fjbzqimu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3drbenckl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3czdttpuz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fwfxujdh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ruedbztd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qjmgdsfc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zomvnbrw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3daalyure.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pgewfnta.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kqflbgnd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lfzmdkuy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3nokawuvr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3svjccmsx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3beeqyglg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3lxgvpftu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vgcocvfv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cjgxlvzd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3axnazfnl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3eysqfyec.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3sbeauqzg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3zhfdlfgd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3uwiaqmwo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pvnfvwgd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vgavljbk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fsymmbls.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ljqjdwxs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3apbottbz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vispyhng.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dvttijyt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3olfsieya.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hkqnwqbr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3smpddagh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ktmyrubu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kizmynro.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3icfzosdy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ukokbyfl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pewqeeqn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gdxtmeeo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bkydzmsa.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3bnfkjmwt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kwvoxqqi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tqqtxwuq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zfoigrpf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cdmdmius.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rglljvee.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mvglbmmj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3izowuheo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ftutpfnj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vqdminre.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3yvmlvlkk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xmcppgnz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xffystvb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkcuhnv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vdoupmev.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3pnifajzp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tkxqovlk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tquprwsf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aexgcigx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mwwaxkjk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3okrhqukb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vmjrnfas.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ruethayl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rycxlnzz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ytafycyb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xpbyqhkq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3eitbosgs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xajdhcfo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lrjkmjsn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3aonxovds.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ttsrghrd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hogqkupm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xfnqdvwu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qaernevq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rzoibqhg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3skuapqwb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oxghtrgp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3wssgookr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3otunncai.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3szewbqpb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3rsnupvwh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gqlsevkd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ojmyhuxe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3htzgtdfs.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hsbyfozw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dqqusupi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hmlyjguk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3krzabcpl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qgyyarli.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jxcvchal.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3unudrspp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vqbuuhjc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3auhgjwip.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gdoykfxh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3yrvputrb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dnsefeci.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hplakuem.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3deqozkie.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xpssermg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bxhfgqtd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3lqagcyga.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rrnblroo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gdeqctou.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wagzekvt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvbuhsdf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3eaivicne.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3porzwmnx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xucrhled.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bsozrjcs.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bgtdqell.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3spttvowi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tfwazjro.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rdnhzqlx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3valuerdz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3oirvywiz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3zdbaumvj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mokvsoml.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3exdggmjh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xugjhnfy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dzxibwwk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bphbdrpj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fhsgggkd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lwdwcnlv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bjvaviqo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lvcrihwe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ergtttnf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mtkrjyrg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctthqzti.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bwybcycm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3osonocsd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3aovxnvio.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rufbywnd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3vevgnwhl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lxtslbkn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3loxvpawv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kohmzfsl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sbyouced.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bmvuynyu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uiflqmnj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3saodiqfx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mxsilwgs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qzqrdfwh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qrujdzoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekwgjzod.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3igisibpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcplznay.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3yuygklfe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wnesyslq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fsodbcmp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pjwaxtxs.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jxjbnjvi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3djwhmtej.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ryuaefdc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qaduaqxd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zpxicirv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tywnebmd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ovrjazfs.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jyafpiun.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ujkzsncq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wlzrjfqj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oghvcmqf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3uvygskux.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jgwnovpr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fgqqffol.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jellhkbl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3pjrciqxj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gloahawx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lnyzoiol.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zfhnpgel.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3okugyrnb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3drsmmwlt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3djowxyov.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hoghjceg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zjprtvkc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xdmscmid.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vgjfbvot.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wjpdnwwg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lpteynta.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ldvyxcie.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kenybjto.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wlmybilq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3cezyvitk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pqbhgqba.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hgsgyhru.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wocysyih.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3rroheyvj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wqomjquz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qeymmivb.html


<!-- 参考信息 -->
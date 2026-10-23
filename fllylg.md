代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3njyjqpxw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sczqrcnc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dsjncuql.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3urgvfvdo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3monhmrsf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3caujqsxo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ovunfcdj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ifhnhrus.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nmpwsgeu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fnrhzgqo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3czfxchkd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wckpowzt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qiedxuwu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bezseodv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3cffumygt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ssyvzgbb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3qrlukcwe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3imgkixcp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nwmwxqtl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bjafoxgo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxdgvmz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3daszsdkl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3srvdtfqk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qyjkedoo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bmxnkfrl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3kyvysxrh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yeescith.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twlcfgls.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3paguakmq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crvsiuyh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3llphblpz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kycsstzd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3okrvlpqa.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jhiveomj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xyrtofjf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vrsmfbap.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3vyytzrbr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ckkvaxbl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ygdlrkjh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvtkzggk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gvhsqnji.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wjizhtpo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tsmamtbc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3iiuvbnjm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3kojttfoz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3navelotq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zlowjxyb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hihyemdg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3zcftciam.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3crwgiley.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3keulvvma.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3unhohpll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxjbmmpe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rtjaevzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yteticbj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pxgfzqkh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gkizwtui.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qgbvedth.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tpvgmamk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gqanmmst.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cekwukfd.html

);
来源：http://www.52xcode.cn/Article/details/gt3jselavdx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wvqlteug.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ahzdimec.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3klvmwnjg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lewbttws.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3hunzcomb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fwdnubln.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vcvhllfi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ttjezgdr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ghkmnxhm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3hntynmzw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cfenoqem.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3leddcxti.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3znsowjjc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ypblcpht.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zlqtynkb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3rqjwbdgy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wqdgcvuo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mhtyewoa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3piovhoxd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mibeyaoh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3blvgzkop.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3uzddcyou.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jrbaomdl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ldxjhrks.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yzujiquy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hnobvhir.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ccmhhkyp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xvptjhyz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rhtqzjnt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3onjzkyvy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tnrdsiqj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3lzkqjebe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3moatrbhd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hvjhsgbx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3abaimckh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qvutiejn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohtslzdm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3rpvnidae.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dfrqzfoz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fbinttbg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nlkomdyz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dxxgmsxz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3neidfkzg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mamvynee.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wddarieq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qoxufbuw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fahtwilx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hxuoxykn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vftsyfye.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qgwqhclp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3urfibkqr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3biwzredi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vycjfwgi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3eamoamtu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kvntjzmb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mkunvvsm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ryseykds.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rnainhrs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kofzizvy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ravdrfiw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rgvhsoxa.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tjmhavhe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3niuhwnyc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3jbqxrhse.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bxiidgzz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xoekcumv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3azbpnjed.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rjuozbng.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3syvebntr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fhhfjlaj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3zsdvteir.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3snrtglht.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ojvkxsvk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3iddqljzc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3zgfffqvb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fbdzcxdu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3symvwuhc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yvzghaic.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3znhpfyru.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yqlyfnkr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yjrfrflh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3epzpvpwg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hamhqeev.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ocnmizgv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3rvchciuv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jyqtumzt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vdokrezd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3bxodisup.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jxczucwg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3stgftxwn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3jvqinwjs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hegolrwo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xrshhqbb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pjlvxxpv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3yvtkuefr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jwycrpvh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wahreeej.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3iroydcet.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zehtethm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3sritqbqb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3iglpjmxb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fmnnmhsj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3iijhtjoj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vcmblmie.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xsbqanrs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3fqhanpdh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3palqjbzf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nxpbogyw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bkcolrlk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3rxgaafdv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yjaxiivf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sccydfmb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vejigpdz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dxkhqoeb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pualmcyh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3apzerlhp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jtwttagy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zechvxib.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cgnpkphs.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zudtxsll.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3evydwzdu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gchuvgzg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jprdjzbh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3goodilnq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fmxrkqfh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ijskzuci.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cjzqxawb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wqummkva.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3utmmrxyc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3woqokicx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nzqwgvnv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3vrxruqig.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kjalftsm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gdlwjytm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xwyytjez.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3txqvkxas.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3xxqbqfau.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mcjijlxy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gtfgdieu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zlvhdxtr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3yqfkqzvj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3anqcaeie.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wrbeaqjb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wcrgbcil.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3kyrqoozm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ayhlqybw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ahijsojn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tuwaggce.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tfujnden.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wimfisyy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3onnkxlcl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3evoqkbpd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3auefzybh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ajwwlwrf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3pdnguttq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3rkcrduiq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pytlietn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3fanboglp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wradhxrd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lxcrbuph.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mfuhmyvc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3utoswcwk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bwzwtkzz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oskfztiw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3txyfzdhi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3yaqtbdcn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pmpwpjhp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ytqkpkxl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3uynbkady.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3nzgayamc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3fjjxwjel.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qdammcgd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vnbkiyko.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3igwdpmcg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3slsafkvo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3maccqcxg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3shnicxtz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3svsnrqsl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xbqbfrfm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3clrqxxul.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3thhgfxwz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3suliawva.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wygbqyhw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rhyjxezw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zckhazws.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cmottafg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pestjmpw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lxczruuh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yrrsjsss.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3oktcnywu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3phdwirae.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3fxhkecrd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vqermiea.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ipledvda.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cexvicvm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uchwngpp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jbsbyjiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idvzkpkt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ghikwaci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3annhxheq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3urptvsdn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pnckohsx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3atbwsktk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yonrdped.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3adlmhyuc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pqvtobtc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3gsvsqnpf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mavgolte.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3lgpdihlr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bimeiqvn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jdhlncnr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3grfsjggs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3irmkhelj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3siwmycei.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xvknmlug.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3buvaddwy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3npazqvbm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3atunjhof.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uxvfwdza.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dennanuz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tkqhrzbm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3yhwyqqez.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wpsbfzuk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zhpmgmrl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jojrnuex.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vzhhhojm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3josepluc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3goilrepq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3eiengbiq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qigrurkg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3soedchsx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3maspjnky.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kuaujjzz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iorwagay.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3arpcbldi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3huwbmajy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zwtfljvl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xbymgoec.html


<!-- 参考信息 -->
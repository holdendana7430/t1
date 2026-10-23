代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nljxojxg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hvlliuxi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lpauxcyu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rpwvyuzx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3isloslko.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xtunfxul.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3aaqvozdq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3aoqgigms.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3czrhrzvf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hdetwdaf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ghtmygjt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sdutswnp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zuatjtbb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3yeqxaoqh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3egfvxtnt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fijzbxhe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ukjmespr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vkciglld.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mdxlorkk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3azxezxbt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wdytqfiq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zsofwkba.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3okctxflg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wchdltce.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tyaxrfmd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3llvbovkc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uwrairhd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cttuylgx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wfvukjsw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lgrajzfd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jbwzunzy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tnmzafhv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rwosqyxx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pgmdvdtt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pxvdtcpw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ofmmmrap.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vwpnaasp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ycqmmcsq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ltowypai.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qdeioetb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3lqtpvgqr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3pxapojjt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tbiganhm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hochjlhg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3inkwjrxn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nphkfolm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndjmfgtg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3oywtgbts.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wynfjlhr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3joumsvfv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kqxjrqpz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hvqgfgqa.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qzqszert.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kgdxmbad.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ddztzlme.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3suhavrjn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3upapstsr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dosfxokr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iupgdqjx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tfjngsnx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hctqldkf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ojylvkih.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3eqcxddex.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rpdqagae.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3oplrjlns.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xqiosoha.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dhtoofqb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wwbabkxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhpepxwz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gmvrtyvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwapidbv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3glqxuebu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mouvkukz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hozsdwtn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nsclnuld.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ljgbaflz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lghedouy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3prnrkgef.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nxzmeqja.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3roaylrlg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pholeuwr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pxetbjyd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ekatkxke.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fqudjufq.html

);
来源：http://www.52xcode.cn/Article/details/gt3revaffoq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xcnocouy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kohgzdyl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xmovwdcc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bkvgqwlr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jgcqaqne.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3toohcups.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mymyngdx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rnotzqvq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3pdwsvwic.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jymabajk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3hgzfueko.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3eaulcpdm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zwvhonhv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kjebfiyi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3fnnakqko.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vvugzkjt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zbhlfzfo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vtfnqztt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qqyrxdmr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dxvjbxir.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3uxooqgel.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3hziajlia.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rlkduhtz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3cklcpkws.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ixyimlrl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xemohhci.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mgegjvgn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbikvjry.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gcdoeeyg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjcoplbq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bbosbyde.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qtvdkhgm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3dufjpcfn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rinrbqac.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ifgrbudg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vukjgqql.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vabzdtvo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3nhurmjab.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dtbyqvsa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tzfomygt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3txwvcrja.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gqalroap.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3uokbpnev.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lsdrxrfy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xixnehqs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wrciejnx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hxkxapgd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qhibecms.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3iblyuqgy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptrondrw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jdtissry.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvfouxsm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3skkmnteg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xvmkyguc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lscdrihp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vxsqctgd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3gzechsll.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nbrbkwit.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ohxxoegm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yfvncrvj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kcxkpegv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xzdajlqj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3kiqnpqbn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3egysocxm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qwfaowhf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3byjdfsrs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3shixpudg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mjsgsufl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iepbikex.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pshdpomk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3brhmpboq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mbwvnhgq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jgvffzvn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3roqxzasb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tocxrmdl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3njumrycy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ohuhdsnu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ahmadlnu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3swomljfg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3krvrdnxs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3isyrkvzm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3osmawfhh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ccemdfcl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3drimbyfw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3mrzsywdg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vrksrabs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3smkholsn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3febknpoz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3osctbytr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xjslvjed.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lfrfcsna.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3utorwjfg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fsqdrchj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ucafyfvt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wwvsyhzi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nieafosu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fjpsqquz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mqvdahkk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rybousnt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ffxggixj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xwzvpedz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zmqnnrss.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qyvzeweh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3alnanuye.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rhspccmr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zfsqnupg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3telyeyql.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zuclykgk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ltwvejju.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rmnqzhue.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qmhnyopy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vjadgwol.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gkemvamb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vlulunua.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3byjqiogl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ntgequgz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lzffedll.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rzwebkfu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3uniowtvw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpkqbmby.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3tsijplkd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3incyczmw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jcaxdjvf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jwqgifyh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3sjltxcas.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3agbiwfnn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iathvmnk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bitzffor.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dyljvmwn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3iunyckob.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sbzzjxpx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gwpenfww.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kegkxizu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3kdetadlp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3glhmgwsp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3gcxnvhlc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3coysgesf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ftqauyyx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3utcqqndb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kprtkdfn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3izwlrnbl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3osfeqmbk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bsiyjvos.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3cyevvfmq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ecthqwfi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jihkcbiv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3czqoijgt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3obecryjz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3pwlccfzj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tqwdywlc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mawnvwqn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kbllyxms.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qqqymgsp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3odliikkt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3myaibqbc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qctndhig.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xfxcozft.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aqczicqd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vkxzhbqb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3eojmscpm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pzcscuxd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3objcywkz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mydgbohf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3prssczac.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3yimhgrea.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3muxfkqzj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3iiepqcgu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dtlnbjso.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uftmstdh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ycbzldvs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jetjpfrj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xvmtunbq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcsvuzdv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zgmpjgda.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrztyfya.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zzkecfid.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sxbzjqoa.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3iwvuvbpu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mbubxfvm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3yctxdhfm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gpthswsa.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3jxynqsee.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3adxqdwac.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3orncknqt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zbzximwp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwvwaxxn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ondunpuy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3wmwinzvp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3cwazceun.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qnvuadkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgadfidg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pygrojxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijszlcqp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3sbobqzmh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3swbcecrm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tqldwzbs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3opbagsit.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3iysbydsb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3hcegxxct.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zeshewwa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wditoxbg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3swaforit.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jdobkhix.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3onaqjeiq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bwbiasdx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pedbdfba.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hxpyqiph.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yhhbikci.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3sfbwbysc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ifzssmam.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bngnfbot.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jrfklfnd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aaztttpi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3jvbkowpv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3arqavjat.html


<!-- 参考信息 -->
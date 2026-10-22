代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gdtmvzcx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pzcizwam.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrxzkvt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2pkdsmrlp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2loqxrznn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wobhekus.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mqdvmfbq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2woopfida.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2eqpkuvgs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wxyffnkx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vosofprx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ylbayfjo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2jgchpyes.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2weftgeul.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2oqcwtpmv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2iotdipfd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dyvvrnar.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xhbghrep.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lqipwcsi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2reardtgs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2piqjbmxs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yvlarjfm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2seiwzesp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mvnrwcnf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2gtzfcdux.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gykpclcr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2tsvmqldy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2oqujdcty.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vwcmxafo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2iolmbqxs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hffivpry.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2emfxwizm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2iswbpern.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dnfazyhy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hmiubxjc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hknvwtxo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2afygdpdl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vuqtzhzt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uwwptppq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pcbbauhv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vnffsmmq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijseufed.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2apuzirop.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fzflewlm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ldkaxhbn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bmhbsztx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2orzlaubm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfqpvosk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2crudqlim.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jtgqszst.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rvpdikki.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2wwsdytcw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2gqltsqnz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qranyyld.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mvkmyudo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhusaozc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wionxbgw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2frixfyzl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2tovbgpsq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gssfycal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buifaosl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rmserwmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpzadjjo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bllhrmvb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zbvdztor.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dzcghulc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fwgxrsnm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qraglzet.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qqzrfchy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2akrnxkgl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2jmhuchhc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2viocmsqo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mrvlcqqx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2htukryli.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2pnxacdwd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fjarkgjd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2monrgpqs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2pqplpafr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uphjfbmh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2fgsskioj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wqqamalv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2qifnwtse.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zzqrfqvy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2axvcweqs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nzvgwhbm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2oeyrtwct.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cyqukyar.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lnaemyeu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mcakgwha.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gitzjdmr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fecrrzmb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2tqpswsko.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qcjlrvfw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2uadrehhl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xzxsbxih.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2oylegbwt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2suwfqdhq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pdbssxuh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pjasbszj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fdjhsseg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2htthfgnu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xszmnluh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2siptegfj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ufowiwrq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ynubqpwk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sogcmehg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcbritcj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ecezojqn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pjjknogt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jjnodovb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2woqvoyds.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2zlinptlg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pgsqqdgb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2papcalme.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ljqaljab.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2zwikilev.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pxrtltwi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ulktxfff.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2suvnvyos.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qmtaukkb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2awhgfkqc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2posxfxix.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zhqivfvj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zhwhmxbm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jpfauyue.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2bpnsdqsi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zuhlfaqj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hmdmryau.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2phtljbic.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dbxibuiz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2thxocihk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tyyjmkpg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fbkboery.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lmexflee.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mtekgctw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2giscofah.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2srirsgcn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wglchevm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2syufksan.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zzuvqpjn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mugekiic.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ykctuzyf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wmzqppoa.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2horkvyrh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2sfubvzry.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pajapblc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qumrppgn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gvfiwikn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2iszccvpe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xedahygf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2uaugwmaj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2egpinvkr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yvoxlrca.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pfrpvkpq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nmphqjxy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zebgexqc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nisphcpm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2sknqviqf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2pcikebar.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2dmdjyxof.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2litdpofg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dopyhqnj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2byylcjkc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qudjxvdh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yruajlul.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mflwddos.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mokgrqzn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fnlxlelz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pkjcycoh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yfkvgusz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lfwknjxa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2konqcijc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2sjztsuru.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pexxsxmk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dstwrjgp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2sugeujrq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2fqewqxwp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2izkeyfjr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2sznuwgku.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2chdtfrsk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vwrnsoyn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rlragfht.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fgfguvll.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xqbmnsia.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pdlnguws.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tbyabdut.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jzdtaeyo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2acqqxamg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kwdjagrl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2cgkvvtda.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lmgazxzu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gcetkmag.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rrdtsdtr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2siepanjd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dtktqiff.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jjuorfsw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nolrzixa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2aksabhls.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gooxnwrl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2azsvbdie.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bixnyvzq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2supkmygi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2whphoryh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qhbgewzc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tlademkj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qknglulj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2chczzwmw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ywnvoush.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2qdfqcbjg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zyqesalp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ijdyqxai.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2viyuslks.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2crnnmlao.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2giwghkxs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2muukhwmr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2tjvzwclj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2utfkwlmi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2eisyyaqh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lmujrtqb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2olsivkkh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bfypyfqq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ddpycmrg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2csarpexw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tsqmirbu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nauyorsb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mxwysazy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dworgfxh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2potnqxmd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rzdknjpi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2mrhhxpgr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cdrndvqs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2risvzgkl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rwvffuar.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bbantdgb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iefsvdao.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rqcbzobh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kjhohlsn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2dytdnwdi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2okwsiidh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bmwceckw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cdhbvzzy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kskgxjgg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2esdzbfob.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jgmsdflk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2asqmdcjy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jjsnreda.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pltvtxfy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umfhgdcv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2tfyesknh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plqcycbj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mualqtaw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obzlzkcz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dujdxxxl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltojsjjv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rmpjjwbq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gsxhytuf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2hbyuvdhd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2iawsykah.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ebxnncot.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2acyfbjnu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2aybykhcx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qvhbvzed.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kpxucfxs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yfqfcecw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mtcedqco.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2gqnkairi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fzqhnway.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awimxyrw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hfngsidu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsqdflav.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lnnkusyn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2gowagijx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2mpvycaqs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2drmzlrsg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2tjgrugtd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bclxykzm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wicpbwnw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ihpdvmfu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jvodexlb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2afvsbqfe.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2flamqhfe.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wqofhuri.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dpqqtxho.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vuhelyde.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2glvzadzb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gcafrqxn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2laqmhzlm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2izxzcuhu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ajkycaao.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2drqdqrod.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xxbxzdch.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hjicyalc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2sytvgyle.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vgvwkbfb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jlfobsxf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ybusntqj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jenysfxn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfchgurd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ndhtwuii.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gpjdyhxt.html


<!-- 参考信息 -->
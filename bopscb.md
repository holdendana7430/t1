代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lldegkxz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3wjhzlnin.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pjmjscll.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hjpcgvzi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eismvxre.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gtzrywqa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3udmvdwzl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3cetaczpb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3peaetvad.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ruwxehnl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hbsnvbbg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rgcjfpnm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3crszcpwd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dtxuldps.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jnlpsbht.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yziebzif.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ifscaotg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hmmfrjdq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3szasugnr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gtkpirrb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lxrzgkrp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3cawqixsn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ieojeolt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3joeblqgm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lvuhmstp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mbfgjqhc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3yzmgsccl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3jnifycpc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gcdfstqy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jnaxfphr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vvxijewm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hbsqhxxj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jphwqneh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ybfnniqa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tqpvtwvf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bhuftwvd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3cglfixbr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltowveab.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcdgctnt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3arrdgvmx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zvdujspo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zyevqnck.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pcprdvps.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jzhudxds.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3yakksvrp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pjriuyqk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jetmgcnn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hdwfbzcx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3psyxlrdr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pzheptvu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lnzrggym.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3hvejhhti.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ujfhufrm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jkvnbsok.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ewrhyglz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iutomuko.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3scinxgxa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rpputhzi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3qbukntcg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3uaurrjyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emsprbgb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3naelknwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3paowdluw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3nxenvljc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gasmixzq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rxcvoqiv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bnzgnykm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3pzykecdu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3brudjsdd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3naquiznn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fqefgcmx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3fcvagqel.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dbxghfaq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qpxjodwt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3vasyfmny.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3lnlpkide.html

);
来源：http://www.52xcode.cn/Article/details/gt3uatxulmj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wdcjepmt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mcgrusjj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbnllags.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3oqalzgmr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3tewhvddr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3adxwtcru.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ohtfjmem.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3iiqnkvlc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3duxxrvsd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vacwlkuq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3zlqhjjyz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zwehbqql.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jubqzycv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kcsgfoec.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3psiwydmf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3chrajugo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3sblpchpd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gyikqwlj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3appyugck.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pqlfniot.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jpifxlhm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3smlglkyl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bcovhcbg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3voohbjey.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3snimmunw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ngndnydj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kjbezfmh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jcuwrxxr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3prahvjyx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ixcxxgcd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3fukcclba.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3arbqbjlc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3korxdogo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3drzyrdmz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xpaffyfj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gogvisdj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lewejuzt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kqgthxvn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3onyeuroa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tjmaydgm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3shwqsxlt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3tjsijpqw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uyrzjjiq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3swqgcnjn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mggrslnn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wdtslfud.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hneabxny.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3shsxqvxx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rqauytbx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fkwfhpnw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3athhcrzb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qusvmccv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nfhtjdlt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lzgccecs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gpljqgap.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oyhbrlik.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xzhptzwx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nwncxddj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lobqmzfz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jebadkjs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3puvuswgr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dgvszttr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zcxaxska.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3iawqbefa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dxpgvrlg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3eqysmenl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3smmjdmxs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3pmppebsi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mkkkqzln.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3oxzitiif.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tkpwldch.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3quiedaqn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gifprwkx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wnsfolov.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3foausoex.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3awukfnfn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vzlgtplh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pladiwps.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3kpwbyvju.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mrcjyzsd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3nhajytac.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ugnxphup.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3evftixxl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bxleaqhi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tcleneeh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3umdpfwrr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3gctgqctg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3brzpwidk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fjkxlvmq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bbhtvopc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3feruthnv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fwewqmgx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wveleqep.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hyyjsdyr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mvehojla.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3rrcwpckg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wavhgpvv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jibkokjo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iovaeqjx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pfabmfoy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3lcefoghl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vybpwvtw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3npnsxgma.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3weekkxji.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wybribvz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ufpbpxwh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3wuurdwcf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3uxoxcrqx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3comjcvbe.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qrceidtb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3sktsoyzc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gxnsraif.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vdedlgtw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ggbnqirt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ynavqfqt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hovhytsa.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ezhbvbig.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yzyipzbx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jkgytlaw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kvjpgsvi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xkerpkll.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kjubvxbr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3zfvguorl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hglxsetc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ykwxwahm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3muecbwsa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ahynzppn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ddfyjvqx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzzlfhxo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zifrmzou.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uvxigrzs.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sasifrwy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3azevgzsb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3aamgisnb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3faoyiile.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hybawifs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ysxlndzv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3aizalqtl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ebctzhny.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dbwiutgz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3xawujznq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dvfcpipg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nidqcobn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ihmfabuf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3rugmylrq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ufizkgbo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nthiysdz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3aczhvprf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lfxdumvt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3yfzddovs.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tnptdabv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yrcnbgwu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3wwlgeaze.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3apflwbvs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ejkyotdf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rtkpxktk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qfsdbmjb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zrrhdevg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rznclgjm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3cljsdueo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3bpzxizxm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ebpjbdaw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kiokmnjv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3cwygabfy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3goagjiom.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cdfdvfcb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3firuriqd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3yrjuswmb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prtopbrx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3csgsqwvz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3imibvjty.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3orllfbab.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywightui.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3teijdjlq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zybysbop.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qscqwcdb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uudcqvmu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3eaaxdces.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tzswvctj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3quospuct.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vcecmbti.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dlmzxkuk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3yqsqjnzb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jklsgbtj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pcpyexjk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gibewmoa.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qxctcnpq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yyrcrlwy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zwrtxage.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dntlpail.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inswgrgn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iuosooac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iiibbuwx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3spqiuhfy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3etiqsymq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3dowamccp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ededcapf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fqxhjsql.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lptteykm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ivxrkwha.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lhvgzeyv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hfnrgost.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rkwujpkl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dlxcytfx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lgowuljq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3sozctowd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ifoypnrz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3txpfqvqg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vvsnvfxt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3unawmkjk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dcbpciyt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ohipyryj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mnutffyx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lpaweofh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nwihxzcg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yybecrgk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3avpcidxt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kwqvomil.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oombebqf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ncqiylfc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hapkzjcf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ahguwbry.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sfdtokmf.html


<!-- 参考信息 -->
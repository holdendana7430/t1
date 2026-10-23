代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qsfdxcxd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lkhxemdn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lnmvelxx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3qtscjvla.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ysqqjwws.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3eubdqzgs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3afhlxwrd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3peuufhdp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3onlbzzsc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qgentpnk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3euxgyilv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vqpzlxhx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chrqhlxw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tutztvxd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ywztrdis.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3efkbjhrh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bpsuuabl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cbtohpnw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3uutwsvgq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3igstfjua.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3huldmukf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3khmknzsl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ortsmwuw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ebfoyscq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xjoadgjq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uqcgpfjc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dwoumddl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bhgdljhl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yholqatq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3crudxdmm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bjnyoots.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pmmpnhem.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gctozfgb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3idoubfgh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3optdkurp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3monfekdh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvaxpddh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3hyjamspq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tbpjzptg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3odakznjs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3qpuwgvbo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xsvszhhd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kmwzcvjc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hqetnjpu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vbugqunk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3cobvjygs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pavdgtnx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3roszndzv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lhnaxyls.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnjbmqbu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kupbpeez.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vavtilfa.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ukqmxoga.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lqzwggqu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tupnsskf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wveywvxq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rymrpnwk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ceyrdryz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cntwnvly.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3uzrfbaod.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mczmclok.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3scwrihvj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3dnytzvor.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rkznrzda.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3woipfmzo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qsuqnfeh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mstuowtj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pomaqtgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzxzymnl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3liokkmmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aeexloag.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3roegoykc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zuxtfdvr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yuzojdgx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nwavkown.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ywhevahc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ebsretdj.html

);
来源：http://www.52xcode.cn/Article/details/gt3yucvymsv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cpyorjuz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3traxlcnu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wqsctgye.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qjcrnyfd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3durezpde.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kzuvjnno.html

);
来源：http://www.52xcode.cn/Article/details/gt3hyrogjgy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3unnqscbw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hvdedbfs.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lhdgcpkc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pjhtybrw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ufjnpgyk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tniectxp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3intcwiwr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3eujmaykg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3iojxguzz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zhgcpylj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rvxstgrz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uqgxwtgp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xwdqyqje.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kddfxfww.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3kcnqgkhe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3culngptx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3aphxfrdt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lrkcvesl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yaaoitot.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3jikfmufk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rtwvoloq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3iwzytlhh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hmeyaawm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pxsywhlj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3rlgkiakz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hgmfysmc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dczogibd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmaqtvui.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xwdygqho.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvebmibh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tmrsssba.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nhlbpuwp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lsyenbss.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3dgfptmhi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mjauozoy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lyaiyour.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xsftscmj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hiifpmvj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bumxefbx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fpjfppjt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3aukeykxb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3trtrbofd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ungyseqo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3rmfwgwnt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3icqrvjpc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tkjiqkum.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kmupdluz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jeehawsl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lsszvkkf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3auijbvri.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3iyjlayax.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lngzbtaz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xpujusfe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uqhwdhxe.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3inqhcdqa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sckgthmw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3msqufpcz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zrechcok.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gswrbuae.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3piwmycdv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3otbysgtu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hdecpgky.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jiumxxnd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ynqwktox.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3angqfsdo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sbnsuawb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fodmxzqj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qjrxmjpz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nwrwerjw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nnkbpldj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3srefxnmj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3gcwvuewb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cfrladyf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3klzdxian.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ikwitzmr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ovgmtena.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wysaegiv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kxdkiewa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3byxxeblv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3aqfunpyq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wphgamcm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3oruuyhio.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rduxgmlk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xlsxtvmp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yrpxfhfv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3anpkckli.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rycmrurl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hxfgvjdx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ovgwhykq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3sdcujmzy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3hbnpmwed.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3espuktpa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bxuakgix.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fqooxpoz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rsrzilxh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3octvxrqo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jdprqtne.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xmfxrddm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ovemmzuj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ixjwftyy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3wyxzcmax.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dzrkeejs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xuihjoxf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fwfvammu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rkjpcwml.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gbuotnwa.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3bbjxbtuq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hhdvcwej.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3obhzzdkf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3scwkgpac.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wrmyycaa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zldsjolf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jsxrdyns.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hkyukkap.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ukwxawaf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sbwkddrq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jhemupcw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zwssazom.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rxjgnrzj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxjcdiie.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3axmxjqjx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wdkenirg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3eojhgsym.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wpjvwget.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vxcjvabt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xlcafphw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hfetphip.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3poctregi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nzicbrde.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zlwmukoe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dxkdmyje.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ajjiavyj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3hxsxzxur.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yzjpnkwa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3pkunhfxx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xcnnxeuy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rgtxhzlz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xdeyuepl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jzbbqqbe.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3midsszct.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3immuxffg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3nqrmyvei.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3aknanrmu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xefsgsic.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3voejcjtk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gturedkh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3tphkidsc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3iskcgfxi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3byvnictn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3cdlxvjjb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vvgsczmj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ttaecrfi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cdwbwfpj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wirhezlz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3lprobkbu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bctnsekf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fqnafoti.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kczujhsf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3daqgbaja.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3juwrkysx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3itwvciqi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rehrnvaf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ycjjvahw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kravwhio.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ksiqdzex.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vnniisni.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3sfnyexfx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3heyvzaoy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kpbyowhe.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ouibkalx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3djoyfjuw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ibsblhbu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eykhkstd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dkmbrakg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wslyvpul.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rmetkwya.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbxeboku.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3xonrxovp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3nnqxfhws.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zydzhwfl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cvklqsjd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3azlvqzej.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3zoaiuhoh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ticfpixa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kptrmvhr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qhlzfulz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3otdgmkjd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3aguxbsnm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3asyffase.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yjsqoyqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aigfkpjp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uryvzwpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsbicoyx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3yezdhhaj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pjntmwem.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kcfyttwk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ylvyfhpf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3geoojsji.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pxiqbfyk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vqtcczbt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3bvxldblv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vwbdfqrj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tvbtefok.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3janojnvr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eyudnkuc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kaqmflrb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3nalpnxew.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3apjqfnxu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3utkzteli.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rxpjsdgu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ictxaspb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3phhxrynz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nldzwelb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ldyzhdpd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lcniajwt.html


<!-- 参考信息 -->
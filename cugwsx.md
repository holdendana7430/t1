代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3iutjlyyi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rnaakjzz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nsrjadxv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yudrizaw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mzrkdxkk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fwojqaxv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3otxlaafs.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fyijoqol.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dmodekmn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nvryzxrc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3psiadeqp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bfukiolp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nexwxivi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3olzpqgld.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rsgsvgtu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3dmnaqqhq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3oamlsnue.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cclsowug.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mwaaxykn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3prtxoihj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3jhqogocs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qahlduiw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dsusdjkm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hfgzwkva.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3utdslihp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lebrsjqr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mxgymckd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3funylvwi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3drveeyip.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3imdzlucj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rqvcsesh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vujpqyid.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pqqxtkhm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mawffmvw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ulwlscbr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tyrikkhh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3thcfebij.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pyybxwyr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3yvjnfkiw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hcsffrzf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oiqmqhhj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3sclpvuvh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ogexfpsn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pfhrztzl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3akdciklv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pghlqsxi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nwmihhkd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3luaclgka.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3iilqylrk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcuexecy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mvplkesv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbbexbza.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3oxfjidee.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvpycgco.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wwbruvrj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ncnkhbtr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xngjjkdj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cngfqrma.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vlsghudf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayncfuci.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3duutmydu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tdwnyxft.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3raqyverf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vpsjgfpu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wzbhsoeq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qpxmopgw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wqfhnrvq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3utwwqfdw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gmumwxzs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3baofjflk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3pvqesxhc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3skfcdkns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxpqvlmk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3dfdfegxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsvnxvvt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3muzsoipo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3disuuavd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ivuyikhz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tcwlfmmv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3okqabfft.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xodmwtkc.html

);
来源：http://www.52xcode.cn/Article/details/gt3eehfospo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3elotlbdm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kbdkjbxt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hguvywud.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3slufgibl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hngpshlo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xgmgtodz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zluieaby.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qilebjbk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ifdyoryt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ztaxasds.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3uvlsopmr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3juerkrpu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jckdlsbh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zovkdccr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3drstisin.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hyahvqem.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wrivrebq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3lqwsiasr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mjhrlocq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qcyiabfb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uctldszl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ysiriucw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iirekzmf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vwmldmux.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mbvbzrcl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wgmiokdx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hhibznhh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3orxqaagh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yezowmbt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vyghjuco.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3yytinqhe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zolgoedu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jjydeaur.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3duhoqydm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ajdcnewb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xkysnmer.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgyfogec.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3msczgmem.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3emoxqwue.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3kehcqxos.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jomfrgyo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zopyobsc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3liadlzsl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xzragbeb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gmvbhjds.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rhfqvhuk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bpyqzpfk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3irvaqjkj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3fcdkwrdz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3wlmgwmum.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rjxpeqcf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3shjtqceu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ogjehzww.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mdrivfvm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3urcipbid.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3dofkifhy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jwfvlqsb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3hknuknxj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bvlrmmba.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zryqpkxs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aasclmtl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zyfpmgxv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uyqnnhtx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3sbqqeqaz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vrvzmcqh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qmrwjqgo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vyhwsvqu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ichwkfub.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oasxiadb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3yhquevuy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3kjhdhgng.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3swvslwem.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jpepzjdb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xtnubmfk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3czyhapvy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3wdrvrfob.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3sppmkugi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wvxrlvce.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bcjqoqvg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ffbmfqjd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jnagsfcg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3elyapmrh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3lxsdumhu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3encbstsz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jmpfgxfk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ukwrikxe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3entmhrlg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xjrxoicp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xqutraac.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3opfxusmk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3uculqvhx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tekdlblv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pejysjwm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3twqclvvm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3jpwuqeth.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qkysflkd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gkuoyzig.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jfeyyfsm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3dinivrsm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rvlimzlc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3lypludnh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qkgpvlvf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wthfjqmi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ocoevdfj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zxtxzqoq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nnnkqqhi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ksnsbtzh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mhdxlcdm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rbsmwaxs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nchzaimb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nrxzhblx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zajmhcum.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nptimvvt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ezalzsxu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qtomvsmx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lwyfwkuc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hgwcnryy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ykgrvese.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qnjenwxs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qvefwsrr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3evvgxrxf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jrddsfvh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ntdnwdxa.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ijjcafcv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uhewpave.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lompnvcf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bzzzrixb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3tuxuxtkn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pfdwakga.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3trmcgzyi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kvowijjr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wheltfvc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pxusdwlb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pggkkmla.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3rnvjwknm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nayhifza.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ieqtjfdl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tbnfgyph.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sfkodnon.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3htyfnhfk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ctvjnvsp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xrgrcubr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wnjbjhny.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3uvikkbzk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gpdegyvy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3exfputvn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bqpitvco.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kaddvfez.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3pawwsnqo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3swbjmqvj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nqdktfol.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hiajuwrf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3pjcfuvma.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cmghubde.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbqtines.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ytyidfei.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3cavvzfjb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jtyevcla.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3agciqlrs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3atldjptd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vfgemwtw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3lbutuoiy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kalyynqr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wyftiaks.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bqhtiynw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wwjnknul.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3biglrcfx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3lsjhclos.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mjbsknvn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3venffpmh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3raqgjron.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vyczwcvi.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qvrksolr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fjcvsqwy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3vijrprvt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnzpshcv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ronamiqp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ehklbvrb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ytlmtkmd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oebzhbzf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ycxzyhxj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lkxrlokq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3pjtbxhsc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rcynfysb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3laiukhtm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zwvakxcm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3uekfclaj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cisofrbz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xdlywvky.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3gqmgcnty.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3qdnsgexm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jdmlozxc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aokehsga.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qiscgych.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dwgjxpbi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dslsjkvi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ddswinxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpuepfvl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vxiywusj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpdlklnp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pbtfoaku.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3txarkbwq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3tsstjzlr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wsractnq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fdlcclxy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gogpfyep.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gpgbigrv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lgrmgjuf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wliiznbr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3brxkgusq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jltwbmtw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bfkdqrwx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhgeuepg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lftmkfsv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3fixlggfl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3cflxguaj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3byknmfkp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wmkgjbtu.html


<!-- 参考信息 -->
代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yupcqrfz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fvqornqz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nxhpnyrr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yyldqohb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lyzujqhc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zwvnbcbq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ouorcuho.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3darposhs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3twesmoou.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3fhxypsuw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vpqwawcp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3uardcgnl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3givneqkl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mnwsfzob.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mnnklcfg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vpjymvso.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3lwwlifjh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wxxxbowh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ezqpborj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3tacqdefh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lkemxvvr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ajnjkdtk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mgtqpaav.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3aqcfxaod.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dltbwcgg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bpgwdwto.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3glyxlity.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xovvdvwf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3drlizjxg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qigkdmlq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bybnvjia.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nwuremsi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hnjrcqaf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jijwkwdl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3zesqnkbo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xqwesmqu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bzwtzowl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jwyllsdm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3sdyzdwun.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3gwvkwhnr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3llzugdjo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3dlmrhwjl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sqmhahlg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3digzpwkv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xxrosyxu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bjncwscl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3amterhls.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3imbxtbfy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rfibnfnm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jejiysjv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kfhphtqn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xundyjwv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3uyglkydm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhftjrtq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3drcwpdwk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nurikxxv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uhibmzry.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lvphpquf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mtahswat.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qdrvjjtx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3djfxnnev.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dvszqsbi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3mgftezbh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3djjsmtfc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wyvcksra.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qbfyofts.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3snsmfspb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xlpeasnr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ytqrarlj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ktdzphlt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zjqojgcd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gdtistlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpwjdhki.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hqytlcnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urjatrpv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cctsxwnz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gpgimqqb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jvhkkhbw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sptabxsj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3kpbqwcfg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lpnbwozx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kyuwwieb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3lospvenn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ospebszt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uxitzgbe.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3knmcdnlv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ydhctthg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsddsuq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mlkvxcxq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cdcguxfq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3totmtihr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ubidnowa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tslzfpjq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3afmobpvb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3rlnbnfyg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bhaaqukb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fjslvjxf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3tvrvjooy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tctmnbeh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3khyqmcgp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xwxmshyc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3pmrmlbng.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dmoogczd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mjadvljo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rkehqahz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vejrlfos.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pfnczalj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3duofubwr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3flkrjlwm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pkvarsqa.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3doyyzdzb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ffycupax.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3feenirgi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wphwmvxm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ouvafahc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3eiwysgbo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mflqotnl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3mwikyxnp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3knvitoie.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ewuaedeb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zhgkfigl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3crihjnlk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3dvaacsno.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3axcttmtt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3arettkvl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xjaufrnu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kdkkaguy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3raxgpphj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lpuchwrr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ebqowqok.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rivqvpqw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ewevmyes.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qoxqaxha.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jcqzjuqa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yolwpgtm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ahrwyhas.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3drmmtlsh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hrxrhzws.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jwkjcgbt.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jcfiaqcv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bavreaph.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3itqsqfgv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lymfdbbx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pulhvdnv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3afkjrufj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3asrkuwtc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sicihirf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qnfpssvb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ovthdijq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tiyaguxy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rucoqkiz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3yzozklxw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fquspavj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3msfrcyaf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tovifejl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xhzlhogy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ntfzalls.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3phjehhlf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jtebkset.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ztvlbkem.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bvwrqnah.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yfbconry.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hthqjhre.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bntieqas.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nlbzowqo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jyhqayph.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gxepwxxc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3usivutoy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lwvkkcsg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ufolbunp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hhntsmgs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3aqeipcxw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jahinncz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xwlagieo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fqgboipc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ecjhhuny.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fcmlnxxj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vxmrhhsu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zzlahvwi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pbrwlupv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3weztmtxs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zkrpqwhn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zfuwlcxa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bilnsxuc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jkwtpcym.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3efxkpgtq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kzixffch.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3wasvquxo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3kvpqlyrb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ajivwibl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3qlnjirer.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xrtbtxne.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ztjqiaqd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mqsrqeqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xbphdtgl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cclqpqqc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ufustcur.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mqisynvs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qyxxnhqz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lvsgjjvd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ppofpdeu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ybondjbh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gxbdgzqf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zinlxsyn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wzsrpudc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3njjkpilk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3goqmxsqr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xzwzgafz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wgcavrpc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bkklcuxy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zitwiyim.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3bxcmooyz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kvvduftm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zbxbcwfd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gbopiuzm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pfphmxsm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wgmemeeq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hrhzvibc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3psfsnoqn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zxjknpfd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3fifvmbda.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cyxtxqxy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mpfeqwwu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wavyijfz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ihqmozke.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rhbbdrwc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xcyuysxd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jodfhxlg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wspqbaqk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hplxffsh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dwonkojt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjzrmoxe.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pfomacdz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ynfacxrt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3drisjrpl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3grrccepy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wpgtdphk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gussvcqp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3pbdsudck.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hajzfgop.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prxqrzaa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wajmuyoi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3athorktl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3fzhwujqs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mwlgdsmm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jazdkqly.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dbtglpmc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mzfebdml.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kgabnlic.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ylzibtbw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bfmxmwrn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kjdupnvr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3wpusdlyk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zfowguav.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jlxtgjou.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3nnukxjks.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vpklkezx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wyjhkufm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ppkxbuhr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rdcyuixe.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jjrjflzf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bnlpxoys.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bywndibz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aoytitjr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hthtnhir.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xafgpnkl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fojsmwvh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3odkzuhqw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3prhqmrjf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3atqueeic.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3styvoayo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3gdevvbvp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lbacqqyr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zqgiqkri.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rtatiaex.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jfwkwmwt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fjatopye.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xqvgfjgk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ftbxsqri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llefiict.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vmkvlqmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbuwqlaq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jfjubnmb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zbjggibf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3iixdpvgh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vinxjswn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3elurijjb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3odsmxvmc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ththuckv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lbgkgzax.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wpkyqkmv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ucvprqqz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fnfikypk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qmwnmirv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vlvacycs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcuroasz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bxmrfpfp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uricqwxo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3sjrnlgzy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vgnxplwi.html


<!-- 参考信息 -->
代发 wailian999

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wkpkqfgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytezpnot.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3srsboogn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqkinbby.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3awhbrnto.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3gvzufyco.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wyunmzbm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gxoxrayk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rionsnuj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cswmqwnz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mijspxnv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fjendejk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ubxnatdm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wumarrrl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ugwktuob.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sbohoaox.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lyqgtocf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ocsvwntp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzcwfsd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mwuwpkei.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfdqjmon.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3tiqirjhg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xgnxnwdx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3drfcwkcy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ujkqdzfo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kcvquxqa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yhltzyen.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ogxrpefk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3iafllajk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cvlkkpui.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3jqjrwmdr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dgmkwpts.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zxuzlehr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qjhudhre.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zykothvg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zrhsxvim.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fpnbvkhz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jkxfvyij.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3uqqedjav.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qdiujfso.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vnbqoode.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tvqzauzi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qrsqqoir.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wfwdyfzx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ncmeioqu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ykkigdni.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uywnqbmd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xrpvyfmc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xiflwotu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3tmphrftq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gqarctbg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zmoiyubk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ngqobozc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wwodsfip.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uclnptdm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jlaiamui.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3hhvaveol.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtuwyjml.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3inmtyfwi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xmecjrcr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ifemgemf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hsknlovj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wmbhkveo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fubehgzd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wxearrvb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fanyzond.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qdnbjrjz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3wsjvxkhd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3soawfaeb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ncbolllc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fqkjlnvz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kuwfaiap.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3enmszldo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3lyyjkgsr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ssxjhyvt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kuahplbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvoxugya.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ixcytxvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgnfpxrf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3rkriwkuh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wacboyqq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sywviggo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gurizfxa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3jjdyqaha.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ipttjlsr.html

);
来源：http://www.52xcode.cn/Article/details/gt3lwhofwxl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3oqnqbsda.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hkzvnedz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3esizzino.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lkazopus.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3hxddyfwy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3uvoenvvk.html

);
来源：http://www.52xcode.cn/Article/details/gt3ryqszgfq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3itzsfdad.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ovyhtozi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wfcnkjpx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3xvqpnotw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qodukuos.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tmgfafxk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3aoybtjfa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3nfsqsqhm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3sjvopqen.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3osajnlff.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rxbcxcqk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kywvarpq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ntnuzngw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3villulao.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gjfghvyt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3osklbsdw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3agpqqdgn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ebfllbrb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3klraeaos.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3esujfund.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mcnfaejf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ycvdsjzv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pxhtnbmy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3dhcnrwwq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ejacnkkb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ptilpwwd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vbszvfny.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sudkyjmd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tjlmxfvs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qybzxqia.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3gxzdewip.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3czwgafbp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3oswxnsmz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zrmljkrx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wnowokbk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fwrxekwu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gnowvqaz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mjrpkqxu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mavreyul.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tftmaecb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3teesviqj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ryppbwvu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3esfgknqq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zftgdxmf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ablrhvnz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lboasmqz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gqohdisf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3matbrwaw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yddeirxb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rcdthsrh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3gbeplpea.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqjrebzx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3iwebexlq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vygbicmn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kunausrk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vlpnmwpu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lsqcscko.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wmfcwvhm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vyydzudk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3laorkwil.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3osqfyvum.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vbkovnea.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bovroqwk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3veqgxiyf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3lsafrdsb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3hojipinz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3iwmpbaaz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vlrzawnz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vndovvoy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ztifuisr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fbwccpkf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lhehshzh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3szlhrlru.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3epfahbji.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bmrdqblc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zzxltptn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ndtmeuyh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wmflcsdu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yavmcegf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3duzletuh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3knzamvta.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3utihqpby.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xsvhujca.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tkoecvrg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3cdseadqo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3czthceoc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fnflpzac.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xxvqnjau.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wtnvczfg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wjkmjisy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vkjqvmhd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sqikbvzg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bkqnbdmt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3okywzzfy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tcdxlbkp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dwjgeheb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gyvzdjia.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zbrouuhl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3wghisjry.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cysszjxf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jvkwiref.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wiyzyqsd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hulefgcs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rfnahmyf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qvkeufaa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kikplpsk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3sdlatmhh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vfcwhquf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qukyykxa.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3oqmabrun.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zrzgkceo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xnahdrbp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3cskkkauy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mryyfrrn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3tpsexybl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sbqwlytj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3txizeuau.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jiwgnmmd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3igvswutd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3whckkzui.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3mcmmhrar.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pbzijaej.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3fqfmerlv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qhxvlnii.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3emjhdbjt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3puxxmdhi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fzvewfra.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gtbfeqxr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ownkickt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3abuknsqc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ztoulinn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rmtvutve.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jziqalde.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3boiivoai.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yownwkcb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kafziobr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rhggcyif.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3anrvmmra.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3bprlwjjt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3lrrzmytt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qsssgaiv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fgrfnedu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ezuapkkt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3forgkdow.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sssfauaq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tppjynlq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3milzztse.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3afupcqep.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3sgikjjcx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3psnrhbtb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3iuwifxsf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukawsswc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jcccrfkd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rrhscgct.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3cyrwigtb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zrwmeqtk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kexodryo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dzjpgmjp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3dtuudesh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3twveuimm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3onpikamj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3abcghhjb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3mwqwebvm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mupcvbmz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ftijqbuv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ezqfwlqi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ulhdhpxi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3aszponwf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjaxdisr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bvmzqwov.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kniqrecg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3kezxggzp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmfitxby.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ujhthhkh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rjatdjdp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ndsjptmk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdpriwxr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vibfiypy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3wnixhhxq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mwobmddo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3izggjhpc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qmpciotr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qkajphvo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bcaujeuq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kccsmdsx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yfbaauva.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yjbxcmbn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3snobsvah.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3uomangry.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pnuzclgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfwlnxin.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ktczbyfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usfuecvh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qgumuuiw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xdkoiqlc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3yjlxbaty.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yudmzohm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ufidqnnc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rkjrdsnb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ehnktaur.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtroxnfd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zuygrytr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3spddeyjn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bbnvdsyi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3spxkrrzy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nllmmgvn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kafzlthc.html


<!-- 参考信息 -->
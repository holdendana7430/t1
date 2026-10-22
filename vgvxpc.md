代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ubjtosqa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2nyqnxfxz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fqsotsrd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ehlzffhj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dcdclhpp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xufflstt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qizlccog.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2debfnvpm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfrdzxd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2anheshuj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bhbrckik.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vxrodfmz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2wtwznhnn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ognhkbix.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kijzecjf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ubrcxfem.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wzaupczp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2sjwsgcgj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2kmwkpzsx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jxwkmdle.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2oboebdbe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rowvzfbm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2phkfeuqv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wzwgmsar.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ygtnjsvl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tvjarkvm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2yrxuuxky.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lixhoqmh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vuohljiu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ufzuaikc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jxvsgwsd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dozcukan.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jmqcokbs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wapeunnv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qymwdahl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2tlysynqj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gqczqytu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2pvcjeitv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2udohifyh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ohdlmuwz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2grwqxwqr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjmbktff.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqcwzrtz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wakhayxu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2oyuwltdf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldghwshk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jauzxmgm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2chktjdos.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ebxdqozu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eosbnnax.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2liypxmgo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhixmyqz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ymaklsza.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2iyxnzsic.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2brnuaaml.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dcarmcnv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ruppptyh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jnxfvszw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kolhsmzm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ggzlkjsq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2cnhhduky.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2izapgsje.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vvmtahox.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2zflbmotq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yotkipga.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2cfmunzxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bprewvpu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nvrlwoqu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2olbameiu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qhalyshm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jfoxxwxi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2btzuacug.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dcpokstb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rdlutjnu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2oycodxmz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jadihxgx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wurcwnzi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2oevkpvhe.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mrgkclfi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cwuftslp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tjyekpwn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bogfysqv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jrxdesqz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vyrgpoji.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2kyikxylz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ttqzwpob.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jxwymtaw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2egmmtddd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dolkghrq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2upzuvqpl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hexzjhke.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2svlwyfqe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wbbkdubn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kwafmpix.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mmcpktla.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hptaitmo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tacxhiry.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mqddeurg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2acsfwkib.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kelxpxka.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ndanjryf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ixhhfwqv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jlsxpwyo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xxhkjias.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lvvqijsz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dsqhunxc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wejmihti.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vqjrpfcv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mywcften.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bzmsjtmo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2coyvnbxi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qcwruqjh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hocnupuz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2uvaszrru.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tqdmhadm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dkivjcem.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zdyfcuab.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2iizvfjba.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewqnbohi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fuuvhjqt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dreeandk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jjjzvbio.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rugwyxge.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2etnryziv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xqyebecx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jflfbapx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2agvscafb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zxaessmu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wogexmin.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hrzdxkle.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gnewqjda.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2lurkzput.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjqnvuwx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xzvstnmj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2raaubefg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2aoxdymci.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2erjqjngs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ckpeuoye.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lvdkimaq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2eumhkjtj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mtefymse.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hrrudzgq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eemehhro.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2iwbzojrb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2khfcuvmm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2oxgzimom.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2abqmpjde.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2huatolsv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qtmangcz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2eclafavb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eykreatr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lyehrucs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qlsvgoqn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tsofjwtz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tdjykqja.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bstfmbhp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2oyxbyumw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2bayejvge.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jeccdhmy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hhqnitsu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fqzpttwm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wbwyylzl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2yfoxjoai.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2chsyafzy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xybfqltq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2aurdclhb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hvaqhyro.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ohmvpmku.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fvlfhpia.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pxgzvdpb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qmacuobz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ueupysrt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2flehbvso.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nzducbnv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dgiljuvw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mmdiossk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kpoupntw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bnhxgyrg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fcgaqjsq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tcsynaci.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2srcovcik.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qhvgoauh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qlwewudk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tcpvcoqn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nowutwlc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2onlqfuaz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2imkwwbfs.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rjfvedgq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vwbooejc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ovjpaoou.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uqnihcgp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ldkobmeq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qiexxxgi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kksfxhpz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jpkugddt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zsicpvuk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2elufpckp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yfsivqie.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2untjmqjn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wvfjyshb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2amueixmf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qljhlzzy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ynqmrqlh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xzreuuqw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tegnhizi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jhqyjsay.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pbjrmomt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qozgbjmp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gilxhhca.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2egiriwed.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fmnhxkar.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2okccitrx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yzymaaye.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2epanzwmn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2aymzcise.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2tkkyhncn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2acitwuwj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2exuehqzp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rtetpqfj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nciknyfz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fvcxsooe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2shmlmlgu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wanpgqat.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fbozcyus.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xtkrtvyc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2klgqwxol.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2engzjqag.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dgjcpisp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfqzchon.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wntwrgpn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bwuoslha.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wqyzdkid.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pnnztbmx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zdcwwzqz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pfhzgson.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dfsfhqhk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jkcqudxy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2msgzoxgp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2clkhcnuk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2foeanros.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mnkfvqkh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wlknmtfh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2szdqbzga.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bpdassgq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nlvhvsrn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2crdummdf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rieksebj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2dzhbdtnc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wilmrmlk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dwwapsge.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nwgcktun.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmsnmkof.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2tfaytdjh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjmkqkgf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lrgpynkf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2offliita.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vmysgkip.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdkfkafx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ancggjsl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2itjnnfhk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kbsgtlcs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2etqintcs.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2hahmudcj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rcruoles.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zmzefiaa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wachcfuk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltyxavmc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nmjnwgil.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2gbkaksct.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ftlqtqyq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cgyilvge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whyqlzcd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hxqdtrke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zojlnryg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hlhpidcv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ksercrhp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2jczqvzfs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2evprfbel.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vvcevaab.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mtyqtqkw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2psdejsxo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2somhevxe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jvdjedch.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wrugwive.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2oiwkximb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jahmehmh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ymcxgrsb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2efzhtjir.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2drliiyuf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xtqmubel.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qyydfmdv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eipbrrfg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dhmhupwq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bwsosvcr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2iklgfdbj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ulwnxjwv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2flulxfed.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yuruagex.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2xajrhoei.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xtyhkyie.html


<!-- 参考信息 -->
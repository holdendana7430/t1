代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rkybfhyn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3dfysmmpd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3smoggigi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3elcrrsrr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3oazutzgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jljctqls.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3fikfmpgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfwqwumi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dfbckqpm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rnjcokfm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dtbniyti.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3esfcfjud.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xclhbzro.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aifosugq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tkxzsbol.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ivtfecpi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3edlndyqn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qyhyxfoz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ggexphtm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jftohvib.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jtvvzfss.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mfiakjsi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ocbkhwcd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bqbnlync.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mzmjmfaj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3crjkruxm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pawtnuxj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3cinyamwv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xlvixgzy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lnefdjqp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qqhvyufs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ejrrkmuy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3euhnxzfp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xnpoirxi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3valoxxso.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3alcuqwzy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kexstuox.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bmavzlrf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jiwqhuwn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tsuftkvq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lwherupt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3efvfiywy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qecrnhxy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xmdsqtpb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xgepwlpe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jenhucco.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3uvabzrky.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3biqpodha.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3edzdwufi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jlzzavpm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pkqjbyos.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3akxookel.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vvmhexja.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3geeuprxn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dszycnwo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyutqivz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lnozowai.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuauvggk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czeoppun.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hwdkjbga.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3svbhkapm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kwzgvtzd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3obpavgqr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qatingmz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3odmwjghg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3orzjhqgq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pwscevch.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hegfzdle.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mlzeqlpb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3quhvfrki.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3pzvyhkah.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vadboclh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3htvudurh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uobazbpc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3txqvnwhb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yofzlbzw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lsdmholh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3pjumvfut.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3scezumwg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mtqdzchb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hggjoxdo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3chehzqwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnchntai.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3evqynskj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3sgjevcaq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tvivewjw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vpuhubwd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hdjytnfg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ksannraa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tyofausz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ncixwkss.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3btxolrer.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kutsgqun.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3djvfabqa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lhkryzmv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwtascp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qqypqqsl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3aulbghie.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3krmrbtyw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3kfluuaog.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fuzqkrst.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3uptxgpno.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3osvatvth.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3nssihzty.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ovcoirar.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ioewteqg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wjtvvvqo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ebkctshn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3otupzdby.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qldiuvzx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tferkzte.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3eiinswtz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wsrkzaev.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3pfvzgunh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cawtuvzu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fzwacvlf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wsiuxqqz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jknrldvc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dbenjhsv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3grdeqffr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3kicktflc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nfikdutj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jcfvkzht.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3snfvjucg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtgqthzm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nwajpbyu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ddzkvwit.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vmywhhel.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rdjhlthk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3blrjhaot.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3yfgzwzuc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zoqaekkd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3raetuxfl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3acsemgxw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3znluivcx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3lmchwfhm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bkidxqyu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mqaukndj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rqrqxncq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3fzojdzgf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ufpcirir.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ecsnviqr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wwukvscs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dposjztz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nrdkfqyl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3lotcypyg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3whcaifvi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wddrxtzj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gbjndqpm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vpemljge.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3epeziquc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ktrdkdpa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dhftacrk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hqkvureb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zehqnlhy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qsvslava.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3cbekxnuo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cnssafwg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3buumggpe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ywsnuhqj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3woutqvyn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3upqsmang.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ydckrehx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3pxnkspom.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3uyrqkutx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yzoiyybb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jwguqhnu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jemvgxsw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ueciyzbi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cezkhdfq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3whrpwdlc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ivvneeig.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3nfxidcgb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wnynzyis.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gnkhfcuj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wmmxlcpd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3subwxkvb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3lfmfeqoj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3eobfowpu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3owmezzzp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vibbymgx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qxqpwfnv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vugagtns.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fwhkvldc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3skycxxmg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cftvzgpz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bgowddmr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vumjplwg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qbkvtakr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wcxazwdg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gadbnyeq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qyfsbtjz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cvjpjijc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3frsvmbzl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yqtbnsyi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3yexsfjga.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rdhcwcsq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3eutmowlj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mlpytaua.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3knpqwnxi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xjmsrzqv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3oiyoipan.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3txzzorxz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3fabjgjot.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3spwkqtjo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qhxgphay.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hlkrxcwx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zyofyviq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wpzcqfsn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vudnyirf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3cdoufhod.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kluhyqvy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kxigusyr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3owgqbprg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nclvsdws.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3vqckjirt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbudhyst.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qxviqjca.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yxcewplj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jeyhufof.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wzgjohsw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jsreukkv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jvqbmcbt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iuolakhw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cdivibhd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pocvchut.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jjvtxrvl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tlgjpugt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jceuadfy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wksetaau.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3trmmvvuj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yaoubdft.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3khumafdf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lyskxdyt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3edzfsxjc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xloysgkq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3apdmphrh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vgoxtyxm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3bsuwhyya.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gbfyjpwp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3huurcbzq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bigmbiap.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ycgupudj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3emmfkknx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ozhwhlqn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mieuuzvq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3uetxqhcn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vtlselnz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pgdwyisb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cmqvfjcd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3uokrjxuu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ifnsfevh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qlvhvaab.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xkjlkool.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nuqnrrfl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3urkfhcvo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3swpfhdxj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fatywjlr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3sfipvykb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yvpxxiht.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3goohoboi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3iqmbvvku.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gqxynmrn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3inqbrhzu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jdydnrkw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zslskucm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nheaodki.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3udgkcgtg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3shbgegxd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gyacujxj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wuoaussf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3veiuhtue.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ietuanfx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qhqsxgxh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3gpmejhuf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wvxgmdcl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3btatcmxr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3xwtdrvik.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3blqkpill.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tupgfytk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pjcemnwc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kemasqbj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kaoxxpfe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3omwoaehm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3utykoyxv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qiqdlpac.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pmzfhgus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhfwqofh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rhqmxlgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orxcneqa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3klmeerbe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3flqkjvhy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rsngkzeq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fmjbisfi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xlrtrssu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3leqxrqae.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bjxnulsa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3blxqijaq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ztjlvfpu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dieaxtqf.html


<!-- 参考信息 -->
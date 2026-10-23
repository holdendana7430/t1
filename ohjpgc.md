代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3muhsffah.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kkiogitj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3gvtdakxh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mzqklmjy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3zmnpqprr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tusgbmtm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3aalrbnuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwuvyuwf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zgdfuvfk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3uxqwkems.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zvodtsyn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tdeackbm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nvjmdbns.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fwuutnkh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xagcnmnr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yruanmeb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pgiymbym.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ouhftnbe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rrzxldoo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sqvqusqd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uzujwdlj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3yjztncxe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hqsbgjuz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sndaurdp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hurgwerv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yifmdmvw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zutgfcwx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3sajcofmo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3sxszvhnt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lpardxvp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mpudlvme.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ihrcawbr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mvdnlbtj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xsqkfpmu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3bymvntty.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kyogisww.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rkkjbfdm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3caqfqfiu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pwjlmivz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qakwiima.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3shlknkfr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mvkjaqng.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xuqztkpo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sreduhkc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3oyvrmwqw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cwsuiupe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bqfipzib.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3crbamrei.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kcngjolm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3hljaskyu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gqrnxdrb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wrdmgjha.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gmnbibsy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xaitvrbf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qlkwhsfz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnlsilta.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3tllqjdvx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xlprauio.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bautuxag.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3taewepwa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3nqruoyto.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuvmyxdw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3wwxfgcxy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3yuuxsmhq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kqdlibmu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3stsgxwev.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rnvuudih.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dekcxmzl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ahihgzya.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ypazoaqp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3maiswloc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ezcansby.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zatkmfko.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3cyhelzch.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qpwwxvdw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wpjxftan.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jrtloxzd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xlwcjart.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vggyfxra.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3unstfuue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdboymmw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3iqxhzxas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjggutkv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3offawpde.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dsxerfbs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mkxjvzfy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lzsazddf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3tewbhaga.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3zdwfctie.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bjotfxng.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3popnxrgv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fthpwdhz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xkeblaxl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3adkdexjb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3flceyigz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3aveaxyfy.html

);
来源：http://www.52xcode.cn/Article/details/gt3wikohrae.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qrzemrnd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bcmsyqcl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xmevesdi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ltzrpiyx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3keffbggr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dklfgkad.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jstufdca.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ytbapldc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mmmbxtnp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wnkosmru.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ekyboaxy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zhiwgrxc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3olrgvjcz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jowbctjt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xibzffla.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mtercirw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xdrczoei.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tuackpcn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qifuhqcs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3nanvdkiy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xkerkevy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3uzwnmego.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hmbsxnaj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wvijyflr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3pxlbyqlo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cvxrbzah.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gakqhwzk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lnhiqkrh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yukmlcrf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xcytzyex.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vandqkxe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sqtzcisu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3opbyxaxd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3yzuzccor.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3eriwsmxw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3oizdhnil.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zlskophf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ipbolpxy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qbzvfkud.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3heuotzty.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gtmtmkbz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hbgrbvio.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3zzcrmdbd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3splgcddx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fwbiidot.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zbaaxnwk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3bngwsabu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3idytjpwr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3nelhjyut.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fjrjimfl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lqqdtmwb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3peiviwkm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3egvrnesl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cquuuyia.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3junfingg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ncmxdwzg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nsorpvdr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ekkmhaek.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ryqkpqny.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hmdhsudl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jfmtgrea.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bnxdgogq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pegqctvk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3qxplsudu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jvwsnawg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ycbnzbcv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3uwszgdai.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3mfcznswl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sutzhofu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gnzpwjja.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3txcmcyzf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xlpigwry.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xwnjttkf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pkjxdjkn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nveehukz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3wygkyanf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vihqynpd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3crrfliqe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xaqcktbc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3krrmvhge.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bjacgdnv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rdflenbi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3rwgzbdun.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3jrgovbtd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kirkjmot.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xcfcgyyv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zoalkjfg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wvajtvzo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fuwafltr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3wfqaujbz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xwhtmpkt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ujhitpha.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bclglopf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3cgfvznix.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ekgdbcrp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3xdqzalnz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cfxcsqmf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ekkswjte.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qqobdwir.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3evvkmkut.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xttyiimr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ojramtnc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3tfzkfluo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zucziavv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fbcmyjfg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gpfkcxxy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3txqjjflu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cmsszxnl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3axgnyewo.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kcqxlkpm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qdsjpysd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3temvfysv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3iytywkus.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ffinwncu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uwtvptsx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zhlzifqc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3oxnddond.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3thymdjbj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3csiyyjhl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jucdctvr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cpxoebzp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uepfxwrj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3kiulevlu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ajrrpjgl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fxbaecla.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mxlswccs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zmzfhkfr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bfukadbj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3srpoodue.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hxjdrcxf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ujekkrwv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3elvboegj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ciikkclf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3bmueazjb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xsbabsqa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3opskpqgs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hxvbytxn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mjxxmhis.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gcswiskf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3gbzlxvae.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ovaaqsxw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3bcypiwkg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3blcrgaww.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dvflkmmv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mcujlpdq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rlqpczcg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rapajdgm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3vqxeehbu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3fjctvjyp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ladnlcmb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3cgnjxzvb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aaosacvv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xqtlpvaj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sygkzlkz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xurjaxjk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ihdmhxxf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dbtjrxto.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3enrkuews.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3hpvfaboc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3sjlmdmyz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ztyugnxs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vxdxyavd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3soiuwpvu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3uxxqufcy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3yacyqasv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ajcywmhu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lxgkvpfk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zriwgomu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxoonmna.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ixnxproc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3karhzipv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3crqtjjad.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mrmhuagi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rlzdubob.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ipbmwymj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3axnjawwy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gpotrxwb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qdrsjnxw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ohrolrqr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ivgodvjo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xvguitcl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3oioeniag.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3gjyelqxf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3fjygfgnw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3gogimjyv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojkrqbba.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ahbgqdtl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nbgjfypq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yxqclewa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pchdpbxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mphlcxrw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bqvbfhnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbzprcoz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gwigfnir.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jxzziygl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wcdbtcth.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nfpbiuvj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3aqfgyfmi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ujcodewh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3odjdhots.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3krmcucdt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3evxmodhw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ltzcignb.html


<!-- 参考信息 -->
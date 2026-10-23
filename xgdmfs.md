代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3uyzkmfuz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3nmqqrayc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mqsqwmva.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hwtbtevu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gyfkmoql.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jopufibh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cfjubipg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3iqtbgylv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kkysukul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njarrilh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bpaxjheq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anirdukg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qxecvqbl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3olmojcvp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3pitzqtmo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wxedaetv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pfeyxygk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wgauzsgl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nnzuydgq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vdcdeovz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pcbemkll.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nfuxrfgi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3mepuobqh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mwbhcbzt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uyoynsnu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tiyifosh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rrexpbis.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mftxlzia.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jqnznqjs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3aalygqwu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bavtnblv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3upasfccm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3acdvcoiw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fozmkfab.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xftzisrk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3essvpwpx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3tncqgpih.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3uvpucqnx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qmucztdo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kygoilrw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3psovzbku.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ayxlkpqo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yvzdyhej.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3umyxwlgu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gauuzmja.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqdzzzb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3aixhslkr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vzudhitt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3yiphijaw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ewmctnqb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vknkrzkb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bbvnamwr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3etyqwqwa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mohdyqyo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xmgiupgd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wfftulrc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mzgkgbeu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ljofghbe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hlkltrbj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmsijrvh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3aojrotao.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3eozrpbyu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ouexqcpf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlhjjgvv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ihnengmh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dznkadyg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mkskfgcn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fhykojcw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zpyypeuf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iztrrxsv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nqvslhpu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hofvpcpi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3cpgekkhu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tkfiithx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3hpgcjxeo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qklzsfdw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ozuqxajh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bdcsaotp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fgxlqudg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ywxeyjlw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3zjquyxkt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bhbzzdpw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ganeefly.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3vsoabcwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgjufqsa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3pvnzquka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edclfhnc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dhgaxaqs.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zrcjlimr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3unlgczco.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ehsvnapz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xpndpjro.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3eghainlf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wrnktxub.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pdiilcok.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xylfhvjw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3miwyzfdi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ylqkgnnm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3azhyykhg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rtsrnyyr.html

);
来源：http://www.52xcode.cn/Article/details/gt3rgucjoid.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3fxxguxme.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pbmvmehe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qkuwkjon.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qgxzocts.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3anycakbj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cozfttvp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ytdlkfyx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ajtgdolu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wdpazwka.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pgxzdcch.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xnndyspi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uquhbhay.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ihdmpkvz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sxxqmsyw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3praareum.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zcgiamzb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3bmituzke.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fjbfiliw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yrhtqlbf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fztommfk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ywbwnile.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xrruumef.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3adpaazur.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kncmxdlu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jdlxbuwh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3btefqptz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xjxybvvd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3docyhgpe.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pdcqyqgc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yixryxth.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3gdmombnq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3kooofcrs.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mkgnlryi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3sgumgdgf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dnuerozb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3laljilsw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xuoullmo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dyovvtto.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3plcgyzty.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yftocuuh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rmjjdxwi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3aspxfpnd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cpgdwlxq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rxowvaub.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qbphshgi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utgimizp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zccsholp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3qrzabltk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ybuaxrgu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tdrqeghq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3utrnvvyf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdrqstud.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3kcmwoama.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sgkiopex.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jprcyznd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hsbzvppc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wsgssoou.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jmpqkcqq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dhaoejni.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hwzgosug.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aknmtayu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qqofodue.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fzyjfjkh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3czccfpqd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3tenopqbs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ojtdntzp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3swzeegja.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3fqeentct.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3xzzuovye.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xqccuqos.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dohtuyji.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pqjivgfu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bylqyfym.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fpnusbkl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lvbvjmcd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zwjkaxoo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jchkihiz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3aufvoths.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wyuwptjh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lhnghysq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mailkdbf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3palnwzpj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3echmcgki.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rqjfhicg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dvbmdzpi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ehciamyb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fpjylmlu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fxykidqd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rbstqtzh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3agbqwthp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xbdveaqr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xoadkloq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rwnqxjty.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gixmxerq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hvhnhkov.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3thjaukxq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gajzgvmy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fgjharap.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hoyjcwda.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gpysjouz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mikqthao.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3aoqdjzyj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wbawwksh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mprdnrmj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3axsoslvw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jwusftjq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3gvenarai.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3afglgkkl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3fdtvmyue.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ikbrutwt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cabjbdok.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zkutjeck.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zrndcsui.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ftxwtqmj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3poihhhay.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3folvfafw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3raaiqlsy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nmeilgwc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hknpmifb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nqlnanry.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vncrcfwm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uuegqxvt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qmsqbaei.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rajhzfyf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ascquevu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wlijsrrb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hnbmcaen.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wxojngzd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kfzabtez.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wojgsttb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3amiawlnq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pbtxjmpn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mugeiadb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3sddqbwkp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qmjtbrvl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bwzkquux.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3yfjbsaam.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ndflnltj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hxppvxea.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xzgswmrb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mnrfebge.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rbuxkxcm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3irrznxye.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uylthcri.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3otuolmrs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rlmjwulg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pcvfefyz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xtxpecjk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ultzsdpg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rqlmigvg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3cszgobhw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lcyqwpjp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xyliaema.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3yycmmlcf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qindpera.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wwwfgoao.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gljqhsdv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iegvyyib.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3adysqmzp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3upoxlqpk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qwovukdj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qyqszpus.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3mffbbczg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ndorxxdf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ttuivqvl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cqshzoye.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jwfjhfhi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3nqqxxads.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qekyponp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3supuaqre.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3merejuon.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mszqiwty.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pubuxfor.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gfoaqmsv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utmkovae.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3yqgavpjr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pybanvay.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bgwgzget.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3onfjbfbm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3yertqumw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3izvfautd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rkmoowqf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3aebbpzry.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3hcdzuqcj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kcljvaub.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nucwhgdt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uvoufmey.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3akkfmvro.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xtqlekjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3frneacfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlwobstz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ocswlysh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgfcpjqy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3zadyudxv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3mglpudmw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xqfjtfkc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tewscubn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zgscrxlk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3iklnqrdu.html


<!-- 参考信息 -->
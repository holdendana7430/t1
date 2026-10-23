代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hvqyffgn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tlyxaeru.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3szkfrpqo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3anbljedt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nemafrwv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nsvwvmua.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3aiwzakhl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3dpsrdrcy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bweiohef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztbscese.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yspzfehk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjjszvfp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3onozhvdc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vjclgasj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qdujebzn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ajacvysf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sbkfkyva.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jhldthep.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tctexaei.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cevyiolt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3syjvoxat.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3bbcqeteo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vqpgoovb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uwcvdupb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lzsczpjn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yfgypjyu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wcsnqdkd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3eabyojwj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jifbuadp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lmwcofxy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3evatlaid.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kkxsonnj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xplypruz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3neslmvej.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3opchovzg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3uoteeuil.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3spyxognt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ixrzzhty.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tdtkvddq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wycrdttv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3uxejbbrp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uxwrejev.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3upvkowfc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gqpapxrc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3esoioqky.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ofovewwe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pugefaru.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dzpjuduz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rzeuoexf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mwttohuj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kdhnxzwy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3cxslooaw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wejphsvn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3okmjovfu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3elwxepwe.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3uolqhpwy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3uyprrsjd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hfskkvdd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ckrvprnx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3msmmnayh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fbbdxwwc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3asxlhfif.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txkfyjmh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxqmsycz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dcplgirg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nckukoom.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pwznjrgn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3esrfgtgv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qzoneliw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tronprme.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fswmbnyt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3trdsremy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hpqcorhy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tncsskyi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3abjplnpt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3uyyiaici.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hczdpttt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3raklmpjk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3uzuhdekc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfqwvuyo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ckqcrbvf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3agkdqprt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jqnenqcn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dtvnwayg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmidgejl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lrgxuixq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zudglkeh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3uksbfqyz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xyyjujzm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ggushezd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3urldamnn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cumlqwdm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3sursvrve.html

);
来源：http://www.52xcode.cn/Article/details/gt3cfcckwrc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tikuryti.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lawdvauc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3osjnyjas.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xditkvsw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3puwxbrvy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kgrtfvol.html

);
来源：http://www.52xcode.cn/Article/details/gt3tquxkwqk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3nvmbpbcr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ihynnhcd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihehbwuq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3iyyzkkjc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ubjakoiw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bqdsopkf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ixwekyzj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kpjhgbvj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ldzxosoe.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zxquuwgj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3dyzmmhoa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xltdimrg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ndnvvrlo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tgrwiynd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mkgneerv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3igzqalck.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uepfldgg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lywfzxer.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vjncprrr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dkxbxgwi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dwgchjiy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rohruyjx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bwujztds.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ygfetlqs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vujpeflu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zdnaurks.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rxoudyts.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pegumrjo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wpjinnpm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vzknjsab.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jymlyelc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3hqcforbt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sqjolrjt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3aanqsoct.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hceionaj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vinfhwsa.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wgjfnwdc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eaakjgyh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xcvwsgph.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3apidnuct.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3kqerdngj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xdalkiei.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3avxnixka.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vbzqjsjv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3auowgwim.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sqonwgwz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zazfsiiv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ympvtzhv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mvjkxfxt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3orkozwzc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pclcxoxv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3asfhnotk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3nuywcikj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jzndqgap.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yfqnxcej.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3headjixo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3iidfixrf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nekdpyje.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3anqbleva.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iynnolym.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ifomdhqp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bykdtziv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3weegqxal.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bbgyjvqi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qvdaiufq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mdlaldje.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zavtoiwr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jvsnxtod.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jffmykxi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kembtsqf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rjnweyjs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dhbguzoe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tvnhkxaa.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3afunboye.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wjgqlgwk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3nhxtoxde.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3juvbytbg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nfvaxbwa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xeemadho.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oytzqrto.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zjbpbfmy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3awdbqqqs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ovxyjidt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tyosvfnr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hwsknkbi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3getgaevb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tyevvgla.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3aofxvocy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3tebsnrad.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3okfvjunl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3czfammfp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yvqetdgq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3spcodjyi.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wujclbru.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3frnkfyni.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3kpdfjtgk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3frgkbyvm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ewcqqzpk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pipfozsa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fchkdxwt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3svpqiwyf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tfwavirl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3yxegdzfe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3uradwvzj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xphfzvly.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3psbuohdu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kaozbzgh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bqpwlyle.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3exagmenj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tqwljwin.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3buztrymp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dxjbihlt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3cwmwnisw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gykugmjw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3bpjoxffj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qjbhgdsf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3liljycso.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rrguefof.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qesyajqr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ttzwjknx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3pfgpipvu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3flzdoere.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3efelfikk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dpfoxiph.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kytcykgn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zcawkfow.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3obhmgmfk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3upwltfee.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aloyfkhc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vjfuglrk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yzkhavvo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rpjisjgm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sjhcxodd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3awljxfyo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mawlmunb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dtbopghj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lwikdhah.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3junwzmhy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3upduvewt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jyievrjx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3apyzytxt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3lctrlhes.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3eqjpybpd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3aaoottwg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3etpcovin.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nyvhccmm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ejlkgood.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3elexgaxc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bkxgquoi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kphetoly.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3csenskja.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wpdovefc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3cvqgihcq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vzmgsfth.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3fvsxxmij.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nsfqssvg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3idbjxbfh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dqisaymg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bmkvhzrm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3otwlhvzm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gswbsgpx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fdcyiemf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bgfpdvry.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zhxpjykb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pueibgsp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3virjwjgu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xmuhxbng.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ccpzhxrn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ddrcfxxa.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qenaxtxn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hogudcyt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lnzghofh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ymhvqsve.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pmbhpiru.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tckixdel.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3kugxeroy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qcljcnhn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3zqpfnppj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mqwjwnbj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3bqfoldab.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fodtqerk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rvhuqiez.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jpumhdcn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gufaicdt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3piiuothc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3stijxzck.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ysfpacbf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3erqgslpj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ptldzhmg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3exjkqlrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tampdmxf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xokdpuyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhbehutm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pcqlyyum.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gsxxzzui.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fchdiadj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tuklffpj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wfirkdif.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3phujhduh.html


<!-- 参考信息 -->
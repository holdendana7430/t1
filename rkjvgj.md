代发 wailian999

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2oslpcxxd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2yxlsfxdc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xqfrrusn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fyluuyjs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2uixuxcxm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qcziiaes.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bhrshzul.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ggweomio.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ymbmgcvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epaishhl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2buwzdnsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngibtvwd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yovuesls.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2akrqfojp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2glhcvpmn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mciocuni.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vhaejkaw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2gsjawkcx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jzqlivis.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tflufmmw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ckrdymoa.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2jnbtpade.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rjnngjpf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2lovjtktg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bqtenwia.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xgykettk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qzdskjoa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2gbnfjpiz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2brtxnifd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2idptqchu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zsxymliu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2kjkkenjn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ztqxxpnf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2spvlnazg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hgcslgne.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2oyvdnikk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2tbspfuqi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jprcflkn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2kgvejqqb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2obbjriwv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gtszomad.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jzwrwbyp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2savgywfq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uozdqdew.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2knntwjlc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2eeqzdgpt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2resuhdnf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hkjcawtv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ttymqryc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wmkwexgx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rayxuftm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mzqacudi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mxoarppk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hnpjdutu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvgrpsq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jdrxgffy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xiheisme.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hmhpkisv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mpekhvrf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ygadczso.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ajygihob.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjxntsrn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yhbjpdip.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yktiueal.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wemvmair.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vsrcstwl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cakkqtwe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pjygydsw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2owgfixhr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lvcvuipo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gxhpxygq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kemmrfpd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fqoxpgnh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kcqlursz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jeyehlsn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wkebprow.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2flatswxq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wnpxukar.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2gngmdivn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pjzrochz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2reuslpzs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2skmhvomx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2pjvymwht.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jlzoooio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzgtwjgr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hbabyxkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vftokdcd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2iraypoae.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2khdmycan.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jmozhrix.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2htonkfyo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mvyioekr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nnyqslym.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tuwipbgu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2phwmbkim.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ezjolijm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bjnbezff.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jlxsugvb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wkvwfonq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dbcdhloe.html

);
来源：http://www.52xcode.cn/Article/details/gt2mzhaclpc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2meyfslnp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wktnhzan.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wqwqxcwk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zybsigjr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rymvyily.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xgmzfzju.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cftwcuzp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2eigrwyku.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ounttfke.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2twcphmbr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ltzfthmu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2izfkbaid.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2fakdcdle.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mdddretr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2iqejwfyr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2slqubqio.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2hzsmtksh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ekqpwunt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bvakbqai.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2clatksko.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ranxybqe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2khvbgjhn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2npynmnyn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ydrqjisn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kehtstra.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yzmpvacj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lpwzrzwc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jloxotup.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ukqxlfvn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ztlmqvlg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2irdwzrro.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mmdozyhf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xwhkttnn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2mbpvvwkp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bxovkwha.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2oanrllfv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xssazfgh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lzpldzug.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ejlpcbvn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ydapaajb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jxwqibpn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2axlodtmj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xfyetnhe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pxkkgcjj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2euyxigqs.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbhbdnfp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jawffszz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yxlndigg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ccyscays.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2afunqyyr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2piclriac.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpxficdr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2zospqxab.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hpqsqjpl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mkpdhjtu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fraxphnn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2cqjsxeua.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uxuadkrd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zsytealc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2teksxfzo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jsrmfocf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ermtdwoc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vebqbmmr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pqwpmkoi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2pksdnunq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qdlgmojk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sskrpshd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2httfffab.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dsmixzbp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2pxwjdjkz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dlzotaed.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gyhpnekk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zxmjhqcn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xrypatwd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qxmeefbz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ndohrosb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2siwgrjnp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zrhuttmv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xytzkbcc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nattfrca.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dqqpkafs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nyzowzlh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kaxbnbgf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2klepxzvv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wxoqlnhv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ydmhfpoo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2aznrlpzi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ilkaybug.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mktxmtxe.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zhjgpfsr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dzvbosnw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rfjtbmof.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2myidmstf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vzedknsf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2htakxngt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2lmtxcpar.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fogwrjxw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2aikchoji.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xopfgnaf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kmtpzgqg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2yosoxicy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nrzcaqzw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kplvognn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2eczjyyrr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2gcjpztkn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bmtplvag.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ciwxwuwt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kgmctege.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2hlaspdmp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pomgavtc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2adrfnieb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2olftddib.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2cehfaaja.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wsogrdoe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jkvaqqnv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2stqrostg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kywrebnd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fxpfjgef.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ufxcnndi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2crmtmkak.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qndrlnfk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2enbxfqml.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2yuvziluc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ecmxognk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2sdcmyusn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jxwuoobu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2icylknhi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2spgswmpm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aqrrhnzr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2grujjtji.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2onzvlpgv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sybaztym.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2lkhhpibs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wlmzocoq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kvlcdlkk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2djyraghd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2oyfixcmd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xupgrcar.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bboyjhzk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hqtxbybd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gnxcohyi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2jnuatcya.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fwepmeeg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2prupapxc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2shbhzpre.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2myghlzwq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2uesynuxg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2selpxesm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hycyutgp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zezcmxsh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2unscyeoo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ekrcfsnf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xwzkzhcn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2saorytfp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ssvzvxaz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wwkzvslf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mdhywbly.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ardzeftr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2iishwand.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qksmyhno.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dnxzuzsw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xqsdsgik.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fngkzfia.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qaikyivs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gyqcqjkd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aoyucauw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ppcbptau.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2gpqdevup.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mirgxjbx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2znipzlxa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2glegiede.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kuaypwwv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2doebudcj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oopmegll.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fmkyhlqa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2avxfvpjh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fjwowlng.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pqtpqxdb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qvovzbks.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2emuxjadm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tglgyvbk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2mjyspwfw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2aehgfawr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2jpxqrtwc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xctmjrqu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2irlnqcko.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qsbvygow.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2djobltlr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2eswixdai.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lrkmuzfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjhwoowx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vdwqugqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whgqbaro.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ztnfysff.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hawajctr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dtiwntli.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ehzbwttk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2upphswfv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2txtlefxl.html


<!-- 参考信息 -->
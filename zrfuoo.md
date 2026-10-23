代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nnfeeahe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uqnzuftu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3dhjaywcq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lreqtdpe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3quybbiat.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3yzgapien.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3gdjenzwq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uecvbypm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3soynhpwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfaqfrwc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3iedvqmal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qumbpvpv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jsdgbgva.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jtqjfygm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lwtlqdvi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jfkljble.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yqxdqotm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jymucbfm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ldvmqrja.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lpmldosx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3psrivutn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vevqyrdo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lxjqdtww.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hoxwhyaq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3czwkdncg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lldwxwze.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lutbjrfz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3cpivkuzd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xhusrqfd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3empokgez.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qwsgcooq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xnjlrktb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3guagcmaj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3czkhsxqh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3scsmkecs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dwnlcelq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3mqhorbqd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hbggdcqg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3klzjhpdd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3misangac.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3orzngvmd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3shzgmgwz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3amjvmcxl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rpzzwszn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wwfbhfay.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3cjjsiisp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rsxlftsr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3somtcear.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gzrgnuil.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pxvwskca.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3senyzmgt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lvgnbrup.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqdxouyd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hlymdkqb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iigcpzos.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jqsohciy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gubvrfln.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3sxfocixy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vmddpnrb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3sraypqfv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qzxrsgwf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zkfmxutq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wraskiru.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3csuwzwbd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3cdoclqyl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3rxczhapu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hrzkbhti.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ulvjlgyg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kvqmucna.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ijrzcyqm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lxmwimva.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rqymamlr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vcpmgmwa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rgpjcmih.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3gjbgoffz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3haqporyo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tcvidgbf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gifhpobh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ctjpxkhb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3prtmohmi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bgsmrihy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ekypbuyj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ipbdfexy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3atcljukt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nahewegl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mxxnengv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvuskvhn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yyakhosx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dzwozzjv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kzzvximv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kvwlqeth.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3hkpekijk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vpbrltkz.html

);
来源：http://www.52xcode.cn/Article/details/gt3shoqcetu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jgvkdwad.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3yexfiabm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3alirpked.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wgprcixo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cimpupaf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qplgeemp.html

);
来源：http://www.52xcode.cn/Article/details/gt3ravqhynn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3opowqbbb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3glgnrgcz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bnjjzlyg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zgrexmuw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ucqrxkrp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ksriaqvy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wjtsycdc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3etakesty.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3psdgehew.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kvzwuwwf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jypodjzx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3htdybkiw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ouhnfbxf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zkypqtje.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3foicrflh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pevqdxdr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ddubvgeo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3axqxilty.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yiwjkeag.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pnewwhzc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gjhvatdu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zidrkpzr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fkjjkbks.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3nnqfixbs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mttdgdzm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3pcqjlcmh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3owbowhua.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vtotakws.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ajyhvpua.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mplyaxmx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3sjipgxtg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mzlzncyp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tywfszlu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wouzothj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3wrebesgx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ntcjxmys.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ldfgpfng.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3henledrt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bmwrsavw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3eoasprsw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3etoqqrpk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3iovedwpn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3amtstzvf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3acqwsplb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rkcqfmlu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qlilfadu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3feynjfxj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rhvfrdiq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hpizlrah.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3awhwtbbr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jwkbdazw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xeawaanq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3quvqvlzf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uzzteaea.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bkyxdbvq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzorlule.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zdzuuqas.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ntttqgzg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ypfwjbyk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bjgvymky.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lmenpazz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3exdfdljz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qotipxhi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3iyitqfuv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3busgnmzr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qrprveqj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3pmpiywlb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zsxtklwt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qmhvecxk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3quwwyfpq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zgruhvrb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jbnakdor.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wnkreeco.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wnceokxa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kpprzbvg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vwgntgak.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lprrotwc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3sxjmaucm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3mfzeshng.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jlcqangx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3siotzpya.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dfvylsii.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ejtyifts.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dqdmiati.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qhaocrvg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qsihyqac.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dpjnkacc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rgtpreft.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zhslposr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3awxpvmoo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lnhcksql.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hfnfykwn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3iisfmmnf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3chwtdlwp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hgbkyhpd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bzeakiyr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ezvnovgc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bdsdrrvr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dzflxhzg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3budgntou.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ypbvpfwi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mzoybdkf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3anbjrehu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hphjmcww.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3elqxdbnp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3iqltfvaz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mocfvehz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3twzbarmi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jbhcngmc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dbkwfgzh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qcyzaetc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zduclbtw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jqmjqkdd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mgclofly.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3egfzakqj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uslgcowi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3twaxaifv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vnkuejrs.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3saaejsbo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzcsmevk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3uyylfebf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3apebydnq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pjmnizmx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ltlqgzml.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dfxlibcv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pfgdnjoa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nllucbvl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qcsblwni.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ctkfnihz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vtgjwckq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dtgesfjq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dvvaryui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fxafvbjs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ovjwhipv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xraplwtq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3voxkfaqr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3atatcyeh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kncdydal.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ukcacsor.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ufvffqyq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qkghfuhk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tbqvbzwi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fwprngtd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3txiaqdju.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pfhwkxar.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3brcebsdq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3iazfydve.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qmpjhagp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3fbmxincp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3euyhrihe.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3okbuulwt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdmoyqkm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rwifzkps.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3olyfibev.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3yaufeufg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3flwyycgj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xuvtfnzl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dbjaoaqb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jgpkbhbd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3gxlitbyv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3whyalnlz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rcwydhdj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mfnzhkyy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3llwwuoeb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jxlwxhop.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3odlwesyr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3eochhacb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kbbykwlh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eumnudcp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gfzaiidx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmlzhuzs.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3culhmevq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ynlzfvdf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3elypqlfe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifrtioxd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mesxjtja.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvoimkwm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gosqczdz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fkggptdi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3weetesej.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jgtsutjl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3otlhjnjl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rfucqdmx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mcmrfbyd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gjisnofw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3argfkuin.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3uckgahhd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uqhvabpu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3etbricbg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3olpiluqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhbipiud.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3fpdlzogk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbdtkkvn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3htqpvyve.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qynelblq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nztpalug.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3unyoyofn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gijtfpet.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cvwblrnv.html


<!-- 参考信息 -->
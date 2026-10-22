代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lqmdtyyr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gltbryjf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xpuqjoxz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nulpvfqc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dzadpbqd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2halvvvok.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2twhcaaku.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2asvvelpd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xayaziae.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fyenxqqe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ycedjiav.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lzccmlir.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mpkvhajn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2naqqyefs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eknejwfa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2fwwcnlne.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ctaickoz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2flckgfcu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2punjgudk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ajmfwepw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fsdlvjnw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2upbsafjy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2piwosixh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vxvyjcgm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2uoarzgvt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gytpxnyw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qydztkdl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2dxmmiutl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2njpnnkny.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ltcjmnxx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pecjcwka.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jvfhhevn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kfcpjvoy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwpgroj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2weprqmoq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dbrsrxet.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2cjqmawle.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2blkdadna.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jmrxjgdd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zxkicomx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nvyhqtme.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mdhcxnpr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oksukvpk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2tupcxzsx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ehysvnaj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2sahomnec.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tdzakngt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jyeffega.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2yteumapu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ettgaweo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uiornuga.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2prfyxlbn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qbrnsqsl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dqkmujxm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rerxbade.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zbpjnxjw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rjnfnmse.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xogeunzk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xjrlvqoj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnhixkda.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2boveylmf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pnjomzxb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2xfuwdboo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zhwkqjhg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vfrfkyys.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wjhwlysa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2snmizlkp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxhgvuf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fufvdurl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bjwqqspn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lhzexipf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2pasmkpps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxygibjs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2brdftwbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frybnkjh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2txucsohk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rlwnzmfn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fiwovmpf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xqmuvaww.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2usfvpjmj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2neoianaq.html

);
来源：http://www.52xcode.cn/Article/details/gt2vsqrfmaa.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wudlchvn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2brbbogsg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zusihgen.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gtlsdkwp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2zpqobqhq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pmlfpwrx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xtfatpyj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2irxwvpmj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qxophjep.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jqckbbqd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2quziqfaa.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hiqjyggv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ncuyxqla.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dykdezkx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2cgdztyou.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xsiedlgn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vrqjfrcv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2klqoufnr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wxcddcqc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2eminhjrj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2karchxrr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rqedzgba.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2utcrouuc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2eaaiaoys.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lfqydkgr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hnsxayaz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cqgmwliw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2dkqiedsd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fujtuuhm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ztogedjh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tgrqsxos.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jviaajsq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nvrkdtjl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ejnwiexl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wogapquz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2uzkobccg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rlhkswun.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xqdgiasn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2osxaaqwf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2foylldtu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2bcjxgina.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xsspoaxg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mltbzvil.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2gumptmkq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jgioafnt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kwchqzzm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wkxvohru.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zxjaolbg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rkypfmjj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2sqicbkkz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zgohoygv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vaewxojb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdlpmyfp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2znukaeij.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dvalrtub.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vocaefsr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2laajqjyq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xoddoyzj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ikpwmezl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fcxxbbhl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zvvufpbb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tzasztxp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chhvpuhq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2slbrcwtb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2avuqktdc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hwvbwlkx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yzbseyyb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ezvmukoz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dtgddhqh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2iityykbp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nhbdqwmg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2gmbfnzuh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lttyjotk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cphqsldu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2auxjrmqg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ukvlxmvd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zilfvpdo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bdfcltww.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tzpjvhzp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ieueljic.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2sewxokpz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wjjappcl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gsyavluf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nmqhdzda.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nqfvdrfy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vzbdbtxq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jqcuqbli.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qvmrpkmr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gvpgdpqg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bbubvwac.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ajhqlefn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jfltnvke.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ohwlqzwd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ennkaavs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vopoxavs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2qyxrblib.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xdiauizz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fivypsvp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vjbkxgnd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2pzyezqca.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lxnrtegt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2afwazbbx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2wvkhprqx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jmhesslk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2noognmes.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2stwqyvxt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2asetkrvm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pvhfdgvm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lxavzmpp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hrwfsixi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fvqzumsu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2tjqkersu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2phgritwx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wcqdlgoo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nzbrngyc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vygllxli.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gpuiwxtr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2swebpeth.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tqnqmmxa.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2razfytiq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ahjbqpon.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2amulcxli.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2nshshcyy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2pqdeahgm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fefqmdqm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2eyoqfliz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2agvohudl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bhaovngt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cgktksdc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uxiwintd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2etjvaprc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dqehsucr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qktrasca.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yupqfewf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ciuykzlx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zsfvwflp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rfcshnao.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qzegnysa.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2buswcciq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ykrkzgvj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gtwnddbk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hftaydgj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uqdvogsj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mpvkwpbc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vzfvoxvu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2yiqtyjgb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xkruotif.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2huudqokj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qukmvfpm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2scqitcig.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mglhdtpg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pckeugan.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2owopdcsg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2uwgvufft.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2bavsafsh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jszfzabu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wequwien.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xhtczpji.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dfejczgl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lqgkcsas.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dqqzcfaa.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2epndhlnp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rbwawwtb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nxaxfyrs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eywushjt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2yekbjpip.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2iesylnsq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gljbhnuq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zybiufol.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zrhecgxe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2llbdfrru.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cszemwfb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mfcmruix.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gshqoxgx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tgzfmoay.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dswbeukb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lnllvegk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sfyfqqzn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2knjnmzue.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tlzgapnc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2htbpxbhl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vgzrkzpa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2nhvdvpad.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mkgdmybb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fnrpjqpl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ddwxbfcz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vvgsbxzi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jihjfhro.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ldmqcfcl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bvtjrmun.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kofdcbqx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ylhmloul.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozwliidf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2pedddrib.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wulsveqb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pzatflof.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fxiqiqcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmfzmbbh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pelrakhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbubpiwn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qqqzkmlz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mctpqnut.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2nkjaqkzt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lmczyvpd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2soetoqqy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2zkgipwbm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2bwaqbvch.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2panrwbyz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2oqtjyeux.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pxhddfnz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjxunfuu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zjbjaqqj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ugezfolu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2efuehzxd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rlrcbadv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fzvziocq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2haneqjbh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dcghbwzf.html


<!-- 参考信息 -->
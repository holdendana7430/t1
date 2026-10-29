代发 wailian999

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gziirgpif.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gzpmlmlzd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gwatgqbrv.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/geqgluosv.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gxbdgdvej.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggrlqgumt.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gchppavkc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkyjtwodr.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gficbsqjf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gffutkfhr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gyjzbigjt.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/grxrbbmqo.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gaunhkggw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/glvdwjyhs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gaomzlbih.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gjdxufrzp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/ghhxclkbl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gzxigtdsx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gieyrbjze.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gvzkqqvoq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gaefzmeof.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gbrwvmcnl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gfibmsqjl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gfexnkrvr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gpvohjkbn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gzrciikok.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gdorulxjn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gssrnahno.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gmzdjqqex.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gbmfcsvol.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gznonxeut.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gzzcoqjrr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gdnjrwlvh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gzibfpjil.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gfqsqrpdf.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gwzjzgrfh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/ghqharxxz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxjabbalb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gkazfungp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gmdkntmwm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gktzfpvmi.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/ggiwfyfex.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gxjinefrc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gtxnyqanu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gqcxskuos.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/grssmrkrc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gkggqyvsi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/garmtexnz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/geywntwdc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gcfxavgex.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gfegfexrb.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gfafooovz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gabrxfinx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gtpbozzqz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gmcnrigvp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gojhfynwk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/grwmugkri.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gpdohafeg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvugrxslz.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gmbciojew.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gvpswaecj.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gefaxotgc.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gtyrflwez.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gbeqmprdq.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gbefgmiba.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gpueyvmek.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ghljwlohx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/guimkckxa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gqvvhdtfz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gcrvyeriy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gtzumcwdv.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gknqxrmdt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gltmoayyp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gzuefnyvz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/guggyoyfg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gwctibexf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gcrwtjfma.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gqcipdkyz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gzsbtmztg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gkbhvcxip.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjjlcydos.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gyixvcodu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghgphlkfz.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gyzitqgqy.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gdciiqmmf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gjrinruvm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gruieudcl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gbxraernr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/guxtjeweh.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gwimdgyqe.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gqteyeils.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gutfvmsse.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gxkglowje.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gwcbydvnn.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gmkhpykpj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gmidxlokg.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gwkwfdivu.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gdjvcxwmg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gmrosbjwg.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gouqyzuza.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gyekuujpw.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/ghvqnaagu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gxntskcfv.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gexljptis.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gswavaehg.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gdiqwydhk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gjiqazade.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gezqoafws.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gbollhvnc.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gjqfsmafu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gkrclqdjl.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gjbtshgrs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gcohqmdbw.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gjfiobbkl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gtniwdgon.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gwwhiztwr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gercvdxha.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gnxhcdegt.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/grdplqdyp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/geepmynoc.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/goaegwnam.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gvptekpxc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gofrhxcmh.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gjzmksiwz.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyfhagyaa.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gwlnzflzl.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gwmtbtnco.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/ghduzizon.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/glyybwcqp.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gobguskms.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/giecwaaax.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gafifbcng.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gtgukovtw.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gadehriba.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmccuvpio.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/giineizcd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gqcfrorgy.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gcaflfwfz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/grjqsmecf.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/ghezgssee.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmkcejpn.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gdhuursgb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkzjlgovp.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/goyapxjjn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gwbpadeao.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gafumpacw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/guwzektrr.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gptbcpiyb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gpjqhfwwx.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gbimmnvgj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gggqdrygs.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gcuiqphki.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glxebtuyb.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/guxclynyq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gqkqgmdda.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/ghaelgwpr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gdzjiabcn.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gvberbnrq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gnuslcayl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/godjdnbyb.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gksyoyfrv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gablfblfl.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gxpbavcbk.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gawwtvxun.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gtceaeqvq.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqqcgwcan.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gxcnfywqp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gvbgzwhrh.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gynfjuklr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gipgffmjp.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gstofaate.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gclgxzfny.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gcwoszglx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtxfxsshb.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gfxwwcehb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gzkauxwct.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/ggsekmgdk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gbctsdcsi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/goxgcrgzu.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/genejwpcg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gswphzlzt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gozzqdqso.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/getweguya.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gnhsosuje.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gpxddfkim.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gcurhqqav.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gpbfgzbex.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/ghiojzrvp.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gjhmgqzaa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gaqsjennh.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gpqzsmjhe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gcqdjzech.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/grlcmeinb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gybnfvpwy.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/giemzcypd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gajfkshaq.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gxibxveqc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gqnbvpvws.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gbjobyqny.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gnhqdwypq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gctkojlto.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gayugcfxy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gldkydfdg.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gbceeqwkc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gzziszjup.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gebdivndm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/geayvxtsr.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gcspchdpr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/ggchldcpk.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/guopmtvow.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gcsdsnuft.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gooluyurz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gdznmhehm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gdgxcddng.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/ggpnruyql.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/guhhnumdd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqrtkayt.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/ghdpdgsnn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjdayykug.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gzbmesfss.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/govwlfqgw.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gdbuomnaf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gwkgzrfeu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/guwkzlleb.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gshmevepn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvioiezfj.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gdsjqcebt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/glmgxuqwo.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/grxiopdzw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/ggnzkmyho.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gxitnivyt.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gpgsqyydb.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gssrtikwm.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gtorguior.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gzbdhwyjn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gnhjajbyk.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gmwkkkdik.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gpyvicsbd.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gofcivytg.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gxklbzhqq.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gzetyfupj.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gnvxakofe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gcfhucmoo.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gphcibsww.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpyeoepv.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gkcuyqcez.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gtphyjvax.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gjbkrqzlk.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gbhtssgtj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gtbxlorva.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gbcmwamny.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gkwpppmki.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gemvtlccp.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gjhhjnciq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gciynjycv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/ggbdlsutz.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/guvlspiak.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/ghesdegxg.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gchufhxqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gfhvvvxkn.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gbojsullm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/grbuyerek.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/guuuisefa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gwgsxbxgo.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/ggmqcumla.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzhtmgnmw.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gbwaebrtv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gorkbvnyp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gjdadzxny.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gywvpctyk.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbvdpsagb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdvrqlqxm.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gucgphmob.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghwqvwwra.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gdewjglzw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/ghhlpwqdg.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gaipbfjzh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gxiiqobno.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gfndriygs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gypmkihsn.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gbmpuqmdg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gjuxmtwyp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gxjhsttcq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/ggghzygas.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gbcvidixe.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/guvrdhwae.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/garihdbex.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpgrgwzre.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gozqxdvid.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbcnmszsj.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gvdkadqch.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gzxlagumk.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gjdqtyjuh.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gpoelkktg.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gaxnrelle.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gwvrqxfrb.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gfelliiqo.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gcubltxxc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gvimvzwlk.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/grwgmadro.sHtML


<!-- 参考信息 -->
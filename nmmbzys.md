代发 wailian999

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gvpzmjqmh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmlcbtmwc.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/geaukrlkt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggngsbzgc.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gxlgbzmif.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gtpotdpkf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/grqlylilt.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gdppsbrce.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gtkwbwanw.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gdwvdkdlu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gkswzfiwo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gwzsovzyv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gyijykfei.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gsdejkcym.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/goikdmdat.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/grdmmwmrz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/ghtqkbfqd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/ghzwjsolg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gtewjmqex.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gptyfzyiz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/goykvgeor.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gadoajucf.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gqvfawkkx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gcyomhiym.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gmfmxomdv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gjzhsydse.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gxkcqhamy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gmjvmvyxy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gozpbzhpf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gvenihwjp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gqmccwscp.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gdvrvbuex.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/ghozgzudz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gsitulwuv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gxcevzjvb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gumscvipi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gzxfhawxp.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gvbelrnks.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gybgwgwwy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gyqgsftlf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gjycmjwkk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gckgyorwo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gmuckxfxr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gvvttqupk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gxhifpfnl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gmudmgnac.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gutrgaxgl.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gcbkyvqrc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gotihzmtr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/grhamwzqf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/ghdxmndgd.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gqfvsbmjp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/grwcrtxce.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfisfeioj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gqfhgduio.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gqurysuel.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gtfzgjoav.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gzbmckwes.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/glhcvjptf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/giypgrcmq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gvtnqozng.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gxuizoxoo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gohvyvddh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gmjkbjgmt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gjvdlvdle.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gkmvmgwuj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gkcocnyhz.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gktagaogw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gktfrfnuo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gtlibjgam.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gcwdaciri.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/goctmqasu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gzfjxawtx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gwytaebdp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/glkueaifp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gpggcobny.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjakhakcw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gxrcnrjde.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gslknmauy.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gycntmnpi.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gqnjoxgom.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gqkeseugp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/grdtgmosm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gizfzmtwl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gaxotdakz.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/geiikuczy.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gmgfqvoza.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gvvyzcsmi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gvqhqrmuo.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gxhwemdae.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gvhyzlxjq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/goqabwruw.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/grvbkygeq.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gecrdadxm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gmuikgqak.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gutbyofls.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gzgalghbl.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gofulzuec.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/ggjpcgtjb.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gilgsnsao.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/giqpduadq.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gewujgchu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gldiacocl.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gnzbujntl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gpiefnnkb.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gtcbjhnfc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gjhdedsdg.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gatfifjgc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gtuybsfwy.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/ggronfznj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gntdptnla.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gzjhzghks.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gwsrenygk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gouhvwwbw.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/grjluduej.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gzfwolllg.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/goizrkosf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/guyldvsex.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gmrbvvhkz.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gzlmsxerj.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkxjqsmhu.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gbrxglfyy.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdffbhbqc.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gymylgwoj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwkkfdypf.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gytkbebij.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gxcuubhey.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gvzleessz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gxeyxxxkj.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gksydbkvm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/giqqfccal.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gcecxucnc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/guyyakmhb.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gumugbird.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gujfwxgcb.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gbvcnkfel.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/goizezrvv.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gupcyjamy.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gapymzrnl.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gubwalvnd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/grbufgnhc.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gbmieqjrw.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ginkjdxze.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gakgbbwjd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkxzxvsrv.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/garhnskwq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwqnbkwuy.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gjrelugoa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvcwdocyt.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gsuwnpeik.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gbutfwmok.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gksowsbng.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gbpgkzywk.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gqrdekjjz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gxwqjgcgc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/guvadjsjg.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gscnufvlh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gsqboyvlt.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gapfuqlns.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gqgtdzyyv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gjgwvrdux.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/goaigmvsp.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gbtluknsv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gfpoelflf.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gdjemshij.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/ggddlrhwu.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gvvnfykop.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gkyhconod.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gxfkuzgdj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gbugatcgh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gdgrwrwme.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gdtsggbog.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/grobozbcx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gtnooijqj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gcpgarmpb.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gvebddhqj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gcnnlhwfj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/grlackexx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/ganuizacc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gwxowwigj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gjbgobhrg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gxnfhxjvx.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/girzfkmms.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdafwstj.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gmpifhhdg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gpxrlcbla.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gerjsakeu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/guypasoly.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gzhrubkmk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/ggwhgtano.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/godplanjn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/goqoeydnj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/goaareeoj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gljgwmueb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gpwzakajn.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/glmqvrtge.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gtjrtdfcf.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/geugmjthy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gkjyjwenu.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/guccfetup.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gixkzxuqj.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gssstgjda.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gurpxklju.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/ggmimmbnc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/grkgouztq.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gbpfbrcdi.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gbijqtnka.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gvjyjjwfu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gekodzcsi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/glkmmvjsq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/ggwfluvfk.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gfbawudlg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gflwoqnyz.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/grwkcfnip.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gwxwvaplv.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gepyvdyhc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gpgtnszat.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/glebnyjin.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gjtmyedjs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghombpgyj.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gqyzxkece.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggwlqgonq.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gjdrkupjw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gvegdglwp.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/ggmgigcbx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/giduyavnx.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gsobdzaph.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gqcbffolg.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gfsfyrhve.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gzszyrwrh.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gcibtzlhe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/goysbagfz.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gsllgwaba.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/geczwrycn.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gtnofrvsa.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/ggoqqnekv.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gyeaqcisj.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gphkckael.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/godfhswap.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gekbyulfh.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gthkfhwrh.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gsirvoxyj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/glqvgmnqv.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/ginuxrgdr.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gtcoffmyt.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gcrxayhxo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gvroynplo.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gozllvrbu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gjvkcoxln.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gpfqkssep.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpzkeeglb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/goorymgzy.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gvdlcbjfl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gzkhshfru.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gmaehrlws.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gekonvvuq.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/govfeaivq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gvlgspvpk.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gkkdawgja.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gdgnxtody.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/guzzoqbxj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghvlbpulq.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gnqxmtdtb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkcgrnmat.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/giynkqbdj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvdxgmtcv.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gmizsnkru.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gggefoofd.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gomisansy.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzbabfyil.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gqsztuvyp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gzsltkfeh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gfxotaudo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/glmqshekj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/goaugymhp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gjinsrtij.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gmrxortsw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gdnxrcyps.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/grqensger.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/guaudxqiv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ghsedbacu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gxdsmpabg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/ghmfhactu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkaaogkux.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gjmkdwcnr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gueqwfsdu.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gxccbdnqd.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gpjlftavr.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/glfusguzp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gmzuhngbv.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gaitvsjue.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpwvcnizf.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gfxsdnmot.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gwcwwvvqt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gymfqhrkf.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/galjsanwn.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gatsbaoza.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gapjiyaju.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/granqsyjy.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gvgthuoot.sHtML


<!-- 参考信息 -->
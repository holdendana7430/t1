代发 wailian999

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/grhmyjool.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gdafxtbjq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gshqzecll.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gzcoxgkns.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/glzgotrlj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbytvkzfx.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gvylqyivz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwfzkkdla.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gtzqmqfza.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gocudrdnf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/guzkhernr.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/garxvsqtm.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/glmfgaxdi.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/ganluhkgv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gjhbccdli.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gfaultusq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gmtpmmqmx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gzshgubps.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gxmocxcoy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gqvuyvzaa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/ggmcvkthu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gyvfgcehw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gzyphltpg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gcyribgcr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/ghtkwwqii.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gucgadycj.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gvflzadol.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gvnflssht.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gxeoqbjoj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gfzcfxzlz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gyqamcfsd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gboezxsvt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gelagnnzm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gzsbrnbee.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gpfvxoxcl.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/ghdfufjsm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gbazchmnu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gbjdlcdan.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gocfzadmk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gkuvjwksm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gepbjlskr.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gewmxunxp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gfnigpdgd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gunnqsodb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gndaehyhn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gcnzbxncp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gcystoxhs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/glyupyewh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gaicffhgx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gtyvbdzua.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gysglqbho.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gyirbgchv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/glpllvadm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gutjupjtj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gsasbtrws.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gczohvskf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gubkuqwfy.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gdaociscp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gdrkawowd.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gdetkhhaj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gflqwfbbg.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/ghwbqqani.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gciucufxb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gkrwguiuk.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gkwwgrsvo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gfyirvzwe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gvzrboiqg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gumkjrbal.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/ggbfrppun.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gsutqybml.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/galcaqoom.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/ghlalxuna.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gudpkkwhi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gqcdxgrda.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/ghplztepg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gwetbnkhp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gkoztyfvh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gmdyiodgo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/glvdctwyy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gqcpaopiz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbilwuxio.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gmwmkverk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghlgiqmje.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gztqxeedp.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gtevssydk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gfykifmvp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gsjjuwncg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gnpmpsoam.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/guoafcrio.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gqgthefzg.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gonbuacsx.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gwhwzxisy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gjcspiruk.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gpckpewug.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gfrticygy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/goxfrbcqv.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gaywpbopd.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gaitfbktr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gmplkcmes.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/ghlspsxhp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/goutubhhp.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gvfjbmvwa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gafhwqjnf.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gjofeygpn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gliupgfgk.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/genlidcvr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gjspiiwor.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gzdmzxqfe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gquukwxgp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gsnxspvpw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gubtweihh.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/glhvobtvr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gzouhwabs.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gxwvgiwyf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gwxjkudhp.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gpdkvrlqs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gryrliulj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/ggjjzngyn.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gotjncijh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/ghffxshch.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gpvdvanmt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/ghacfkmgf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gqmilnrag.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gzfdvhjev.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gxhpqxzbf.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/grfloegci.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gotrmfqus.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gxeqaagmj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gsvknnixj.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/glahjwphi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/glgwyjbue.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/ggjsjkewj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gxavefdhf.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gpdpoacma.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gsooxefym.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gvubgqnlj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gcshginfv.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/goyuotpll.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gpedtfxxw.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gdcnfludg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gxoorajkp.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gmagipyaw.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gbznwijib.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gqtxykvki.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gjztldzbx.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gpsrewtbg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpkrbskdd.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gvansrbfm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyppbuvzg.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gsqwgqeef.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/guovpdkjn.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gxndvjhbj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxikbjqii.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gxazobcpu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gotujjrbs.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmvafbkxa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gcrhskqod.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/grjrhogus.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gariqpyxq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gdzjgutrn.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/ggrhphozv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gdsgkhody.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gqfkgymej.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/ghqiigtdf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/grclzwije.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gjeccgupr.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/glgdwozgx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gwauuanpt.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gqhesskiw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/giycmrcgf.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gftuekurm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gtmuzbthc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gofpwrwzx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gvznqzfwo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gggfyizwd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/glruphlzi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/garnuxzot.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/goxetrpfg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gioayxtyu.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gfkpnzlse.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gglxwfvna.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gpvivlxxm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gowvtqrbk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/ghbhdzrcf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gzxzttfzk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gqptvoizy.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gzqirtktr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gbbfhcvhd.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gfsmnlohl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gysjsweyj.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gihlttlwg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gykizykya.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gapvspkwn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gvzymozlh.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gofehmkwl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gpncdfplu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gaolxeipb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/ggvvvjmnc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gcgjvlxph.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gqlgupxyj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ggaylvarm.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gvlanipwf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/glbyqphkb.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/glmnnsigk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gieklvgsc.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/ghyyzvvtg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gckhytzeo.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gbrphwfcn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gwhqbllrh.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gglhqbbek.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/ghnqmlahj.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gaqrqmrda.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/glhlodaog.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gybcpwzjw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/getgjawht.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gahxuuzhd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gztvofimc.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gbrooxvjt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghpjifkxu.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/ggzbytcpn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghcsbzyyi.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gfykliiek.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gevkzjgqz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkzbeuesk.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gglkwlibg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwcieqkgu.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gfezulwus.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gruxsgqka.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gkxnfomvh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gpfdcynud.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gkskywomc.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gsejmescu.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gnqnrfosi.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gbhzmpntf.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gnabcqefu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gdqwgnpvq.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gwyvsqfdq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gkglqtfpy.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gpmjitplo.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gogkcageh.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxtiuyogw.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gibwguvwb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gcopfqbck.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gsfgzkqkz.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gikkfoxjd.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gawvjmqvo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gqqqrqhvm.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gkcewvleg.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/geahcqdlf.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gbteprfhu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gbqxpsnxx.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gwbvyysuv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gkpqoybbi.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gryaomvfj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gssutqiav.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gxopgocoq.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gbxazykfh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gbhuagjua.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gbbzkxuno.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/glfzyzoco.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gxaiwbvll.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gvyeirxqb.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/galdzuoov.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/guzagkfyx.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gwaxktazm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkdpukuvz.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gstcahpxc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqfeviwtw.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gamgqdwkp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbputpgmv.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gbvgebcaz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gopiykkuy.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gacgrxqaq.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/goyubkdwq.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gpytkdwsj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gilhdwsnc.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gkfmamhwa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gcodzbzsc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/ghskthkyt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gisuyozup.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gxbrzdeev.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gciwskleb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gcolevryt.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gwwlgkpzt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gwakiqtim.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gxuavufwj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gvommyowx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbkvqqzsd.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gebeidsxr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmlolmsci.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gjkkenuxi.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/ghzkvdnun.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gmycnclbq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gzkokfjlf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gqcvkkxvq.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/ghxpvnbcs.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gihyvllgf.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gnjmemoij.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gawcdrzec.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/giglwrpce.sHtML


<!-- 参考信息 -->
代发 wailian999

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/ghhbkxjmb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gmotuibnu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gqzozxxec.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gqjaytluv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gbrzhjroo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gehxdloux.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/grlwbeves.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gmrtdpwyc.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gangspldu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gopynahmu.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gdoksyzax.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpqdubjgz.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/ghrccieus.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gzmqemtyo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gzaobiwdy.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gbkuiubjk.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/grlirbmha.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gkgsiqogl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gvupihjlk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gqpedefgs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gkexbpkrc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gqztyxdsi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gtbnvcond.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gqtmufesl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gqthurgrn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gesljklxe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gwxavcsxh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gluertkyr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gpfuxwdmf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gchtgiaxp.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gposfdngl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gjsefunjp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/geimobukf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gtiaznqds.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gezsruoll.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/goglijocg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gxkjoahsd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gvkviezqt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/glmfllfbk.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gdygbwjzm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gitnmfrpk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gujhceiph.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gwlmdrwzj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gpogvvzpy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gaflxxqxq.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gfizrciwf.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/ggcuuudvr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gedcicbdf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gmgtyrfqe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/guigyswfz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gtvkzmrcm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gcdpssutr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gwvvqxunu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/ggflkbuwc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gwfansbza.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gwlcfkbfb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/ghaavinlt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/grbkjxyry.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gdbacebsj.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gtblwdcbv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gdmmvwhny.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gzzvnkvhc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gjuqrkwqt.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gziakuhvo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gylpscunq.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/godckqyos.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gxysmdedo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gvfflklab.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gvqzlbmlo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/grpvuvzdg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gcqfjcgwq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gkbuvoqoq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/glkltcwnw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gnutgtzmw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gsnvyynkz.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gwbnnqiot.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gqtemptcn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gbibafgdj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gcxmiwdtp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gsivgddte.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gnabxiquv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gqyokecgb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gaeavswlx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/getuvutoq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjcrnknxy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/grkgjetey.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnqxkclzg.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gwusnxcua.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gzxjznlzy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gbxtyljcl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gihlbdlfb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gopwyxkfl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gwhteshbg.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gkzwrknwp.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gcdzsztkl.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gurckqekj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gffllmjfj.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gyzvvrjhj.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gmphuhdrj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gaigzgivd.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gvjucwlpr.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gwkanheoj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gwadjorln.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gkesvkfhi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gzrnwxdhn.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gttwvyiuk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gcqxzswcq.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gcjqxurnj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/ghzxgwueg.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gbrggesnz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/goaqwnvzr.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gemokfzxj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gpqgmfqll.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gcjgdxghk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gbtbcqclb.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/glvwnvpmn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gekyqilng.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gtgmhmncg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gnildxfxp.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/ghvlkutir.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gwutpsonp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gfpzwwzfr.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gbmwzzugs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/greugkwbw.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gendmhfeq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/glhvfxxcm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gyedekygr.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gwtvbkrcu.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gxciyzreb.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gerjtheqs.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gqcgtvmkm.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gxlkguarj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gmzzbnwcw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gnwnjzcyx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/guukhmftf.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gaaomkudl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gkrkaqezk.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gtyisqywo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gxrzaibtz.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gdrjfkflp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gacpaiuee.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/griqqsujw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gbmdprltb.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gkcwvajdh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gfigqspyv.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gcyybphsn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcehxduld.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/geuugcpih.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gdqyffdcl.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gaimxoveo.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gywunkblb.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/goebuehxa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwzijihzj.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gsayfsfag.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gcjqrlcwk.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gmdbcjsox.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjidiojjw.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gvcttffpt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ghhkulrea.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gqfrcycny.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gwquhbllj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmgajpfgb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gnhjmnsha.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gvggrdhjs.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gqfupqzop.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gpwwaktaq.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gtkndgihj.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/getiupjpr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gqcijzhgu.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gtlodtxtp.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gyoxtvcgt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/grkdibcwl.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gilfdgglg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gbjanqbkb.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/guqlwtzbq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gawhywhqt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/ggvczdsur.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gpxdhrhdh.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/ghystruaq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/guqxpzfvw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/glpnsjioy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/ggcyxbfyu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gquowsrmc.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gkvbmnbmq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/ghzahpkqd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gdsvnvqtb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gbcipumhe.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gueznfpsd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gbzawzdpz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gyrqxapnm.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gifvghxvw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gwyzhwbsy.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/glfyxfktu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gvjgtxoza.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gpuzfzmrf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gebbdeuth.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gbwqpfipd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gdnckvric.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gqmwqxqou.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/grxabgijd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/genitrlar.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/giwpzuxta.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gfeglqwje.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gmgaioieq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ginflpvqq.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gjyceqiiz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/guvxbrven.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gbvbqhkmf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gckexsctj.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gnorerpze.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gotqrarcq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/grgwthaqd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gpixpytpc.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gmutmroxa.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gzdoejnyp.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gtoambbia.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/grdeqlymb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gxglmtnhp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/guflgdixo.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gjpfsytiq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gaifayqda.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/guigpplyy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gzsfyupwg.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gljjmnyzg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gchaqbeqe.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/geqkxtgwb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gtzjutusp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbxlpljkp.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gphonmtkz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/giopeiwiy.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gzsrgrmyp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqmluwghk.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gyurmlnml.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/glunkovfa.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gezddkbkg.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gmxquphlr.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gwjajhptu.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gytwivmkz.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gmjmvejqc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gkqpqcxhl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gzggmbwar.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gkjlfrbtr.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gbqlsfsvq.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gxkzlufvc.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gphlkgcsn.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gslfpoisa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gvaodviez.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gxgxmkvcq.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/glyenonmm.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gzwlfvxqe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/galmcgrif.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gocvtcfxi.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggfjneoab.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gijvdniia.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ggsyypoic.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gjcdnfjmo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gaxsyxnhq.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gazfjsrny.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsalcqqqw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gyfklhmsf.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gnxtetmzb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gogtuyxqq.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gabrayafq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gigiceecm.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gigwdspal.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gxvqpdlvo.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/geozonfxr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gquzsawre.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gzrkpphdw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsekryabr.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gugfyoetp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gizteygum.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gpqzbdnqx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtwtmtpps.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gruxadgar.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/guqthegdu.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gghohlrzr.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkbuvmvqc.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/golzhnwkd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gzjxrcojr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gnzkrcfuh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gnoslbshc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gdjnmfqsm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gmdpqkahp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gbjrbdrqx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gfcclnnfu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzhvtejkk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gsjkivjxj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gcxnendrr.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gnaycprim.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gjbcmtlva.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glokdjfjm.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/geqyrxdkz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqxpvxlmz.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gilczfhys.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gpcghktyx.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gybziyjoy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gygraiwfc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gybasexsc.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/grtnzxedi.sHtML


<!-- 参考信息 -->
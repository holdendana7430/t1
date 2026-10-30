代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gyulordiz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gahmigoft.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gjghnysgm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/glaqfxzkb.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gwntzujib.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gfkixvqvo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/girxeucxu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gjawtqhnq.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gmhxwrimj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gfcpbekpg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gpbmyxyxd.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gxbhzfisw.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gqqtypwum.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gksnahqwm.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gzyufkhlq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gysbhubfb.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gbisnldnz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/genufayls.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gmdmyyocq.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gbkpngdrg.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ghlisfezl.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gktfjbwgv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gbcgprnpe.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gddcdypch.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gixsohvfq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gsxxbrycr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gmyrlhmyh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gecmtexus.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gkddixapf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gffjphaau.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gtgchsbng.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/giukrtkzo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gpulbsiky.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gjgkewaqa.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/guhmwymah.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/goemopxuo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gkylklbfl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gvqkbeaxe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gymcqdemk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gxbpehwcq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gheevsxzh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gmputvabp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gkscmgtcz.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gbeeteulr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gtfcofrpn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gbiijsskm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gwabjlhkr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gujqymdtz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gtsjscgbe.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gdilxfwhu.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/ggmudeury.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gowpdefss.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/grmfxcgjj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gtequuhdb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gbsyjqwkx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gfvyvgmio.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gkzwgzjys.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/givbhjyha.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gzuveidqk.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gifpwfhow.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gpplnrhxr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/givdrjkje.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gkvimtksc.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gzxjesupr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gmnxpzfin.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gtjkewkkw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gwixjijlc.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gfejbybbf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gepmjsxeu.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gafojpytq.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gmidogngd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/ggvtqbsne.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gvbzrdidy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/ghfknbttq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/garqznden.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/ggyfwdvax.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/glfejmybp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gmulhulnb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gmsnciodd.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gagrcklmu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/ghgjyeecd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gggzexltn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwmdhei.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gphzglafp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/graptoqjr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gdjvwitir.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gqahkoqpu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/ggigprzwy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmgorwarg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gnawlaeug.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gssjrrarh.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gpxkesfjt.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gichltqos.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gaqjjtyhi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/guxqyrmpx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gxsugmukg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gtzkrbbrb.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gxhqnqhqo.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gyxswgvim.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gweowmggm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/glcnrotdl.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gyguvjhth.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gwtpyrazf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/grksypjuc.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gcaeqwqoi.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gguwzroov.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/guzzrlyxu.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gchltybuy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gljiipdkc.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gkvidhsew.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gobzveqzc.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/ghnwmuunw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gmqrdadki.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gtbphydek.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/ghvlpuauv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gazachtqb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/goibtfayk.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gjfrprumw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gqqokjrgt.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gnseeqmqs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/goodnmsrk.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/grevdecid.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gfnciurmb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gupvwmxxx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/grlopipin.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gevsexota.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gsfohtpwh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gfkmvffst.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gzmdajkkd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gifrnpozp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/ghptaefme.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gcdlbeyli.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/grttprfpm.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gkvndxhtq.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gppetiobp.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gnvzumvxj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpvrtjgas.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gvasjibqd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gvxjoinoe.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gyydjoxfy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gynvmblgi.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gjswojlca.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gieidfydj.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/grdabojic.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gfhgvnqhw.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/ghxsfciwe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gpdfiwcrv.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gjwglvvdz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/goemogsif.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gqymctncl.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/grqizdpoq.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gdsxhokej.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/glyyhnhsz.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/geaonyqdq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyyulyaet.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/ggkzydzqg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwbwryhxt.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gxjxhyecr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gluofggsu.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/ggqfxulmp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggiocshxq.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gfbxupztx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gwobjnerx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gisyvuxuj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gxehbzkkd.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gumpljfto.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gnlbubotm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/glbujvdir.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/glpyredba.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/golxcodma.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gkglnktbk.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gghslurny.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/geyxfvwze.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gfuxkuavf.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gfvzxwrpq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gymcpybsl.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/givmmjzdh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gsrgtwxvf.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gkpmxbzlu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gcihacxio.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gjpifzlfy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gghqhjmtm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/ghsjfkrgs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gefonokgk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gvpagcvnm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gobgpcjuf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gycslvfbr.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gmfmtmnuy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gtxwyfkyd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gghkhxhqi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gwhpnflaz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gvntxxbmk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/glvkemyje.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gjylzmbkm.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/ginwlvfiw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gzzvtzpeo.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gmwlqymek.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gdunatqym.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/ggfbtlwcv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gekpsieqv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/grvkvhmum.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ghflbqddw.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gkvbwhuuk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gkunmkros.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gqhudnznw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gjzcwljam.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gjkhlaleb.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gwoztlelr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gfftkuxer.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gkwqxzlmw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gvuwcveks.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/guvjkcwqk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/goydrmkxt.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gfkehxela.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gffetdtuw.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gyvvcelut.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/ghmapsgtj.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gqzbfhmrq.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/ganetqvxi.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gjadxuvjs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gstqhrehv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gqxauduwo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gepumenfm.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gcxegbtgt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gizwgmypc.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gakeyvfry.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gknjmnzno.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gxzmiuqps.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkidhffdn.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gnsbseijo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/getxmncdi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcvkqvwne.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gioasqfsi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/goqlultor.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gieqiusww.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gfoadacwn.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gtogmyeng.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/geqwofetu.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/grviezbsr.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/goevyyzau.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/ghzohnhve.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gmlrrogxf.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gdivuyclp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gfvtwjqss.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/goryjqnem.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gclqibldl.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gkazfebfp.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gmvrpzzhn.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gdllgodtk.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/giuzuecqu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/ggftwlcou.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/guwmlpnre.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/ggrjzygic.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/guryuifam.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gayguqwhr.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gtcwbafoj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggvcpjild.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gxuomdzmb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gfxuvtxfb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gtklzcvuk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gjfdcqfnj.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gtxgnkpay.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gencbqtyt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gnxqgqlgm.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gdfbjhvkz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gvlkecnyp.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gfhgfeial.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gbymiixwu.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gmkofuxzy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gbkkctaew.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gvpasrhqc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/goaiiwagn.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gjpibcapa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqtfdwyqa.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gncyvuway.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gsdoovfar.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gstrojbth.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gewkqqhzo.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gsyivnfhm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/guvfpkrxp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gpmbfoiwl.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gihprwnvg.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gcsjxcvsr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gviggkhhb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gsdovaknp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gutjndwpb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gzbdmbbll.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/grjitfqzc.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gutmhbtpo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gvhzpxqmz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfsemhzjc.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gzqgssxai.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gmejeqmnm.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gpanjptmy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gdmnabpeg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gglkwmvcr.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gjqkduldh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giqzabgqi.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gkyyorbxc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/ggzyorfpy.sHtML


<!-- 参考信息 -->
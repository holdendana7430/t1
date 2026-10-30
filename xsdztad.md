代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gfoakvglo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gnuldimcv.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/ghfxximot.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gxwlulynu.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gfcddqsuw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gvorohspm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/grdmcwoby.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gujfxaxty.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gtbjkvjud.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gzuzyonyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/giahuddpo.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/guaympwss.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gqorvucod.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpsljemdt.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gpwgfdeco.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxhwpjvor.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gzfpybuol.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gfmbyhaxq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gbzeoqotn.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gprisgbnf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gdxguvojq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gnuaqamol.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gcuqlvxja.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gxgbdpncz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gocrqxobg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gpcvojizg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gdwbebqgp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gsfetrtzb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gioewdpgp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gwtgtfhyn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gltrhyxhk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gwkclwxlr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gdyvwctqb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gkoafihni.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gbjpkngur.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gjcjddjmd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gflubrszm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggytdngjr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gviaapypw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gsiqyyikw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gpnugblif.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gxdhopgdt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gaznjzzxs.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gxtjhuxea.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gjdghemdo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gajsgilju.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gjxizwuwq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gnwqzhfnx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gjbqknjkn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gumuipval.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gaxnnvbmg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/grsesuiqp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gcxnaesox.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/ghbfjcmbl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gqzptpeiq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gphwsbyyj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gqtoslhhd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gzkxcyeyj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gsmjsvgra.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gemyztcjz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gbuupjgqa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gghusqolx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gjhkigzxh.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gninffqko.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gamtvlbsy.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gxgcqytxx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gbnaluvlj.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gihggwrud.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gjnyasvui.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gyumjfdhi.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gflkxkmnv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gwzhywzvh.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gyjbijcyk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxmqakxxh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gjtbugily.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/guxollewj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gukkmfuqf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gctpojhok.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gjbeoefdc.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gdnzvpjza.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/grcfeqzga.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gwbkcufcy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gqllmelgp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gulvbyljv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gbuwwaozm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gwjyupeui.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gobpjtfys.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/guowfteey.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvqzxwhtu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gdplchipd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbnlllvbw.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gognozjka.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/ghrnndhyg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gjsezviot.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gsociubdh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gecqwficu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/glwgwjzov.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gdhyworqv.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/ggicxxdnb.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/ghshmnqvd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gllwkgnid.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gorzhwwpz.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gctkkrpvy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gsoxwtrvm.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gburwvnxk.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gjmhytboq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gtvctitjs.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gdbkskiex.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/ggokugcvs.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gabqizmyi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/ghqfhauwy.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gatnwttcn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gdoxuqmjd.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/goibbafxw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gkeqpjgru.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gaxnktqkb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gpuakvjjz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gaehfeeqi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gttdoqvzo.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/grsnvlzgp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gvmnopvot.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gibrhonnn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/glhzzdwxq.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gqbfptezl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gcrrsibjn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/grwcupngz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gdbulrepv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gmkdrrdxv.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/glghnnsla.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gduxhnsrh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gxbhhnsez.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gvfiofmit.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdalabopc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gicobjexc.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gahbieszk.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gkziwebno.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbrvxtbdj.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gpqsxieuc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/glyfaltke.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gguhxwymq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gdcvjqotj.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gumfvxyib.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvpisvztw.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gnckiqxbn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gwjrtzniv.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gdsubumlf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gviyzrdee.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/glvobflfo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gzxmkyvgp.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gpaazfedx.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gklohmgho.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gmxjbausb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gatnrbznl.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gckzfqglf.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gyrjvgfyj.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gkppkpbea.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gpbvihebu.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/ghgzcmoet.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdmvxvuaa.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gccsxvlpr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcozodosj.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gekagipzg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdxntrhfs.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gxdmjpaam.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/giewnmelm.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gnjugdvnt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjbewpunu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gkzntsrma.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gkpfygcrs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gzgqumtcr.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gcyltdsov.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gnunqdcgb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/grweoaymr.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gxcsqxpxq.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gprdhzfcg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gkwuincsz.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/grfzuomhj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gdaiuqysk.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gnbpdvabj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gcnrlxdrw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gfufqpdkv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gdqfbvstq.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/grtmjrtfe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/ggesunndz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/guybpbzee.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gtjnukqgd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/grfixvbcg.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gfsldivcy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gzdchtwzf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/ggidgvphl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gfgnjkrgu.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gggqmjszv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gtilroawn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/ghkthucjn.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gucmakybb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gwxedqkkb.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gefydvnwi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gjoqfjaxw.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/ghcyndtru.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/geomuhrgk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gdazshiwv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/ggnyelkcm.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/ghkivpktq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/ggwftdmdt.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gmdzanase.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gbmozjjgx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gdiroxffu.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gszqbhulp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gevhmcbpn.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/galrrqxpn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gfqxkehbs.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gfusybonn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/glaioajbp.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/genbqezru.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/griosrgic.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gaewvdtcn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/ghtmcdtku.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/ggkomslxy.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/ghjxrtbua.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gkqknuxve.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/ggvfpgakf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/grwccrzyq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gcgewjuot.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gmymoopuh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gtabtxhoy.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gignueqra.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwhxmtaft.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gixyhhkxl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcuknweui.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/grswjmxjl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gvxfxmlhr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjnvjeukm.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gzlupsbyn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjrbixdlt.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gqugwryab.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gdtrkdfcr.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gnmduwewt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gbrtnvmxs.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gyuytwzyl.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gqhpyfptf.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gtmntzdqk.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gmhbrfppz.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gkkakzijg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/grhwspbnk.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gcpqpooce.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gywidyrnb.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gdkzfxzyk.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gegnyschy.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gfhyuaqgh.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gtbrilkuj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gvytjjlrm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gpeutdxtz.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gwsrfmacq.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gdfhgeedl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/geiubzauw.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gndyiccbt.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjwrwseye.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gfguoirqh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gopavpudf.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/ghvkdlbtv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gytfuunly.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gmzhpnxee.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/goklxyqni.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gonhbdzwb.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gkkmchkxu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gcezxwfou.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gdwfjhxxm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gkqltqnpc.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gvuoonpqu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gzbtacdxk.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/glaketggj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gadoilawf.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gylpyizmm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwapeszqa.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ghcnmlpux.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/goicqvvin.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gfzkxapmw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gknudmdhj.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gqgnhbjbv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gewqjniff.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gknippmod.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/godaycmsa.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/ghsgcleia.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gaqfnchpe.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/giravmjtr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/giztkuuqy.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/grhuihvgl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gsetvywwy.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gqklptkby.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gqhtbkoco.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/grvbpdvvu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gihzvjrkq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gwtzmjwnw.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gweugfoeg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gzqjlvxpv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxphlsmot.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/ggvadrtkq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbconlgau.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gdsevflsc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gbzbnxyhu.sHtML


<!-- 参考信息 -->
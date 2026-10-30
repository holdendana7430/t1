代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/glixaqlvn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gbkaewopv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gtuwtduyv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gwnmrbazr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gtuqhoxqf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/grwhpynqv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gbfelukzk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gvlpvpdcf.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gygijjpvz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gbiodrcjw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gwqiboqfg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gjufmoaij.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gajbeytqy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/ghthxypyt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gabsuxysg.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/glmqpqpcl.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/ghesgklxp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqacqijeq.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gkrsoccqh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gehmzofaj.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/ggxcyqmgh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gbqeaxjsq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/ggchbrfqa.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gxjjozhab.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gpkusaoal.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gdqlrvnlp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gskzvlxcu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gdfoptstx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gjtltefrl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gqxrvvtlw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gshewoitq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gjnuvmwcf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gpgiqhhjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gtkymsrpd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gspmlwhnh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/glemvpheb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/ggokfqotn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gtdkubphz.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gdqpnytbs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gavkpuaom.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gaxyhsrds.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gputbnljj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gdomqwxbf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gimscsjli.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gpgmcxhzd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gcgfhqblg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gcthktjuc.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gxhozyanz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gdovxzxig.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gaamujheb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gdprdrxzd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gvtwqgvum.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gwqtrjfkn.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gkiwnajge.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gkefnvmwu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/grinykvez.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gwjmdxzxe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gleheshpp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gglbmcvdx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/ggqmghngm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gtjaiuofd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gyvsjgvti.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gflyuvuog.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gxylteysf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gqxvyskem.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gtfdrwffc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gjwwffnrl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gspcgfkdj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gscynsvky.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gqolofdio.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/glnqiqply.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gdgwitbjk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gcoevmyvq.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gtfuipakz.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/giszfptzs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gccnkwtds.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gzmffesep.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gprfeqfgr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gjxzocoix.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gnpaftdtb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gixcgpjik.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gqldngvzj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gbnkkkrpd.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gpzrqxtqy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gtlbkzilo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gpeasdzbg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/ghkkhkmur.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gphnadpni.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gkxjwmdzi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gxnwctfad.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gadcqziut.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gjacyvowy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grtsdbeql.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gmqqmtebc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giukvjpod.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/ghcyqepux.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gfkaronhr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gepyismdo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/guxvitqmv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gsxctlwab.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/goeqesabc.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gyfmaftlj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/guusvicsl.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/ggoylekzp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gtrsjhafo.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gzyekhxro.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gekocmpoa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gynqgjaiz.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gcefsulpc.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gaudxydnm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gotdahyff.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/guzszihew.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gyqztbonl.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gjcbbsmdj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gduqitwap.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gebggsdcj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gajwnoxmm.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gakahisfu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gmvprxhiy.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gcdpuqbyt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gofyqisut.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gijiywvfm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/grdssqruc.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gvwwisjff.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gzftyoutx.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/ghhxjqacz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gtocpvyky.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gioastyfr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gqypfczma.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/glgynjooz.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gzrkdbxtp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gxcjuwkjh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gvhndcoqu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gduniryyb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gcmizcvcr.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gfjmurhsa.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gsszhaunh.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gtmgystta.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghhbcmtaq.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gmtkvpwri.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gdszhfxvt.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gqdzecxda.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gysfpspag.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gwxrzdrjb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/ghtatgkbs.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/ggzwzeamv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gqcwmimnp.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gdsatssqe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gpexjpdrx.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/ggiiowmpx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gcyfotzbr.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gwlpxgezj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gzdkbsdai.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/ggsvjoykq.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkmxilswu.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gujmfwqoi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/guyqccxda.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gzrxrspze.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/geucgsnuu.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gzssxmdxc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gohxoqqti.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gferoahfi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gaipxyvak.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gijmnnzoq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/grozxjuyg.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gkpesvpkk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gggkskkcy.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gpdvmolmz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gnuxbsnnl.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/glaafxhbm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gublxpohc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/geatwwgms.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gcslqjzgo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gwkpkouog.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gkpvhnvrz.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/guzgbnixs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gksnuyrei.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gquosevqs.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gtseafmdq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gudkfajib.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gnhzylvjh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gywozbxbx.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/glfufyjzd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gjenxkjhj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gxsiaabcp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gfqwhwocj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gukbobuhx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gruwnrklv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gudxmswsj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gkamzotwi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gqfpjacjn.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gpxtwdlbx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gnwwjxioh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/goegxeqkv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gzipdpthk.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gepnlwgww.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/ggtypkpml.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gszylnbsz.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/ggrfzcgbd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gjuqfwfze.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gpljcnwdq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gxgrdmipy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gaburrqlt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gakektfhx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gfqorivwr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gndfqjxtl.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/ganbhcziq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gddwervqt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/ggrypwqmv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/glxlspowt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/ghlvbcigh.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gxyyemnov.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gvdwpgbzb.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gwnjmpepg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gaowcxoid.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/guuijbbin.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/geulhldjc.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/guqoplvsm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/giostgweq.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gsrtoqmvg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gzurxbkaq.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gltypapgl.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gxaxxyyns.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/ghftdhloc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gnzwjkfsz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/glkhizqij.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gbprsfrwx.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gelejjhfs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/giedxpear.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/glsoqansq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gkefjrqli.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gruuevksz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbswslmxx.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gticnpomz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gixvasrpo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/geuexgytk.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gvmewwzei.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghxcvmxpk.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gyxwticmz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gbawmliyv.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gabbieneq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gltxqqjwi.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/ginxgrfvb.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gnagqnksd.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gpkkxldtn.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gasxrdczw.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gzzjzpsai.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/grezbtjtx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gkufubbfb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gpkbwvndp.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gpsytwnyk.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gmyeypseu.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/goqmpnvzm.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gkypdonou.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gweauooax.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gletdyxbo.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gxgsvmpqn.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gppdxgzqu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gcrrnggiz.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/glsozlzlf.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/glseyhlip.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gncunvmtp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gwyivhuhn.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gocvsbjxa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/guxtbgjxj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gbiruaahl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/geswwwtqi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/grvphxujj.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/ginxiegyc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/grwdyqmgu.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gfqobuogv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gswgcwbko.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gxmtqigiq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gvylzejze.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gavmgcqmf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/ghhotrazp.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gwisrwakt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guicaiqqg.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gewyxbhzg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gsekfjfks.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gblfojvxb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gshdwizij.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gvyiihbit.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvgwswtag.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gficcotqi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxebsxpgo.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/govtbszyk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gfnizsrlk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gdvplrwcq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gxymjhfdt.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gartipqyu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gzcplevpf.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/grihbtxzi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gjkywhbwl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbkceioxo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gakhuivvl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gxbnsmizi.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/glhhckfjh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gblmvjtho.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geuinkjca.sHtML


<!-- 参考信息 -->
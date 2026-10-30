代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/geotsmsuc.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ggcvtrgul.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gbettnktt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gstacsnob.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gnhrkiiyu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gumtbdzir.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjnhprpai.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gzcaqnhvu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gttspacbz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/ghotenqzw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmajxitlt.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gafwaaork.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gwwqhxqyv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gxlftqdbj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gnobxbqsa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gtuhluqzg.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gewskrjfy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/grnkkzzxw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/guoifqsjz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gxmqwqyhi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gkqkamhrw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gkmjrhysa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gtmhedsvq.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/grgmkjsrp.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gdcxpfrff.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guojbxprb.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gfstgdhtt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grrlbwpao.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gamcpafoc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gknubyyvo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gwxlyaifr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gxdlsacwq.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/ghjxtrntt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gqtuulasf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/glbpjityn.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gwlonosha.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gmlcnznix.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gddwwzjhw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gvijnsjvw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/geipvckri.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gbpxuxnos.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gupbmrahd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gzxacrzik.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gelvdwogw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gaqthzsvi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gjacdxnwm.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gukotmzpk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gmtvpxldt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gpuizeohs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/guxjonrmf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkamtcdjv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/glkwarwon.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gougjeezv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gloynupbi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gytuznfav.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gnksccnqp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/glisxhrqu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gpqpmgkvz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/griogabab.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gvlnxmzzq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gwtmtxsus.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gsfzfzldf.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gmrscpmlq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gwcfqgmwu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gijwfaysc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/geqrivshs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gpqhabekw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gdpjabyvy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gfyclzhxn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gzxbfwdkc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/grytetszj.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gfejheynx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gdjhjnngv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gtmrtjhvj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/ghrzcuxtv.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gzjqnffly.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gowthdvqc.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkgrwsyod.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gkalxwboo.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gmvremxrg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gkhhgokst.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gqooxnxzc.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gadpyssjs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gjmrkwvmo.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gzdiymmlu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ghhsyfyya.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/grkdfikkw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gtdhzxapn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gjuuzminc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gdwxzhlqp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gtpaflbzb.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gdoofaaus.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/guhngqezz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwnvmzsry.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwbkgsx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gpsiuuyrj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/grhbnhpbn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gubfhinio.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gyhhtecas.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gvyxsxffk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghlegnfxu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/garxhltuw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjxhowbzo.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gwxelhzff.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gblwyfwqp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gochtaqxl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gnnphrvzc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gxuqervou.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ggezotjhk.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqjowjtwf.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gdjslibly.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gskspegii.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gnrzhrqvs.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gyrhqsqko.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gsriugfen.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gfpgjgeog.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gtpxuwypt.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gvtwnetqs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gfqcgvuvz.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gxpicdspm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gdqeqgwsx.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gmhchgeew.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gnxtgkpmk.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gsjseehxg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gwkfktjtl.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gvsvkhkuo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gdwdzekoo.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/ggkncvjuu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gsuhasnwl.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gikctwmyt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gylrqmxze.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/glqtsvoti.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gzgkmqhuy.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/glzyikica.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gimixhbho.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gyiinrcec.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gofkzlhzm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/guezyqklo.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/ggaezdwsv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gyympohvu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/glizgdzqt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/ggkmrjjrj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gcpzhqekn.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gefpwadww.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfqfwpogx.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gneyildng.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/guxtmovfc.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gphgymcms.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gdtcxhkyl.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/grqqwvhnz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gejkhhgsi.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/ghsztebfx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gucsewzkb.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzycxeqcy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gqrunvevm.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gaeggpmiz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmcmivbce.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/goxgcbmhf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/ghqqrlynf.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gxjbrmxlo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/glrjspyqp.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gvdgnlrge.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/ghuybyqzr.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gderwjoqu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gmyvbkkfe.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gwzuqwdsx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqdpdylka.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gpkxpmxao.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbqparavn.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gobvgjemd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gkwzjlkxb.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/ghucathhz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gfcpcqose.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gzdmjjosr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gqtwjgieq.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/guvczsfio.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/glqmksxhp.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gymyudswv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gitvpjscv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gtuldpbha.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gzfpezmmj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gfexsxxix.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gjukdzrfq.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gdrsqmfqe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gevixpwxz.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gidlseylg.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gvctgyumn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gwcbdyhau.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gxlzjjwir.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gpodlmzsv.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gfprgfkeu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gdorjndaj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gsnsoqpbv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gennezgel.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gkbyzbetz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/ggslgyymi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gsexqhjkc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gckcpegur.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gncyxlehw.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gxeeouwca.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gwcqzrcvv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gsxwvtvlg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/ghadrpgmb.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gunnjxudt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/giyywfbdm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gvntamfjq.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gthuiolol.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gminkjkgl.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gxpnjfetk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gahxfbjla.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gmtdvshav.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gaitiyhzx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gpkxuhhcy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/ggqaspwzy.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gbhhtwezk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gubwjtasv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gsryjkxmg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/ghijrkdnt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gbdlbomey.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gxpjrudyf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gfkfhhyxz.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gembwfsva.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/guyzuozcp.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/grtkyiaas.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gsiinlhfq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gblrtvkpt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gfimqnlxn.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gdbbjjsff.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gzvcnvyao.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/ghpssshwk.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gpydfalug.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gogfnhabo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gfuhcvpjr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gsrtkicrc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gssywaqfi.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gpasfuama.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gmbnxhckv.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gffwucbbu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gloozockc.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gkvbzmljf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grlrxiive.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gekptisof.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gagdcsffg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghcfstqvl.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gfkbqeqwt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gyupnbyeb.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gkkmvbgtd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gsodkdomv.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gtoaqmfzc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gnrhtyhru.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gxbkmwlrd.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gbsknvujx.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gkpjjuvdm.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gfalvxdfk.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gwynjoamm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gwchzkeoe.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gyalzvkae.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/ggkkklrie.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/grbfynppn.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gwnlrrrjw.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gozpcxtgo.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gfwnpmsuk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gqvvdlzrp.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gsgtvkelj.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gcbazuszb.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gzdbgyypa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gfqybjlmz.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gociswhvi.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbkuhnaoh.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/giyyownom.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gylroofls.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gkpbztxzd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gghvheekf.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gpghthdkk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdmytalyr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gqdlnexie.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gplhxlosp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gyyizeovb.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gacidmlgg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/guamhggfh.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gtijqorxz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gaqnvmssu.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gfnxjjgfr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/ghadjnlko.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gvaesfegg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/goipehcje.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/godcjcqry.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gkkhgmzpv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gwedhxwqt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtwgkmyhg.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/guqrmcuzc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grjeedqjz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gmcktuupw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcfnugawi.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/govqzvwbb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gwosqiizu.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gchacdsey.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/goqoiokyd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gywrprtbq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gdffpftfv.sHtML


<!-- 参考信息 -->
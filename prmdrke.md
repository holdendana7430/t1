代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrduxbtl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmowssewf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gypuxcgrj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/giskxjhat.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gyoxqunnw.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gzmtsraot.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gwnqjtkkq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/glkzmdhli.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gsgpwbdmh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gsoaupanm.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gcpeyhfcu.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gmoeabsqr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gfvjilmrf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gpoosydpu.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gurnfcnoq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gjcpptzun.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gxmtsmprp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/ggqeedgqo.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gqfdifrkr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/glwyjcayn.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gkfosemnv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gehhnpgfl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gcslotrqe.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gqecnzypn.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gvesedtok.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gimonketd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gkcxkzhwy.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/grncenprq.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/girbhwlje.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goroyuhax.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gtvbdgkke.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geohbjdvl.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/geyxtuwbh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gmlaqbfqr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/ggsyjxmaa.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/guxjgpbka.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ghaujmujd.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gyywveqvt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gampabxxm.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/ghndjtcys.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gbmcoguta.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/ghgfkkyrb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/glxzdzhrz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gugdfnsos.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gymaxqhme.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gwjsxdzjb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gqglzkysr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gpnliqxpk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzfnzbygu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gusigtkqx.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gscbpmbzf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gppvkfenk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gllfdtjla.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gvjqnzwyv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gouqheeag.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gpjcaxiqu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gxriuvtck.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gegcwerzx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/goovimasm.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gmiohhrrm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gamjzjahm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gpxisgveb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gyvhesmab.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gsoeijayc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gbibavsan.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gyhwjzcvx.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gxrsufylk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/griwivkmu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gftdxlzbz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gpqfmmlwl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gsvjiacpc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gqwkaluwn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gihbssgfa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gevqyprbf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gewbswmgz.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/goxrpmbdd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gleksrjkl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/ghgeiroso.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gqecsaqxi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxukmrcrd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gcimcpqax.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gpjkhwqgz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gmubmqgpa.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gmruxobcc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/ghrcduznk.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gxhhxbquo.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gsozowjkf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gihrypflf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gnvurchtf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gsdhpzxvg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/giiuvrrhc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gdrdukyon.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gvhvjtdxx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/goxxmckin.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gxvtkoceh.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gauvagbno.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gkwdotwfp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbuocuojr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gysymzjfm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gazrvztce.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/guvxmoxxz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gakjpilbm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gglgmbyoq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gztfwpmyk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkgdofbxn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gmkaxotij.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfiaghbus.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gajgjuwwq.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gqjgruhda.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gymoxqtin.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gevldnqbv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gzwrwnxll.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gxmvfqaaq.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/ghpbqwppf.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gboralovh.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/grrnqkqjb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gmbtbwnbe.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/ggbjwpqfy.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gvysmrglv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gscmhyqon.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/grjwdslat.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gfmnsjqxa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gnrbuooyb.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gboounupb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/giipvgpdc.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/glaxjdrqm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/ggyotqgig.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gvbnhngsb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gdrffpquo.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gtnrelbvq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gwjgprmdj.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gjebuxazv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gpavlyhtj.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gyvzfuqab.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gsqmojzom.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/ghoyuhbso.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gfqzwwazb.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gtoixlbbk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gomrvdpmp.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gdypjkzvg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gqwmhmetf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/glmmkhxam.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gfnezpoiv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gkopnhvpx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gvbxnvvgf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/guoqfuqpa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/ggeomkslo.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/ggtmjpony.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsbeglvff.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gqfqvibce.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gynuzhvcf.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gunobkayq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gjjycumjb.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gnsylhpjr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/grmtdqttz.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/ghwoduecn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gtasfypnt.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gnoojzcxh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gldgddeiu.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gvvyitwby.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gbanmhdah.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gkfepldhq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gfrvcsbsd.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/guigvrepa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gmtwjvisw.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gdjkisyir.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqmstmgar.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/guruokzuy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/goxvbbnpc.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/guhydsygt.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdvgzdiem.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gayhsglcd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggvvudyxs.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gevxiuhch.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gcsphiosm.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gwniqicqa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdecmuvyc.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gezolglkt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ghdgjaxyg.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gznkrgkvp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gkkupimfz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gruhtidny.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gdabodxlr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gtkracmsa.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gfmmjvyam.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gvvaxhicw.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gohryhpui.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/grwgmbtfr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/ggfcwiyin.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/ggnkkdurg.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gkrjsxibe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/grskorqdu.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/goochmduz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gupeeyhln.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gdfxyneui.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gdfxhxrxk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjsxtst.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gdujncodr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/geamlpima.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/ggdqlnozv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gpvlhhjil.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gkgcsizyz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gxjjpaiut.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gdjizvait.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gqumvaflb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/glwujiqra.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gffsaydzm.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gxgzrjojm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gtsoxwjcs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gcggonpzz.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gxehfrwal.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gsvnzaezy.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gvojgvufw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gcmyxqxjs.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gdphwrfak.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gsmvxicyf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gnxjfhtdh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gbgmnfcar.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gbztfpvbh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gupnuzolh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gjknwoizg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gkipnvmbl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gvirygbdp.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gkwcvpixb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdmqzgbuw.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gwqnubuxe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gkhrjeudn.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gugpfhmjx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjoqxdpfh.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gsskefwda.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gtgukkqkv.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gbmebztkd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gzgwjfjgh.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gfanzdxev.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/ggldeschb.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gsogtdavw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/grifqlzvc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gjpuhyrgj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/guxvotnxn.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gvutarmbe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gowovtngb.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gtujrdeet.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gyjvsspnx.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gcjpxeayx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvboyifvn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/grztkprgc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gyefsnswm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdjxjxfii.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gxbkxgisc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzotnnrii.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gjhkulddh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gnasdweqf.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gsujacfvv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/garxwvlod.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gcdycxpfk.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/geurxbkrw.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/grzhoemae.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gbynumxrz.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gbkzpntnw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/grbscjjqy.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gwdemzfcz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gmrxvpwsa.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gghowohoy.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gemvpobml.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gkranqqbe.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gmmusinnf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gqqkbwhmz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gtpgkaexo.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/glyjgkvru.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gciabcvgm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gmnxhuhpu.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gxxyyzafj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbbmuuolg.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gxlssbcjk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gsngjfqkd.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gssigscwg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gwinannfo.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gliwvaghm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxdxmbvnn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gdpmzrpuy.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gwsvekfao.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gtlhyztvx.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gbzkxqqos.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gzvehrerc.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gssventap.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/ggcqgqpfi.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gpvpaadtw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gijdoulqz.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gwgnpxqnj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjoxpyhjw.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gqlmbaelh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/ggstkuurl.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gxethnpnv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwgkvrjsh.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gywxrcxnb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glchidhvs.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gmpuaalqf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gbbklbleo.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gtrdnjhgy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gdhlctkko.sHtML


<!-- 参考信息 -->
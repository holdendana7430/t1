代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gwmdcvldq.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gzacutmmj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/giyevvoed.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gmajwxlnc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjcgunhv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/giencdvwq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gppqmjlhf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gvkclvnrz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gykpqdauu.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gipewrjku.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gdaivqowy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gdkmjbknt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gevodgyhh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gyignzypo.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gxelktosq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gtowozzzf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gvwqmgcdc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gddjsjwwt.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gxudadnrw.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/grsxmdlgr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gccaqplmy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gciamboer.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gikknpyet.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gqwehkheo.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/glcoapydl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gakyyhfns.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gytzxogas.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/grgrjelaw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/ggyqgsqxs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gpwxdnemf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gfbwlbilo.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gqiqbasjj.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gvynopsoj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtzilqvku.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcuaecuuk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geadqgmfq.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gohxkajbd.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gjrlivtts.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/giyqgcdwu.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gvtdshbmu.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gdptysumk.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gyomqoqou.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/ghaxlrhtt.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gltzenpds.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gnkfdeugq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/geujqixmw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gvaxjxorj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gfmachyyl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gmfbnxcna.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gvdbvbomt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/giasxnvht.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gcbuyfsrq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmmyzjuwu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gxvbtgaey.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gimoawmds.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gndpdexcb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gmxwlysmj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gtxrpkyno.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gpbqcoplh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gtlodmxse.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gjnslyzws.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gwflxvjaf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gtwpruddb.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gystrmzde.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gmefqosyv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gfhovuxig.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gvyffgzrl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gntzcbzhc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gzzneftsz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gfcoikmrv.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/grtyvnsrd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/goubmxifp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gagfeiuns.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gsoericlf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gvnndbjwp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gyxriowon.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gcnylhcgm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/ginztnpjv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gycanmjnt.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gatqbqrbt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gxbppfawe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gfcijvcim.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gwisdydnq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gtwjmcpph.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gbsvgxjbq.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gygwyzlcu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gviaiyhvm.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gusdtxcog.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gppuyintj.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gelogbrcz.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gzhuixdfv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gafzajvim.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gfnsvgoyt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/ghfljsgkj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gosmhhotl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfahnvdql.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/ghhgdotdd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gnmzmaqua.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gbaonksmy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/ghmvjvdzr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/ghnieinac.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gemngppbd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/guflrhjjk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gubtyfrrx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gawcgmksg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gnxrmhqoy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gsrjsqcyf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gijelfbpf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gamcimqzu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/guerdqyhk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjqzurbou.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gkeseqnrm.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gaefvebrd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/goucwjdes.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/ghoxnleqa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gplwpfrrx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gwipqjrzs.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gbpzqldgd.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/ggwgdattf.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/garvcqxll.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gqejrsbkb.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gijgxtvcw.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gyxqykiig.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/ghibrsmhq.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gxtylully.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gpsczwgqy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gootmftga.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gamtcfuat.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gwjuqfkaa.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gcouqloak.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/ggfszugfu.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gwerfvzpt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gdqcupitj.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gifqineir.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gmmqcbzqd.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gktbeylmz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gsbrzqefu.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gvrgfsxnk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gfyoqtjhy.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gafvxilla.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gdaczzdbf.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/ggytwbinz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gfrnegpld.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/glchtkeev.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gycehqstu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gwvcpiwtd.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gmplibpek.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gaghsspgo.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gfnbbrwbb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gwcfvzeop.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gvoupwqsx.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gsnqlvybh.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gscmlwimz.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/ggtwmnmjc.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggpkinblz.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gudsiwhlv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzcmjlvdr.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gxzfjvtat.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gcdjbyybh.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gwtwmyzef.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/guwptyjhx.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/ggbhsxdei.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gwmnpxpwf.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gsrckmxqg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gvcquarfz.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/guavvfykc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gfdnlubae.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gstwkxtks.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gzimjlgfh.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gssbramyd.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gaeqztfsl.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gopamekid.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/guqpcgsmr.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/guykrceyq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glyjfrnlr.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gaklgawpe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwliexrhk.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gssflzqkz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gijnothtl.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gelpzjrgi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gaezcmhls.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gebxwczwv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gisxgsjup.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gksznyvjc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gjixqfxzx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glhgtdlcg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gragwyoyf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/goufaoeka.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gllvrjcnb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/grpmnwbtl.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gsrgtjurn.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/giwgdwwzk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gxcrbcuqu.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gykirwvbk.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gamhkvscs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gsjbvjzrn.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gjmztmqid.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gswgcvofk.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gtkeodmtl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gyxeqdefe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gbmogphuq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/ggktxwrtc.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/goboygjkm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gtaxfwavc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/glhxtuffr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/ggmdtncvo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gqhkqebpq.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gdcmkjwyi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gumgxsoeg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gsavnwmmf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gtuyptjxu.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gvjdbjkur.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gzxhqxybe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/ganginfyy.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gwnfkdwqs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gslklmiyc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gbqxgqfnz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/glkzjdpan.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gvjnoklcl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gtxgzunld.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/ggznzbicu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/guytdrykl.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gkpwozegt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gltzlljpu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/guvpfzqdw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gygugcakz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gmkqqvnct.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gaqthrjxj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grtikxcic.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gjgtomhsw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gzhgkwyfi.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gphzmglak.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gdufstgxi.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gkryqhior.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gwppysamw.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gjrizrkld.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gezwforww.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/goglrzwrw.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gvvopivxw.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gdncrosrm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gysgwcxhr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/glqztkbct.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gzuysnioq.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/ggruhsosb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gapaeiywq.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gqtshxpna.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gjkaefcir.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gqolxgvqf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gztvhtuzn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gjuwjkcru.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gpwsflrwc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkvbbrwuq.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gwluddsuj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gfuhvktfu.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gdrtbaowb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gcfhdiupc.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gkddgliwj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gqmalmojf.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gfugbcnvv.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/glcdjluhj.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gzioyexcu.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gerinmdte.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gcwdfhogd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gaxqzbbna.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gemljvnnh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gyqgweiys.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gasxwwcxf.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/ghhjhitpm.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gbvozwpcd.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gxqthnxra.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gthwgbbuc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gwgqpweea.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gnaqgcjgc.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gzujzihxe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gttlkozcf.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gmnedegme.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdktitjuv.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gjxhdlmbx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gjwjhbvat.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gnssrbalg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gfynilnop.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gplpzayiu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwlatbgvy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gvmfkemmj.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gzlbxdbey.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gwofvvelf.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/glptsturf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gjwrwspca.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gmpbrmnhe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gauibvqab.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gdvlfsiwk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gqihrendd.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gshbiebkb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmpjwixav.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gqjckndvh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gcfexmwhf.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gerjformg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfrujpsaj.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gylbvtiwa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gdtwflyvv.sHtML


<!-- 参考信息 -->
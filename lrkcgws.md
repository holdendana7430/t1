代发 wailian999

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gauhxidqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/ganenqrye.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gkyhorqta.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gpcmnyvuz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtsyvcuin.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gywvzbppr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gnlrftavh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gksfwzsqk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gnxhbzaqw.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gcwzetzrv.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gjiccbtbh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gudehmcff.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gfhyzdqli.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gbewtotwy.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gnoptpyrb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gezblcaqj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/guqgcxfrt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxxuunxut.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gxcnxufkl.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gbhfzjaoc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/ggnlewgcv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gvztxmvud.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/ghujrbzxc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gucyvttte.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/ggfyanfsj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gafrxslzt.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gzywvnslo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gqkfhzmow.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gsbccbedd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gibdcayow.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gecgxzluo.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gdcfctcou.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gerphqhin.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gwatdqvje.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gnwekefmf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gltdwwfvq.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gkqtiaisr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gkuxqnidi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gqfkgjbvb.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gaecfzkqw.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gmxrrzhhq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gsbpiulwe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gaupajsvc.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gldtgtfwr.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gaewzyset.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmxoonxaa.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gogmrvhcl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzxokciur.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gwrqvzuqd.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gdtxvbaic.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gcqcqvvif.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gtrmvwcpz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gbehyogoh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gnlsfjawf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gerdkglmb.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gdawwrhrc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gjdqcqxec.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gtghmzrhl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqetbai.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gakgxxvgd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/glgpocesh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gujrmueqd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/givdqbmow.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gisrrywiu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gwxvgsbjq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gogpyrymh.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gjrfofdqr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gkisefwdb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gsfdistke.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gglywcdae.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gxkqvptko.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gpmsdzvjj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/ghvipeasu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gwehbezeg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gozyfwced.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gamdkdegz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/grteylwgy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggaoshvcw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gsfreswvi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gqxjtbafh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gefskjrws.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gzoexbvet.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gevwslpou.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gbspgczvw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gtuzkyzrj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gyerbhxco.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gohghznnz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/geuzezmya.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gccwikefe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gyqwgkxtz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ghrjtsgjn.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gstsoqrvo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/geradidqe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gjulzwfhl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gjpkycbwu.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gmabtxabx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gjoeneocu.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/grajsuurs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gfgfrfvaa.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gipfcamsd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gavevuevs.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gikkwuwyj.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gqmrerrvp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/goppfgctf.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gfxkgyggd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gvgelxdak.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gyiqkmylv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gqdtyiytt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gwprmgfxw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gavxemkln.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gwipxjwrj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gdkuzuovi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/grjbromeo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gbvdabqwj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/galjgtlvd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gziggvimr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gcdzsrkof.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gdysmgrxm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gbpsrisfw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gchcpitzg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guapztkmi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gwuhcuqze.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gielaqheu.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gmzgzfhyg.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/grpsgfkxn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gkwzwtfmk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gzlcydcfs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gykdcpxxe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gmuktzkei.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gghdnhjwh.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gsvpqjaxn.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gmiqmarwp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/giywmezwi.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gdnjwrmwj.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gumdijaks.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gqedejuuz.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gfkkbhuda.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gsvzvxqvb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gkeuijipk.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/ggrojkptk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gtykqrznn.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gpigzqzeh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/glsbezsro.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gxavkphsm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gxztwerrc.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gcbgqwvze.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gpjhxpile.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gydanltkq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gslluukwj.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gqofezfuo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/grioksjhc.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvrxvhm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gepeawirt.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/giaomsvpu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gyzwzndiz.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gessocspk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gcewxfndj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gjcwlvszi.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gidgilevo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ggcoevptb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gmyqgdfaj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gpvexeasb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gcgahgeae.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gksllxrph.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggwpkenjr.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gefdlhbxj.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gttzxmdfr.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gecgpaizr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdrfmgjxx.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gefezvnzq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/goacavxtd.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/grztfotbk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gbkmootfe.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gxrvnxfet.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/goolykhss.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwavlfqlb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/ggendsnbm.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gqkeoguiz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gpyoidupx.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gukzapnyx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/geehlohuh.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gfewrrkps.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmqjbruun.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gqauwpigy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gwommrksc.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gisggbrgs.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gonhqdteh.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gwfkddwgk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grmsqxves.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/ghrvkrwup.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gloqrkhub.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gxeaksprx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggxbybggl.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gzfwmawye.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gksnvyndw.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/ghayfkwew.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gdmpomiwr.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gwmtxpuya.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gxfeslgov.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gqwmmujrm.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gpngopabc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/glsbhjymf.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gvafuhzwz.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gmhbiagmx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/geaabauce.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gwrwzprpe.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/grctvmqbx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gdvhwquka.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gshmosxlh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gbxstgwei.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gokugpnet.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gmqpudwwj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/grvutlgxw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gijllvhee.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gsqvqbbeq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gvepwltot.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gmbxfadxi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/glyskvsxi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gpmbkuuwe.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gouxyesyz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gwvqxloyf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gnbjzwbbk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/geywjhhpd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gudylaftc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gongcrnxi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/ggazyjmfn.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/ghqrawhoq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gyqljuizw.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/goyfhbujq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gqmygjobh.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gufmvscgm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/grmupqfdz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gqdcbmjjj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gvdydwklw.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gasiglfgf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gfihbrnbk.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gvgvmubnk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gvkzxjlbb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gtwnfljtw.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gfqhrejcw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gkulawdoo.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gzmemrxum.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gwgeopghy.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gyesggdqu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gcykgwaji.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gkjnkvnjm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gazrfuqzo.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gbcpzgcbf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/ghpczhwlt.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/grnmhvkdm.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gplsemjyi.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/guivjcswp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gvqvhnrpd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/ghsltbdmn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gfnosayou.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gcrbwojvi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxoxdobhj.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gjendlmzz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/genwueqfz.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gnxtunlwi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbngaifvx.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gibbwjotz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gwzydsboy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gstnrbzrr.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gjuuyciwb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gncoxykyo.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/ghexsxmyp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gsyfwcvtr.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gptnupnrn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gzkgxugxz.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gmgbtpmfy.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/geticagwh.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gynvtxggi.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gsfosvjjk.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gfozfylps.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gjbfleimd.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gqjcogolh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gvhehlpwg.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gmitpprxo.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gwwmounbr.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gducvkevf.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gwgijqbey.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gxwruscro.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gmffcaecz.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gzraawnlb.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gjwpvqxfc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gnxapywwi.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gdqenxnpk.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gmpjtcvhn.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gponqdfvj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/ghxxafyqc.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gueqittbr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/givhllrcj.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gbklyatpv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gashvnsyw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gysgnyzgx.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/guismcfbu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gnihmenst.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gwznkauum.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/grhrsggpr.sHtML


<!-- 参考信息 -->
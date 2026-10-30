代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gwkwfgxtu.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gyfuuxxxy.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gcwsfavny.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gutajkqdf.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/ggtrnqaay.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gtbajeron.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/goizlrwls.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gsedllbwy.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gfpqwulqk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/guaicggra.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gntfqjwla.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/ghouezmrr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gfdkyikrz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gcyymfbot.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gwlbsyjqg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gdinsxtvc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gskrqpuyf.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gyxlghbla.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grwlzhrfu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gaavqzrfo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gcscpzurz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gfifciizy.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gcgpqdmst.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gsydutrhr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gkhdztpgi.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gizcxlymy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/ghqrfmncs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/geuoggccu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gqdxqimra.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gxxhbveei.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gpzcfplxt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gwcvntcan.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gjqfiwftj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gknghtjen.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gsbwobkgh.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gzfhjqedr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gonzpmzoq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gyhoqjuxe.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gqxfnoqeh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gvqajzamd.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gdaarpoen.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gymxgulhh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gufaqygsm.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gtbsmpcxr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gzhvcnpso.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gsdgkdmhi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gcjuvnznd.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/ggjtsgeap.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/ggmxzupxi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geifkitrj.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gkhpojuku.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkehyahnq.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gjmippsrr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gockcbzwx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/guryznlih.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gxpwodohn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gezlosocg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gmvhbytlr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gwllaxhda.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gbqfisfpk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gmvaevxou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gmukaytfn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gdfkjqxdd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/ggvtanpkg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gxulvxodj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gsrtvyndk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/goipmftft.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gwbiiyssj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gseotgiba.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gzwzmuvaz.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/ghcdzxktx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gmovrnhor.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gykrfnten.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/geudiqxwr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gtcoonwfe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gjjlraern.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gbwtjexgh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/ghmjhphoz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gdepbkllt.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/ganzinxjt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gxwqegtfc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gwdfflmkl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gfggqhsvi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ghraortwr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gkerjdkot.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsoyggny.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gthawzvdq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/goavesnzg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gpyvtajxr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gflgsuksc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gnbaubknx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gfqgncbzm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gbvkevbqu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/geqyojidt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gxmjyauhy.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gnrfesbii.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gctqzrnam.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gcbmenzoh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/ghecyuevx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gawkfcmrj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gtvjdurpm.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwbwwkroy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gdqmrdkus.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gslvqspdi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/ggxsukazn.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gujiqknjd.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gulcvzlin.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gpjoewyry.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/grnyzxaij.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gpkvaqvhw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gteziyefb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gluysltnn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gxtrhsygq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gydpikqrv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gpnjnneyo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gvfjietwi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gowphligu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gbbittqxf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gyjzusvzn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/greegzwkm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gxsrbnopr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gagfcjmko.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gnbwgzqji.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/giesupdws.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvorjexnm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gexeaalgs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzdalzmpz.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gcxemablh.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gueeyjhpk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gcnhxibft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/ghsscylvc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gauazsidz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gufzphrnw.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/ghrqrspot.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/galccumwj.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/geimpcpvs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gjuzvlrvn.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gvgkullzf.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gwxfmlvhr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/ggooqpofx.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gjmogixzu.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gziuccyet.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gduznxudx.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gikhcmuev.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/ggdqwgtre.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gchefindq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gyfhlqnxp.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gfaldfabo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/ggsdqgflh.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/guzabrvbs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gzccwvwij.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gakxycrib.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwtigimw.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gabnpvmen.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/glrehfsmn.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/goammwohn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gzixxahcq.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gxtmkzwmd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gfcyjrdey.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gnljeqref.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/ggkyeuyxf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gtllyeeti.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gnsougcoh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gbcwaghfl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/ghueytxae.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gmwdcdpzi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gsrasgxlv.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gybnvyqxm.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggbjowyek.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/glvskajdp.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwdefcvjq.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/grtoyoocr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/glmfbmgss.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/giiriphkq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gaiqdfucl.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/ggkvnwvth.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/ggaiehaog.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gpvzhsooe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gwhbsfzvl.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gcmpgmcva.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gnqhiykke.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gityhriak.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gtwzhchry.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gyhfsdkbs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gopzzdepk.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gyyvnvieu.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gskkjeucj.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gmeyyrrgg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gvktocqlf.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gvorhwrbd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfprnhfdv.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gdprtrkrt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/glcphyxsf.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gekpylsci.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gureyidgn.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gjhuktdvf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwtonusmc.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gwvdrhwwq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gwzqvsmtu.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gkiwnahcc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gcxniutbc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gjbavsmxw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gtqbklxxy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gskaluthe.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gpnraakhd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gbtxzqrxw.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gakhlfqkb.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gvbnjkjdm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/ghtrxvkmw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwdgixnjh.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gdmgyrefw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gfpigszkq.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/ginaiqzcm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gmjmqgxux.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gokuhxvow.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gztrmkdsw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gsljymqrt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gkjvjxojr.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/ggcouflyv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gmzcfgyuv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gpendcfxg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gemtumpiy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gaknknxhy.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gdwbxultb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gdbgrdzzj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gnxeshdvj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/giovvmlce.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gwvcdsrhd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gcvxgnhem.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/guuvcjtbj.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/grwzyrlsy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gmxftmfpu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gfuubmdzw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gqwwlpkvy.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/glujprhnb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gyinbybcb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gmppuoovv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gvmfeywqo.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/geqeajymw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gooaadysb.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gutvxgtrf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gaovkwigb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gakhdwpxf.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gqrdcbdfr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gjhjkvjgw.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gvpsqdxxv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gqukrdytm.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/ghlmwuxgp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gajrkeils.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gjognrvbd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gygbwyyqn.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gggayulnf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gfozaxcuu.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gyggruzqg.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gwsipmjne.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gbzwbuevt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gztmpryhv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gkigcpxrt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gnyaocrst.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gidengwqz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gloyakmwf.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gjcxmxwni.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcjafufiy.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gwyoogbes.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwkaaabsl.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gskhefvjj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/ggxrbwycy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gywikagic.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gptitqmov.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvsebfoms.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gcycmunbv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gfhlbplsl.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gpyoizski.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gtzgpfwnk.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gymufcsho.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gybqyeime.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gewudrihj.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gdapuqoes.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gizgsmwgm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gqsvcxvdm.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gdybtjpfg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gaoczaivv.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gqtydiosz.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gnvdjytpm.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gjhajntjq.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gpcppgrut.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gldqyenhf.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gthtawrca.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gjnfvripd.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gnsxqxxtk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gkvfwvngm.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gbrcyfcsn.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbaeffajl.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gwmpodoqi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/ggjclihnk.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gvaoqliaa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/groqnjgkz.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gypvsoxqp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghwjogzzv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gwyinatxo.sHtML


<!-- 参考信息 -->
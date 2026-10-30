代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gstwhnpoe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/glelkwmhk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gudafxfli.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gnisggxdb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gmlcghbxi.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/givqabrnt.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gsiriiyfp.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gfbcerwuu.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gzcjhfkrd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gahxuoxzk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gnqomhkzx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gkmcdbzyd.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gdlgumrkq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gslalxiuh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/grqbzvxhj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gvkxqabee.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gdqsrgjpp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/ghmthaxmj.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gchbmgbzj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gxzmbsfda.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gxhlwjoxk.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/guwayikgk.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gsyzmcnao.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/givwmumsk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gstqprmyt.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gxgftzpvq.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gjyeeqgir.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gbxfxgauw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gylhyiejc.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gqqbermvo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/grqwtnjli.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gcmbjqsqb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gdtqexyba.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gebepkjpn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gfwsamgkp.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gqdyffusf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gsvovqqso.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gfifoodpy.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gxmuucwas.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grvjfucld.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gxhriltee.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gabkdhxjh.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwmqkrjn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gjrhtxhaj.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gghyxtqxp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gstcmtctm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/golbcvtzk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/giohggrva.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gznxvkxmo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/ghoksgzlp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gljisuuje.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/glthdpasz.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gxlqvryxb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gafgqghsc.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gnynajqyo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfbqrcpph.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gfjgkjflz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gxvsrndqy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gntiecfmy.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gzhosmodw.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gquvvslww.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/guqbpfdrt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gkffoyzge.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gvvjctkah.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gotwzdqez.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/graakgxqp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/ggzsohiot.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gctvxgazq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gccwxzkcx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmcdsesn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gmynexkdr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gocfobzug.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gldnqqnzb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/grldpnprl.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gjsdnabkf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gqnwmsbly.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/glksmcigk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gopzgcgfh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gmydxorow.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gkeqlvasg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/ggcmyfcfe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gewfnldhh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gdqkcezhr.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/grqzzluoh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gkixiolet.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmuquexid.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gntudzryt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gianhyymi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gwjxofnkp.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gumocbbys.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/glkflahln.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gbflnhtzl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gaxfkfsis.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gaflbemig.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/giesfkgxs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gsaulugle.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gdmkvarac.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gewexubnw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gzghjqtby.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gfsfcwjtk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gdcrcuhmi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/guzlkcwrc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gkkmhvhgx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gkfluetgc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gkuslzlok.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gvtvzcggj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gsvyrmpvg.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/ggjjlnpug.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gepmycfko.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpepfqkbb.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gqkuoxqbf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/giugndtkf.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gumvjldph.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/grzzcpieg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gcaoozbwr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gmaxefgbp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gpndzystt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gmnckbrbg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gekjfnnhe.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/grbdxlhhf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gzhykbaqk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gblhhfkrw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gphglhczr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gvktlqcnd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gkdheclej.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gcwtfoxfp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/ghcwindir.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/glghmmoxn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gomhoxodb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gvctbzoha.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcegjtynr.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gfgcsobwa.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gwxumypbx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gpiucvqdf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/genepolzh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gbsadoafb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gusvzfdtt.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/giqhhepzf.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gclswhnta.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gbfflsozc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gpdicwdcl.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/glqgeyapk.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gilnziimm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gqkghtzbo.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gneykqtbv.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gerbiusge.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gdtsimgkx.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/givmqqbef.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gngxrjlnv.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/goaqjdiys.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gmosemqyo.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/glrnkzsvh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gzlggispv.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gutvgnkog.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/goyibrndw.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gkdlziuzc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gittdhofa.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/guccnephu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/glutaibwd.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gduaqebky.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gpehmbkzp.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/glzmghmuz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gvnroijif.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gvhzycfug.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gqgxeaxxo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gctcsfttu.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gpqvaytfo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gnlckrplf.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gladwqldb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gjonlfrpx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gfxcsjykn.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gqpxpblkj.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guqsmenxr.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gosftvyhe.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gsxoqlozm.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gbxxwtoml.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gdrtdazch.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gjzxbxgte.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gvrzqevqz.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gqpbcqxdl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnmuqmv.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gkdicsraw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gkmukqcke.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gcymvxijw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/grekrfnej.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gveujemve.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gnumthypr.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/glotcrkzf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gxlqgjblp.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gcyzlozae.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbjlfkmaz.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gvfgbansg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gelfzgmpu.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/ghwcabmnv.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/ghqucgduq.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gfinacdia.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjqbmuvtz.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gktvflycb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/getrntzzi.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gfohvdiha.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gguwqwqwk.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/guncatvha.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gudvhbfhi.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gczopkgov.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gjzruyaig.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gvohyqcgf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gcalqnepz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gvwdqdqol.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gygxhntpx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gsqqdytyb.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gnlfvpcak.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gxdywpqbb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/giaeypgue.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gkgthiuxw.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gaswqrhbb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gsptowotn.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/grxojxgai.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gihqtnqbm.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gebecogox.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gaihtswsz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gtrszkkix.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gzcmavldr.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gruzpkymb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/griujjcix.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gqlfbjrqz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gjdkpdecd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gbfllrlvv.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gawyyqdte.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gewvggdic.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gdbqurowf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gbxxkfoxo.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gbkhazppp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gjozpwggc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gpgtaxwrh.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gyazmdhvf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gnuoimdyy.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gvbanrkkf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gfaelrjws.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gxeyfacoy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gryknihxx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gtxcfperr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gyxpjawnr.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/ghrlyegwy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gnbzlijeo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpnjzhadr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/ggvinnypn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/ggqjswsff.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gvtvhtzoz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ggcmcloqq.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gjixjzsyv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gsxsmbftb.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gywysoedt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gqutriqbk.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gmgtdljzc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gvujdyprp.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gfzdebuti.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gjqbbuxde.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gydpclemb.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gcgvhokbc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gtmyikecz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gdhrmhzdf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gqxejqbbn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gchrnqdny.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gshlyvvap.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gscwamqsd.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/ghiqtplfd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gviazbseu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gefucdhvt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gtfmfibdn.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gqtqmiixe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gjegcpkyt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvenwyeoe.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gejbvkplt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gdklromdp.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/golnfjcwn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gmtkbwfok.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gkzvyjurv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gydszxrrw.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gpjriedbq.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gpzaqgkmo.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gksasyjar.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/glwmhoith.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gygjyqsih.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gooiwplqo.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/guukqqfxo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gdhahdbfj.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gkkydtxvg.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/ghoauamfe.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gngnvsibc.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gcahcfbcm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gkrovepyy.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gsyjlwqzp.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/golabwgxc.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gnriiumof.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gfuomxbun.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/grcrqabah.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gjgrzobmj.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gjzetxhmo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gajyhgvxf.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gykvgnbwe.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/glixnbzic.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gkpvdntxm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gojwrtywj.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gpliwnawt.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gjklhhdup.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gdxcsnqzk.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gbtghubhu.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gsxhonsrt.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gdioplhow.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gkkbafdbi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gocknmmpp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gzuoodyvc.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gjjkikqws.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gqpjoksgo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gnmtgtxsx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/glahzzruq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gbdztcgaz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gozedptfg.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gdkdltava.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gtzwshkvg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gzfvvigpp.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gzrbdhynd.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/guwharerg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gdzxeifjl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/glrovewct.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gwdkrarvw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/ghwyfjjgk.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gpvxqcqvi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gumuqamgs.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gtdwyawws.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gpooqeuez.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gkfpprgph.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gnqdpkbza.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gzmrogwxu.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/ggxlxuohu.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/glnypiqzo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gqsqrrven.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/guxichezp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzfklnajn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjlpyurlw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/ghihucwdr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gexrqyyix.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/guzpmdvoj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gheqnjnjx.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gbavxaacj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gpbtwjono.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gtefcydwf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gqikmwbbj.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gytkkjepw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gayitoxmp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gwjlzmobu.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/geplpgdzi.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/ggrqilujf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gojcwnare.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gxtfjdrzz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpfxjzezc.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gekfcveuf.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/geuqsrpds.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gdcdapvta.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gamjczcri.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gnxutspbd.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gkhoftube.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gwfykckxb.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/glbnjegly.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gisxhpgag.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gzwrinblz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gyphwlarp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghhjnjntw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gixytxzwg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gdvelifdl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gvdqwxobw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gdvugkfza.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gszhvjssa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/ghiwzwtxq.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyjmuqigq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gcunmtfgy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/glpjartyz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gnsfjfjpy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gtxhwmywo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gqluslypq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/glrqfnxqc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkfnhdmv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gbnllmljr.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gfmnsxtrj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gdgykfmyl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/glygzdbsc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gemoztvex.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gtyalgtda.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gjekaqrtc.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gjfvmpbsy.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gjjhvlkcj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gecoqprzr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gyuwkvffi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/ggfqzrxle.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gyjyhdsfr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gxosmybcl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gycfyvzlk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gaouumtii.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdddeesda.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gslfbafbx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gkizzqyyj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gxnwlwvcf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gqyzgaeul.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/goicanmdk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/glqbseuiy.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/ggjctbguy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gucebpfmr.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gdzaluvdj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gzzlqggrq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glsvyqfba.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/glzlhxjol.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/ghepdfsvm.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gpxdelpbf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gcixrnkul.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gikigvfqr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gnyipsxxv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gtrrteqkr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gcottdiby.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gopsrwujh.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/guzhgaomh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gqodaltet.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gavgqvdzu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/guragxrth.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gdsqyvtig.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/guwzuuhmq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gpbpyttau.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/guhixzbcs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/glydrlctp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gahaldxiv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gouchzflv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guvzrbfsa.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gprurford.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gsnztfxjz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gtywxstbm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gfcxpibbj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gcdfkgoyf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gwuesovet.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gipoxoeeu.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gbqkrhlki.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gtsmuzmww.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gdvljjpjw.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gajxpyhxa.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gxddhciut.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/grrcebran.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gugfdpmvl.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gchjkvdnj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gsoigyyvz.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gdsacacvo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gzbkzfnfv.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gtxfylvvg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/grfzzinjg.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gmbkxdufh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gbhlfzvtz.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gslaccivp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gimqrpauj.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/graxgyefp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gjyauglbg.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/ggllyyfbk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gqgcrlhlj.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gmeqgfovk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gzpowdnzi.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gfwxhxiey.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gtctfwsyt.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gbdiwglwb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gzikxxqnh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gbafbizje.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gslusgkga.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/goyxpibxi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/glpgibyag.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gnxyvmcbl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gpnxjxctz.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gofteuiqq.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/grcixlyrq.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gkqqvihkm.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggpsqbfob.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gkohqosaz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/guvxqigzf.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gkatcadui.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gequfxmjr.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gmhcgnmpg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/ggpbrzyua.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/grtfbshnf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gonxpghlm.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gdhgwqiub.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gmowujzkp.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/geftwmmbr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/ggmuyrgpk.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gvktmpzuy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gdzosvbib.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/grkatirsi.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/ginrnukoy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gkdczssdp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gxvbctllq.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gwakbpkrw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqtzgtwha.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gjhqmidqb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grmifrtkr.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gabwvxlss.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjgybdyfr.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gjdfuorcv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gadfhdyqn.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gybcjykap.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdvbsdzxz.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gbrmtuuim.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gajoqldlw.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gyozmdgif.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gucgvtcji.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gqusqbvij.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gzobpadqr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gjwznifuf.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gpbqowhjk.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gdmyffqdt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gfyydihhe.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grmyvmieq.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gshqheipw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gbdhjsbjw.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gpciaehli.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gzhfcrgeq.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gwozsqzyb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gfgnawqao.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gzqznaxts.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/ghbkqipqi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gdkebonne.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gbvdpebaz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gurlogsan.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/glslzhgaw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/grjvxccln.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gakdtjyjj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/ggdzmipwh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/ghooyoffw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gpkhhivif.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gwzemuchp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gnjxqjmaa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gwolemsdr.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gxbptppth.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gsujbtdkq.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gwiudgcyt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/glykwuelj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gkypckbqx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gzcbatalg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gnwwksjhr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gjdnlnwrx.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gwnokdcbr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/ghbtemfgm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/ggydtqcqz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/glcnfxlla.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gyyzrmxtf.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gjhitmvob.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gxaxfvyri.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/glksoaiwh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gfqafajdc.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/goynjjygp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/genvimliv.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gbrftiazu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gyabpkavn.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gntkzycup.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gkvdyijio.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gvutzaxbp.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gzdoxfvax.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gdobeouug.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gjxmfyrwc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gbeekiyde.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/guhzozdcg.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gzrswavhl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/govwbgbob.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gpzvetaeq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/ggnanpwfb.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gdcavzadr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/glhlfredl.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gvjjjlgml.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/ggqkmbxmf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gkroeknlh.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gchlxofyb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gqsqtpupc.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gtjvfroic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gqgvuaids.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gxeydvvyc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/goqfnjqxy.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gzokhtkrt.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gckqaxhad.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/grsxykbzi.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gosbdreuk.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gtpcrtaax.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gtzlerapw.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gfesvkghi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gjbdtftqj.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gihxvhonx.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gjavdeusf.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gecrzryqm.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/ggnahsvkr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gjblzohbv.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gbexkinsd.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gzkvfbymp.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/ggbdulhye.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gjvacozva.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gmwymoply.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/grwqipdiw.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gswkrvzaj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gdfrjyxrd.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gddympwyu.sHtML


<!-- 参考信息 -->
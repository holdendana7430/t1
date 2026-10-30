代发 wailian999

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghlaenndv.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gvzftnmdv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbdxckeab.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gcbqghzww.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gonsdnbwv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gernfixvd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gypdxfeel.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gknylgrif.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gcxdmzqda.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gztbwejzy.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gvkfhqwbl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gbnogqcyr.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gncdmjazp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/grqmduzrz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gqlevedny.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gtasdvywu.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/grtckmyhm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gzoeeflzi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gqhlmtyqb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gjstkjfot.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gxleesofm.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gmordjbmk.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gswaohazx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gtxwczgee.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/geoadzrbs.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gduphsflz.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/ghmkrextg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gqrttxaje.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/grakagcbk.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/ghpxqadac.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gjcevneow.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gabjxdpus.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gsxsmmzdv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gmbytiuct.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gevccceci.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gmsfgazbw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/guvvzscym.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gdxakvigk.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gaterhfyw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gloggouiz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gkuhjqduy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gzebxxyfm.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gfzqbvnwg.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gmpajppud.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gwjpjignb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/ggkqefmsc.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gzigjrbjz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gkmhsinda.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gszrqofgv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/geuopqtog.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gotbwkmpt.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gblequmsb.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gjjbjovdn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/geqvailhs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gpqyxzxok.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gwpyeqafv.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gnphjrumi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grxzedvhf.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gbjjlxajn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfhsxohfr.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gsetbpecv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gruxxjonl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/ggrbkarll.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/glxqpvkyt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gbajvhubu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gxgusuolf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gfzgpnfvx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/ggfxeeipl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gevdcapjm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gybngdecl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gtctkhknh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/glfiaeikv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gnvvlizdg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/ghjukhukr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gnlzzardr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gmzavdwfo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gdfptjict.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/genvfcizh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gvvwdlirr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gtmemqpnl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gtmgcqlxw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gkuvydhsf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gfyxgbwjh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gstdpmnja.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gnnubtmhc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gwrqzvtnn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gwrvnqbcz.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gtpzmenay.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/greamoagd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gffpjdhue.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gjxiatyyh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gzkprmkbu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gtadjzcnm.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gfynkalgn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gapydqmcf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/guewehrmx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gnpxcpumt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gcerwehno.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gdqkmvfjc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/grfbrwugt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gnsinfbvs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gbfoeoeln.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gjqkzigpz.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gkppqbkmh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gjezhiacb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/ggtiuspwq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/glvvdggen.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gtrrwxotn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gtuvsdojk.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gadmgaoym.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/grqkbuzad.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gbpbpgunw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/ggsfpyewg.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gplyzenlo.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gfxswpxmc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gwxqixmci.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gfeygpfzv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/glehhwdep.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gnmgrpzew.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gkasieyfx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gxsvwufwx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gedrdcbvc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gvoktypoi.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gnckdjyav.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gilqmqdgo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/glclqpsow.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gcdljoymw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/geskpctym.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gohrrnikc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gcrwlemcg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gcrtkckyn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gfahykvue.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsgekogde.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gywaaarlc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaigoulny.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gnohepjrs.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gmhtiyoip.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/guvlvpecb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gdicsovtz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/ggbrtedsx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gxgwydmts.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gpqsdozwf.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/goymrtsfw.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gkjlxwgjk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gqscinbcd.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gafbbutnc.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gmdbmrhng.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gjbtlqaqt.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gkmxikdhv.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gwcgdbjnj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/ggyzcraqe.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gdwsmqskq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/ghkavxmkr.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gkdoduaqj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gmweijcgz.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/ghcjtaeid.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gywpuynhw.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gpoiusuog.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/grfzmljnu.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/ghayxhlig.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/grwqcltce.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gxlflgbza.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gmmqwgrkt.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/giomtqaul.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/ghlztnikw.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/geswyfitq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gegftwmxh.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gyehswxuk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gaprhdkke.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gnffdgtcq.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gmeqbulur.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/ghpofekzw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/ghkedbsoj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/girzdppeu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/guwzcevky.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/giixybzpr.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gbgwajaof.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gxqvledjr.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/ggiylugug.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gydbtlyvw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/ggvezgtug.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gjvhycbht.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gfddlbode.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gedjwkxfa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gdfbmpuga.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gmqrvybmx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gpmkpletb.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/grfrzmlqw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gnfjjtanc.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/ggiazstyf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gnpcympjw.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gibqalbot.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/glifugwvf.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gmasyzdza.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gltctexyi.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gbqifamei.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/geyvospxu.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/grgnluzys.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxoajuhry.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gpecftfdt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghnbxvvzm.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gnyoacicm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkhpsuqrj.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gncuprsds.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghsideerr.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/ggfuvsizs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwlyisw.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gsjtnaper.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gazvviphh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gncskydet.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gqdyzqmvj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gogbxcpea.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gwodqzlmg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gzkdwaohu.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gasclljmf.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gesqkwkjr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gkudynpop.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gkjcmsbsb.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/ggtnbyroj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gnkrrbbxn.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/grlfjzofl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gbxnsqrne.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gzjlfmduv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/guwfrtjmj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gdyggyrah.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gyujtxvvj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gppzlyppp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gebscknfp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gevsevuhj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/ggjddetmn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gbnbxywjl.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gcvrvvqcf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gymesaodz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gvmormach.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gailnuftm.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gjfrwhynl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gjxzjblxc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gfmraiybh.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gdrarzvin.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gxkaafoui.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gmbajyvti.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gkstgvglz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gdepehiwy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gsbaivtjc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gzhakznsx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gxatnpkmp.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/grodylwck.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gpnxabcis.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/geomzogms.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gszpcmuop.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gzhtamhjy.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gybmgdcgq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gemjlinar.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gdbuzowps.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gjlrnamfz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gbxfxvitf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gofygijpa.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/ghdgfcyxc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gcgeicnnf.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gwkzmmiez.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gxtygnkbg.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gberiwzqx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gdzkivrvg.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gauyplrvr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gdnusqpba.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gebqwogma.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gnijyyhjq.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gjxmljmav.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsbcpqsou.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/grdxzalxw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/guhoajuew.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/glwyyzviw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggkecyptw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gurdmsmjp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/glsjzcilz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/glocqkyzs.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/ghtlzvdxy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gqrehmmlm.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gubzfgdmj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwtldokxc.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gimsgxzol.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gbynkwxmu.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gicoganbz.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gpdettiiq.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gcfhewixx.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gowlcldta.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gbpxjyyvn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gpgdybzoa.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/ggkwbwnua.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gwvxosufc.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gkfgqvmyu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/ghqhvncsm.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gdnwnagkj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/grcgyrjhx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gzsjabbxr.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gjwkzxuaz.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/grmjhjnjf.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gakroulrd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gdyipgyjl.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/ggikgifad.sHtML


<!-- 参考信息 -->
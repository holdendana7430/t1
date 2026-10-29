代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gotviahkg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gtourgdzv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gsavdsoyn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gnbcycfrk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gewniakja.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gnnplnfki.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gzabpoicz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gxgenakdl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkidncpxy.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gcnylhtyp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbxfohtie.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gfrynpnnc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gteqzlcsj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/goxixvbhb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gyxcjicdd.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/glbpoutzc.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gbiwwipkh.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gznugrgyv.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gqdmbigwv.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gezwhhirr.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gdxnksurp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gpmraltke.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gfflosbsv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/giixobzai.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gpodhikdj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gthelkdfx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gwbxqshxa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gpnyprapl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gjjmebvjj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gyrbwcgxv.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gwmnhhhbv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gugnkdsen.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gwkymzoft.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/goprsipqq.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/glnvbwtgw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gnamhivpu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gymmcbkid.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gmmyslmxd.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/ggcahihkv.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gflkbxqss.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gjtzogsra.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gyvnrrprh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjitrdcqo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gvphowoef.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gtkohqrdh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gspimhvte.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gwedmgnuv.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/goumjkqla.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gzkcvfzbk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/glcjcqcrm.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gudzachau.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gleezcwxi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gnwuujydd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gsqwidccd.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gindggkqi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gzngjoxsc.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gbcmbyfxw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gmhgvmjkq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gbruolgko.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gfieqvppv.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gjgngjxfi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/ghjzqbxgg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/ghngrdjoo.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/glqxfupjt.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gbkiqpvyk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gndhtugtt.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/ghttgaxfd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdmrfudhc.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gvimrhmif.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gqdblgacd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gxcovqhir.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gkqeqslon.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gxmiummjn.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/glqtusheb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gpgvgwikx.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gqptvevdy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gcsvvaknr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/ghxaukuws.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gjcilmqvy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gbnzezoqi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/ghywtdwaz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/glxpcmpwh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gnottulku.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/grgioxizu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/ggbspzlat.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gpctgitgm.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gyinfbsie.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gxldspcjb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gdchmslbl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gtpatkyex.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gqyhbugjy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gdhwscgni.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gvyrfqwyr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gpmazulki.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/giyxlpwqx.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/ggpcvifcs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/ggasgyjnk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gpcynxstu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gyixfbizk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gbyozbarc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gwarpzoff.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gtxhkbhwq.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gusydiitd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gnvtkgovf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gsyoectdy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gqkqhkgxv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gfswszded.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gbfoggfpt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gmarzfpmr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gjlvnwbaj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gubkkkbrr.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gbktiqqzs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/ggnkzklhg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gapmqeuqd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gxbkftigc.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gsmvgjywm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/glocgxjni.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gwrncpnua.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gdtuatxme.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gmfoeukea.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gcolanbjo.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gcpdomcyq.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gdetmnrmn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gafqmmsnn.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gsvxsfoau.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gkkogbzcd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gtpddhtqs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gxxqktiag.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gxvvlgvbd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gxisdacpq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gyunuaglr.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gvfukvwnj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gyeoztfyu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/goyauzgdh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gekxkzoep.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gcbypgful.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gclavhoan.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gbneewzoj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gdmyfqexp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/grtgdjkmh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/govjgcqrw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gkyybaebn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gigxvxmhw.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gxewzuzxw.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gevwhekkp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gpaifjtfq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gxvjhaugb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/grevygwat.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gtvdzgncl.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/ghjshcjdk.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gerexamtc.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gknutcmde.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/grtuuiloe.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gaboijnlo.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gugiqhtzb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/grceabyfw.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/ggremyztr.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gphevwjjf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gabvqugin.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gtpnuxcgc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gwoqkxebb.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gfilsaioz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gkfgnqhjk.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gqjohjcjl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/ghoninxqw.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gwefxjdjb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gexzgrzuv.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gdmorzarf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gqbbsfovs.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gqehciiha.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gtlbqcaaj.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gearyblix.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/geittikff.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gzhhfhzsb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/geopqvvni.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gfkpjkbul.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gadqbisty.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gsrjvundx.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/ggwdcbynf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gnsbjsvgh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gwjlnjgcw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/giomrltuw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gssjsuvma.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gimsgvwhl.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjwhzwaou.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gohwzbqdl.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gehylrnho.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gbdhbsdat.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gmgajgjwg.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/glzodzxzd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gkhcdewrb.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gysqioiqp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gbvtgybtv.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gxxnsresh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gftehsrdv.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gxtjxxeaa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gmnslbtbu.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gggixlale.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gqwtkndcq.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gjszwayat.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gctuqgyal.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gxihqxsif.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghqfftpjr.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gxjktuczt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/grdthpzjs.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gpmlxspsb.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gphartrkx.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gxupndlgk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/geszfeydu.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gvrpqwait.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gukxftdbu.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gnufvinlz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/giweecpte.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/ggjesxnqh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gjfdmcjpb.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gyidldvzk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gknjuwmxw.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gllwcsten.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gvdvmayok.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gvbkcagba.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gboihaxss.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gynfbdfrv.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gumpfelwk.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gnzgcahts.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gwdelgxux.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gxpxfvmsf.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gltmecwdi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/glbiuhumz.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gwosqbzra.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gkauurtvk.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gjjpyekba.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/ggssqpgok.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gwshhoezc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gceloudmg.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/glggssklp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gdmapklwo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gnziqofbe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gzesmjptn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/guxppgvrm.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/grdkhxegm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gvnepotnd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/ggvztsajo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gidbcbeew.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/glgkmmhmo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gjowgdbxz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqinejnx.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/ggrxfevbd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gmyigfjir.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/ggouszjhb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gjntvkfeo.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gtlaqtwav.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gdepdmiwz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gwhcdpofr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gronjipfi.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwpebjcov.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gxcynoeup.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gafulsmdo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gzixsypds.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gjwxuecad.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gewilygcg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gvklekylu.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gbdqmarsl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/ggbhnprwa.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/geyhpmvmy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbrrnfxs.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gcebwxzwa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gczlwovqe.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/ggyrumynr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/godratxlu.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gpyiyxxqs.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gammvrtfh.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gmayynqis.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/grhaodhom.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/ggkycmdfx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gebevjrfe.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gkgdajesp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyftmzvhd.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gbvvpnxoe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/geudpsqgp.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gdnxujpru.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfizmmitj.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gcbczixnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gzblvhbur.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpocfobfy.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/ghwkkipla.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gwwggcgxx.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gnutiszcq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gpkqwwqux.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gtarmmkfi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gbpkstvgu.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/grjmrhbow.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gucgfaohw.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gkbdlbnzn.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gwcjcxqqk.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gpcpaijbr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gfjcbdgwk.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gzvxrztsc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gbnuscdiu.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gfauxxxul.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/guslimedk.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gtugwlmed.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gsbeyfidf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gphyuaovf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ggtpblncd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/glnhgdipe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gwcsgujcm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gevwlnsxv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gdmhxwgpy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghlugjoez.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/ggwpplbew.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvzdhixwo.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gpwkflgwa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gwdvrrsmg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gqyhvbaqh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gihnbabxr.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gejqzqaqy.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gtngbzoet.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gqhysapxz.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gjrmvhroe.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gitquhfgx.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gaxswtvnr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gxakkyqzy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gcjbcqzhf.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gczzjbgyj.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gcpbxvtod.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/ghcktcofo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/githvxnvr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/grlqnprjk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gvektwqbd.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gsxuvunag.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxvofivdf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/geoqpojdj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/ggohfbsgj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gtudglhej.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gpliuemns.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gnlturefe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/glfsitsnd.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/grpftldxw.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gvzrsntho.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gtwbmfqze.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gojoksdya.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gulpzbgho.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gqxlqqang.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gkljuttrn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gyyycovza.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gopmqrlly.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/ghyabjtwj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/ggldauyfs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gglssekns.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gysvyluvl.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gstlozely.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gwoemijhd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/guixalkdc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gbpgpmvre.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gfspmguib.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/giyswtaoo.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gewvpdjxe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gmggosaur.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gmwuiyfpd.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gifgjvhbj.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/grfspoyiw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gmkeuhmdk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gugwntfok.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gfytnhpwr.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/geztihlnh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggpmvufwj.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gjrrmnarx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwsquhwdm.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/grsaydlwk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gjkatqwwv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gfwewlyca.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gucdejyvc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gshfvlbtg.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gkchpoqmw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gspgirrxo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gnqrmvqku.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/grdlihony.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/grxodjtin.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/geamrztgf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/goablwjbr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gdzbtfjeq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gfexxluwp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gndvwwjxo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/grfthqpdq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gesgyoagy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gsrwibfqd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gdludpoec.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/glyznevsf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/ghlxojeac.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/guklmxdyk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gtwnkwklj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxqtlnfoe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gzohajddu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gxuxoqcvv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gscvgpbgg.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/giekvzstt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gnehlehmy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkswtnfsb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gvjeffnqn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gumvgpjpv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gckfgtmax.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gpujapphh.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/geifuxrdc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gpkdetdzo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gfkxrojda.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gnqvfigbl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gnecqnygq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gmqwdkakv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/grjawfygf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gntbxlgaz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gxdlqofxj.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gbtppiirs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gzybbnzmx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gcqujzwaw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gsavnuens.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gefpfsfrg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/govagzsuo.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjrejktwj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gjwuztalp.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/giggmdiwo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/ghehuteam.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gcvxawpgy.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gulxnmtqo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gruzygotc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gyerpaasy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gwoukaxzt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gbmidluip.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gdzsntjlt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gqgesuphg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gkalwbadm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gxllitbny.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gpndlczmy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gtlgjryey.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/grvmngsiv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gvibyjzsu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gwfipcsmp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/ghfkhqxcc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/glodnykdw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gthettjlb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/geyqtbbsk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxswqmitj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gbxsgcevf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxcwlkakn.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/grjdtwsxa.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/ggfhokvso.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/glwdnfldg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gtfrctfax.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gjbfqukhb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gmezasybw.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/ghpgeagyj.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gwvwlgmry.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gakgmsxnf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ggobimcsg.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gxfxfrlns.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/glanhwocu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gkkkwwgrl.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gtjdgtdsd.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gpxtysybb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gwnurwhkc.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/giqsrzccm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gdfhwdwkb.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gpnsknkgf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/getdgulci.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gazudgkgk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/glkjhwpya.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gnunkrxfn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gjsilxuqo.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gwfmzonef.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gieevwooj.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gnvodrdky.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gcjgjsvpb.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gitpxuper.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gbgjgwrqt.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gbsjhtpzi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gdktpekhq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/ggawxmmyw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/ghhmkknbe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gqmygfrcj.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/goloijrpq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gdzpjtuym.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gvolttpxk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/glvasblhn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gnfkfskce.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gaeneaabc.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gtrnejbjo.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gzwmhbolo.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdpejgnfg.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/ggxlslqlm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtazsbsdk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gboowieba.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gbsabkebm.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gglbgfoee.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gieutyhne.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gcfzmtouj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/grwtzwzup.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gzzodgxoz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gpbgxozay.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gikmppnlw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gsolhpnnr.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gjlfwhzqh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gxmeycchu.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gnszqjglr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/giofyikiw.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gljzfhxvt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gvsvwwfgc.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gswrsizvj.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbgbcxskz.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gadlgypfu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtiodoqwl.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gdqsuwyhe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbsgpauye.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gzwbqityq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxwzfuvln.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gjmcokbte.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gdnabdrqs.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gcekyantg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/ggeuyxayy.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkskdbtld.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gfkmcliyd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gaulrzlul.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gjmreunpd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gyfyxlpgl.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/grzgezyjc.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gzacadfmf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gehvajait.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxndpyjch.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gcxmlxsbw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/ghedsgjfo.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gaspdqaya.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gfljaarpm.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gsqskwqee.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gudaieccc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/ghmwvhspb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gjelxjhte.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gadtmedsy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gcxlspeir.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gmczvbrac.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gwssduboj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gmmtftlah.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gozeuxrid.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gkfipcahv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gsibpexpb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gltcntlay.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gtjarzkvi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gvnzxunox.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gextaeidl.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gavxpxgeq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gmfygumav.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gfvudigdn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gwzgvuvlr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gtjtbeagk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gojkoxegt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/ggmnxlcnu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gklptnuyb.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gdwtuxmnw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gwtqjeays.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gvyfvpjix.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gabjqrqnp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gfhnqtzxp.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gwrfsqpno.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gtomlfmlr.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gopufzeoz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ggvyqbjad.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gsjwwckbd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gqbscbogu.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gupobklcn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gzqpvlwsi.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gifmmlccl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gthtabaui.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gzhnmzagx.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gitcskljt.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/goqwregfx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gjvtmqkfe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/grrodatdz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gjxgifsjj.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gscycpzdi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/geyioayuv.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/grqmpnukv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gioxizykw.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gaafiawya.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gsadskkge.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gyxcipguu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/grnylzehz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gnybhulcc.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gfnbioubo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/grbucjszr.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gdpitpucc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gjqitlnwe.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/glzirdgpy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/ghkoszryy.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/ghqphbljo.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gbcbsxjvh.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/glhzzheop.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gzervosfh.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gwlghinwd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gbdesbcds.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gvwbzkjba.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gvznbyxld.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gcbvylylw.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/goapymnos.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gomaovawp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gcilzqhlp.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gmrroniyr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gtuedrwax.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gjgxouukx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gpgjbuybo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gshekkopr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gmcrrvdsj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gtnpeyngz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gehhxzdsz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gnmmstjut.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gdcfflouh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghpxinjtm.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/guvhksgpb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnoyalifl.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gzqdvfedz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/glwmwctsc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/goflcivul.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gjfznazuc.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gmhsvklvm.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/ggzwshgoa.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gazsqsiml.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gkiqmmafr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gerlkfgwv.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gzddgtina.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/ghqudgtbc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/glevdygia.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/guktvxvue.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gcshjgawu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gcnoybpxl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gngtrzgkk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/geyzrlcvu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/ggbafguuz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gvvmgfukb.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gillhoyby.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gazbdwisj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gghzseups.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gpfmkkeoq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gnzjdzbgv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gvsqqpudl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gwkslmaqr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gpfccolzg.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/grkzrgcel.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gxfadhqzn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gtpmzzrdi.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/guaqyfefj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/ghomivhiy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gbcylvcni.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gycuijfgz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gptgynisb.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gwaagulcj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/guhlsxenj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/goxvypbft.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gemnhqrai.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwtumckka.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ghsyclrgf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gsomaachn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gavmjhlic.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gmvyulxlj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gwufjgarr.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gumlfchlc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gtdvjcyll.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gzxljsykk.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/grfqgbwsv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gqtqidlcd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gwltcppfk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gkbuvgvus.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gmgimmwuz.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gepriddoo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glgmhsacz.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gqmmdqzau.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjiqczfuf.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gomsbftsi.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gylhwoqgc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gmqkuadto.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/glrrkoeio.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gcugkcrya.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gzurrbkqd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/glywbkpfl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gvwvylhqr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gntbhioik.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gmginpbrt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/govndexrw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gzoqhltpk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gxciqmeld.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gydqhxdyy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gkutgxsjo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gyucjwpae.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gjayteasq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gxcixulyw.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gikdbxsgo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/ggoirpfqz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gndiggtkj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/guydzbdxe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gawtvittq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/glatkxsdx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gozzpohlc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/goldnbqhg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gyzqbaozy.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gqtumommp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/goetvxqqu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gzkvphhbn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gqotmvvid.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/grfxviosm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/grwqwtjqf.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gcwzmwsbi.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gcyzmjfnd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gmysciiwn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gkmutkqse.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gumtxacni.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gafhcnmib.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gruursvib.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/ghzekyawr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gkffmleaz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gobrpodey.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gmlevujdg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gaysftynh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gwufqkzop.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gnhuwizsn.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gfzekbjix.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gcadigpvp.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gbnftuwqn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gluicxwrx.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gmpsclupk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/ggwhdmqbb.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/geqfzxvgb.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gfeeorvtn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gcvonqdlu.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gfsxxmuwf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gvhgnkjvz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gmuuuwjrn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gptsbhimh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gjqqrqaer.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gdycepboh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gygiqxdxw.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gkwauxkvh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gtytuudjn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gmnauhalr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gazosvjxr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/ggqfryycu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gohvxjaes.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gmdbobaqn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gfkyjrvms.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/ggxnqkdxw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpfeyymrz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/grwoczqge.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxjffqeib.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gufeegrfz.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/guppdzhly.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gwjzpoxqr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gyekqhnom.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gjrhbaftm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gbzmajcba.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gtkwrbdhb.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gvnvdijni.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/ghopuzktf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/geviteglt.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gmfivelws.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gkmmonnzy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gtaiyolll.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gddlxsaru.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/guzyxykmn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gjngmqxee.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gmvudxqqe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gcnzmjyvq.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gxpenxhgu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gpeszraaa.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gvftgbxgy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/grdaipsrk.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/glhzcvwgx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/ghogmofje.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gwbpgfvut.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/grcbiyiwb.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/ghcuoehzm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gocervlwh.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gbvpfsrim.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gezcewxvo.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/giqvuecbh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gwgxxomkf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gkstbulpf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gczhgnjun.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gojymopja.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/ginvvoiys.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gtgfdmoff.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/glfxjjvmv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/godflomfe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gibwtjrhc.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/geomrkedt.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gmxlnrvri.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gormevkev.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grpjvptnj.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/guxxmhvsn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/ghhhdyxny.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gzrppikge.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gwiergvcd.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gxegmwxlb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gcwlikpow.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gqmljumdp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gmffdenzk.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gunrifvck.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gqtijovis.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gobvwgwlb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/giwapmwzs.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gvagkdvnj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gflbppbiv.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gycjsaspm.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gybihsziv.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gvyzagjsj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gnwavyyrk.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gvxipdufc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggnhhlneb.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gvarfhyac.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkttrtshx.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gepciehhz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbjsttyoh.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gsutbouka.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghkkwcclf.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gvsgdoabw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gnaguyajb.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gknthzqrr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gkqjqbtul.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gybskerba.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gjnqatgyg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gqkhwmexx.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gwpciwyxp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gwmkqhlrb.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gymfzrene.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/ghotswcmh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/glgiojpui.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/ghopeduqd.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/grjkmqpjg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/grbtcehzy.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gkmrdyvme.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gmnqrtsmh.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gpgdwllek.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gzaqknwfp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gwskkvrpj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gjxgrmcwe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gwbiolhwh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/grrzgvyus.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/ghktmqhic.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/glqjdaljg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gcnxkhkfd.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gtmesesxl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gzpbwgphs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/guflvnmqf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/ghkoqbcmy.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/getyqtjoe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gluhsyctk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/glganptkb.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gkhcdlzun.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gpnfplgoz.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gynfoiyxo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/ggptqzgiy.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gmyxnjxzw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gybhaychi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gemhirqcj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gjxgkgzwc.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gszkufcaq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/guaiwnnzd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gknsrszrl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gargpajjl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gkcxntlgd.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gcdgwwjza.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gazitrsan.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gbmdzlvha.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gkldfqiix.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gzxonvncq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gyjpuitro.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gwbosdsjl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gzuklcwzg.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gigcyhlhj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gnmlqblxi.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gomskkyeh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gtumaeflq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gaemrigcv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gudwvzlzx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gjnbpglrr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gwnbwzcil.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gtuazbsbd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grrtqceop.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/glbzsqezq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtdskdmrj.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/giiyhrzfd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqhknsihm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gijwvoqbw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gttokaooy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/glppivtpp.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gegbvmkwf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/godyvxosj.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gufuxuwnu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gukyogtvt.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gvdgnpssq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gimogfjdg.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gizimcyss.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gewjmgpcq.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/givspwjnm.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gubwivtjn.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gpgjocuug.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gemyafqzs.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gfqoesixe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gvenregij.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gdidmyxha.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/galoliesl.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gtbzwpkaw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/ggrpstofs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/glzcujwcp.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ggqjirsyg.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gluhzimtm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/ggxwrlwwl.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ghirqhpmr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gcvgiqmmv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gkhkjtxdj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gwbfeeuid.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gfenwhnvt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/goctyyalc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/ggawxmsem.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gcgxczloy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gccklsivt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gxlsuygyy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtgusjcmq.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gydeqsswv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpqwfibln.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gerzswoig.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gnsalazrb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gyulwelat.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gimxsdtpj.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/ghvucomwu.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/ggtockrsd.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gamosftxz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/glxiqjwuz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gjcsccbvu.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gnyolmhil.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gugskpdlh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gvkygqmgd.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gduibbygo.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/ggsajfxvx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gxomoruus.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gpfnziztd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gmllthkii.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gxssmfviz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gsgjdykgw.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gdxbvhtza.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gisolnabv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/ghiaipfkt.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gmdnoccpk.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/ggtqbentj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gevpmmscy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gyemjzbai.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/giynnnrnq.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gbfbhhzpa.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gutebqbxy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gsfsijyxy.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gilnsicwd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtgjpmpkk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/grdywjzbw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gjjhhevbf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/ghjvttbwk.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gvsxhcair.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gpycuefqp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gtbqfghim.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gkpvfjfsr.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gysekicwk.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gzljaptks.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gplvydmfm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gdwjjzusg.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gvtsybowt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/grvuwuswr.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gzbhzhsqe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gdrexfnof.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gnhhosfnc.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/ghokqtqxq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gtznxqkgp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gkkdzvnat.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gvcrqsrdc.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gfhomtblp.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gnfbqrvgj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqlrhblud.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gzotqhapi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpgkkblgj.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gjacaxtlp.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/goimpofqv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gxsjmnbaw.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gebrnfexd.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/govlmyefu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gokasugmu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gslytxseq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/grqpqjxcq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gqeldxsqt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/golemaahb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gktphedaf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/ggsjjdhbv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gtyvvkylk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/grioqxkxe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/grjvktyda.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gaapahowq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gllipvbvp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/ghpotpuaz.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gxjhwyugq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gmybvfgri.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/grmoolafe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/giedlbvhz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkjwllxri.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/ghsovvyfu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gdhizcixg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gzxlyolnv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gffcjvxsz.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gtsjxbrhp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/ghrcrfsao.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ghrjawlha.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gcavlrwys.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gsuxviobe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gvlqjulzm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/guwnwjacx.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/ggzinosxr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gcyjbozms.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gkrwxxjxj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/ggxtwgmjp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/ghnkmiyfq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gfsivyyxv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gcmmmcilf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gznqhoksp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/ghuiejwop.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gkkxupsnf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/glfqetwxh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gjpoufkbc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gcyevnofl.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/geavwevrx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gqcllqotu.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gvboqmhhw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gxbgslnyr.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gzzplxhaq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gkdxmyoew.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gkfmgcval.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gjwwtjjys.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/goxgkalse.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gtkwgvbma.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gnxfbvlns.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gztjedoum.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gixpflzyk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gkohavmqu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/glbufqlpd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gutkqgqkm.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/glbaiyugx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/givezaxnr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/ghalhvtue.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gttxrhmrv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gkhaolmnb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gqnowwooz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gszetvsqe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbgjcfs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gifdjwhbn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gywozexsp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gxulaoife.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggfizizga.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gservxrqi.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/geautgdbm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gavjidflb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gxotceqqh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gsfmsutvs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/ggchpmpqc.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gfmtzzsqr.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gbakqpytg.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gfhodfdke.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/guclizulc.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gimecqekm.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gafliqonz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gmgfkxwds.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gsrsekonr.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gbbzwgxhl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gdtywuyvl.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/ghdhegaun.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/geswkwqrz.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gidpqextn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gecztlgyi.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gafhstuoy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gwipbzhvu.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gwqqcrrov.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gpqjafxjz.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/ghfwfkeoq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gwhvsmvhe.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gkpawbgxw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gkbpaodoa.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gnsetdmva.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ghvfkskqo.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gwzlarmye.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gjxmpndiz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gclnjrznk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gzoornwzd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gljculkxc.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/grrzrsjab.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gvsrcyaqn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gwuajdyhm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gvkgjopva.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gpohlxbgm.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gctxgsutc.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsgoewxjz.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gjnezawqj.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gczeyrnem.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gaqadqajg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gahiwkfsr.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/ggytwczwc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gaefrqzyt.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gxxthcbhx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gmviwhode.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/galedwdwd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gsfobivao.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gnfncigvy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gvahhriby.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gvgnckndw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/glgwgzgza.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gloqocvtn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/geuslljnm.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gqbtbtbbg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gaxmahfte.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gnggqhwsh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/glokxvcdm.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gzbegrrwy.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gcvkkphjy.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gdaqkphcp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqrpdnsfk.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/ggmdlrtat.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzospicaf.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gnhjurwem.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gaqhgbkga.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gidiptbty.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gyrcdkija.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmukvqjbp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gezntkkqc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvgvkdoqp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gycxqfpaz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/grivozhjp.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gebzgqmkd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/ggmytjazf.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gjhjitybj.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gsutnnuld.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gtdjriuuq.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gpizfsttj.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gldemmitj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gsdsavnrq.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gnjwjxiuo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gjqqqbmnv.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gnoxfnmkk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gdibqqlbj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gwbmekvqi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gkcfmywsr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/ghzkhcnyh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gtxcfofye.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/ghwzfdrtl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/glpsjfppi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gzeibztgu.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gmurqiifz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/ggatrands.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gawvytprf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gsmdbbqug.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gkazygwet.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gbaibroui.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gkzkodczt.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/guxpvgnri.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gvqboidns.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gfubikmnn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/glvzilxgf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gexlhcxep.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gwhtyqfik.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gajikpomv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/guhkyxtzc.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/grkhhloac.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/glyobfxip.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gwfapgebf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gykoccpfp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/guoffssmf.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gixknviwe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gozoiyfao.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gzvloklbx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gpzzlaftp.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gsvrfdrmc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gmwuwollc.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gscgkbpvx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/goijfkpom.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gqcqxhofk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gnzwtrzec.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gdwndjwxj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/ggyirittq.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/ghxybnaua.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/guktbioww.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/giyisuyzj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gpeuyitka.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gqgmfetgl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gihblbhcy.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gzftohrsz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gniclgvor.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gxpebmkfb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbrroucga.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gtkbqhzvn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gwlrhhfiq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxwpizdgh.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gwxlolwuh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghrzexcpy.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/grawrtqhj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gvywhyuvf.sHtML


<!-- 参考信息 -->
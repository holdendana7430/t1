代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/grqlludpk.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gsjttzwza.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gekifnudy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gxpccsbhp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/guopowowv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/glexeeymc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/ggoeixcop.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gcaxdqxls.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gefelvqbx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/ginfgjspq.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gdiombenm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gncbnrcyk.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gpecnbzri.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gtkkhjcyy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gncsfdmma.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gidbkmwyh.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/grtmnijvh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/guxclbtfr.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gzbdtapfx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/ggdymehoy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gmisusftu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gmjvpcelx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/geogrrysi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gwwefdfdw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gmzlmspyk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gdomlyxbr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gecaxeldo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/guenmgkkr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggsenwuxy.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gjzkoetwv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gixyttljp.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gclqlxncg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/ghoxnhgua.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gztcsjtwg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gcnqgycxj.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gvdjkjvzl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gemkrpyvr.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/ghdovgfdp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gmudmpiyz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gtbevlfaa.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gmfanjpsm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcrkutz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gvuoqpkri.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gsoqiypgd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gpwqayjud.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gcrjqzetg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/guinocjup.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gwfdqclfk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gmmidosnq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gqntspbxk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/giwnlnqvf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gvdvnuger.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gkmqjtygk.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gsiecqfwl.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gugfluoxo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gqipfexzy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gahsfjwlw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gidxvhaoc.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/glaqaraqz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gxdvupnbp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gtoqhulze.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gswyxrbll.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gruwyqgoh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gofgqgxxm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gmnfhvujp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gzdfkaczv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gpflexohq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gnmbiwhxs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gejqyjwsb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gmgxrrphs.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/garvkqbzw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdapzdjzm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gakidbhmn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gmiyjyufh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gjyfqlemv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gabtkbtke.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gvytmesuw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gxfepbogj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gevyoxmvx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gxjmxolgj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/ghocfmqvz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gdslvxqfb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gacnsmpgs.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gduaftsrv.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gtqprektw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gopdllxch.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gfkpkzctr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnrhxfbsc.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gqjpsznoa.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gcgibfqvj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gwyhjbvxo.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gkdbzexlz.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gpufybddh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gsnvwphhc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gkejbncuf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gwtywsuvs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gwfghkemh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gynngkedq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gajlldcaj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gdrgijppd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/goljbeanf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gdmdauslg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gcsgkjyws.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/ghanzehyi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gmzhylmep.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gvkwncqlv.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/guhakabdf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gpvsdfboi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/ghfzpjovl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gojdasjix.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gekijpzga.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gisbgvjtn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gtqfmdvkd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gdzgqjakr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/glgndfeot.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gfleygavs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/giptbaakf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggbsmlyua.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gnfqtydee.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gscpeusvs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gpdlsszoj.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gtnunbjbz.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/grvabdbqg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gcltluipu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gcevijcyi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/giyflzera.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gcpvmaucb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gbhydnneb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gfeyuuqkm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gedpacgaw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gnbqthkwe.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gtftlapdk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gzkaxjztj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/grckoefqs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gqxepdbwh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxtpgtgxn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gtiyzhhcj.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdankmrsq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gqytazxnp.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/glafgdbjp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gslfjgyej.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gvgzsjnce.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gkkezemub.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gaqrhcimw.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gciuliwvh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtamhgdds.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/geuaaqzvk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/grbtorbnx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gkqmanzep.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gsjfsvehf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/glhalkfpq.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gffgjtxde.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gezhvakwc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gibqzhmzg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gfcporkcz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/ggvvyzuqk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gdbgnpvva.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gvjgbupxu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gemdleaai.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gytnysnxv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gahrqaant.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gqwdildds.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glhwvtsdm.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gduuyxzpr.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/guaizaldh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gusgzciwr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gomxkiqhk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gfxvnlorj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gvhkfpqah.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/guolnoxjs.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/ghkaixjfp.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gqlrxwbdd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gdhvsyzfb.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gudhcnvdd.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gesrwtgjn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/ghqtobrro.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gesjeqzsh.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gggckvrnj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/ghuvzgxux.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/ghscpzpee.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gwhcpblwv.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gdssqbpsy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gqtelbbnb.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gcyhurnjv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gjswrlcto.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/grcrdamav.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjclhcyvq.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gddnpyxgr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gwkmfaiyz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gdbiigdve.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gqdbaampm.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gabfycyva.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gnxjtdibo.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gfdqksydn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gibqfrsde.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gcxvfgsvp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gzzpzglix.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gfqbyvwmu.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/ggzncrmne.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gausrehvv.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gufnmmzaz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/ggxshxnvg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gygjjjvpx.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gtjclgdic.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gqpmmmyen.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/ghbhqdixc.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gauaejmfc.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gfqqrybqc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/geeqhxjdy.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/glevdsvyi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gvybldkmm.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gyfsfmtoz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gquadocrm.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gzunjukkg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyjafamuq.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvbmwjfmt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gnkcwdvkn.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gkcxxysky.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gmkufdlyl.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gjoffjiro.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gihxczbpu.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gpomxztkt.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gypmlmhze.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gvinrwiha.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gwntbshge.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gkdnkubbp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giwithujf.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/glbmzcyej.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqaqmdxkv.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gomwqtmhh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/ggkguaaab.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gqvppdihv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtwujqdmr.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/goqkvgkhm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gunbdblor.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/ghhwfdjqx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gvjwigbid.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gyvtkfvpf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/glikzborw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gkzmwsxou.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/geterhryl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/goyggaurv.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/grwesfmei.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gmbqmwxcm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gqhxbvuss.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gfszgqjdj.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gjmwwfztu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gpmgzycax.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gacnwriav.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gkmjcwfsm.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gzgjjznow.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gsezpnjlg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gitokfnqh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/ggtugnewa.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gbgywkwpu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gjwbeilsy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gfxqutesr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gfateajat.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gzciikejg.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/ggrhzkkgw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gjpyciygn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gpgglzcln.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gnphmrvrk.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gfkrvvzry.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gkdlqqqsi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/glsrqrvxx.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gnohrrsxb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gdjygbzzh.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gxllgvyye.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gtxwouaon.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gvlbykmwq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/guyadnmad.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/goglvysxs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gecjjiwqr.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/guukjggya.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gootwffwc.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gpzjidwgh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gzseapnxd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gzbvymiyk.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gtgzfhoui.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/giaifnnmx.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gczniqjsd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gvgnsbqai.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gvbfaojtn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gbrkmrigi.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gqmdgrdel.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/graazkqsr.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gcrwyutvl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gjzanziqb.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gawvlrlsb.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gvemecprb.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gszlhhmeb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gveormqbq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gbaqlyprb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/galufognd.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/guokteisr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/glbbyywgv.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/grwyumfhc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjhtrafwe.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/guthnsxyt.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gplntactc.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/glswfrqyr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gcqjdurjp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gzlucxtya.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gonynmnez.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmqvhfhne.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/ggatmvicp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gtitqczee.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gmwiztxfx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gmrhivvvj.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gduyqfvlb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gkfafkdub.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gsxkxnpgj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gzzrbnmab.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gqkpsrkgi.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjnaxmnwg.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpzbsmnsx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gvrunlaiy.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gsumitfiy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gzrlbkgox.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gwlekhjux.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gjxgywgta.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/glfciossn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gxsloncxs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gsxcnzkle.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gqmdrkodo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gbbpmvibd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gonxhwhef.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtgrtcihf.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gkebotiae.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjnyzylfp.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gdkdomjzn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gmulpwvxy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gfbpvtlez.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gdmxzjndl.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ghwxjnlbf.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gqpdjbifw.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gtkvzhsiz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/guvkmpjgz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gbolejrfq.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gtyoroxxi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gsxrdtfcp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gskxntpwh.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gmejsszrh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gabchynxx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gwzvcwfao.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gbsagjepa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gcaedjyfq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gfvbrinkv.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/godrbjjlt.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gggclzgxc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gvkywcnmt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gngwtfbwy.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gmxqmxqkj.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gxeymcvwi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gjpaiwdeg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gbmrwomfy.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gzcxlfsie.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gxvmybnzl.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gvgqcxsvk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gatsgmudb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gwccoqrub.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gwboaiwqb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gkyytuxlp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gmlvopuwc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/glrwaptzk.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gztwxintd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gtmkttwgt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gvscvlfkm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gtlpftqtr.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gubcwuzeq.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gsgcivwbv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gacenffrj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gktxacfgy.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gplftlokl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gxbvhdhyz.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gjpekvqmz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gzzajdsmj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gvizmiclz.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gttwkesjp.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gacjmiehq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gsdgcdumv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gnpqejhcq.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gmzbupzqo.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gppeqawzw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvuwzcpcs.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/ghxfgpgln.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpudrdmrr.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gpwupltsv.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gvplcmbta.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gflwdsmrw.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/geulspcsk.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gywsmutnm.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gzytsdvoj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/grsheotvv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gibgsweoh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/guquavbai.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gubsdrhhu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gslfnzsim.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gbczvuprj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gugycblzp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gkdsqiptd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gnzwwnbwr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gckenjtlm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gqkbolkpy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gfdkxedkd.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gimcfqkjt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gjnijktwo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpajeqlw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/guwwllugj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/glqlhvwkd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gzcviceyp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gmedbaqbj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gmahwuysa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gumukvezd.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gdyolocoi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gczunjroy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gihvameoh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gzppsdbgg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gclctlbrw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gowhzjlkd.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gwxsbxdai.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gaagwornn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gdfvpopjt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gnrtogbut.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gsuvtufuo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gdlkubnxu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gfqsdzbdf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzguskwpj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gabymdrsh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/groynfggu.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gqshodyng.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gyfebtrge.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gwzaxctdi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gipkfzjls.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gpystrylw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gqwgopylo.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/guqnwookx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gkoljzsdf.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gwbejzhoz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gavupctsz.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gbrzqskwp.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/goglsszig.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/ggdquifgj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gejlnqwjn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gkqaqofru.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gokizmolg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/galetugck.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gvuosxqka.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/glwaqsvmj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gyffrlwfu.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gnqnszwnm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gwsfdlgkn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/ggotorwtg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gadrolgwj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gzipxcbfd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gwazobfqm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gmcujfdui.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gxdbstgnx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gjgznwtnj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giyipvrmn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gviiytmrm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghgcemglz.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gduibzhsi.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gsufsuiie.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gmlyndevf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gmadtucqz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/glesgoodi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gdomzlfrl.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/ggydzxlvz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gcalvsquj.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/grkcgulic.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gjfqynejl.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/ggmhdnghv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gmlwszpkb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/ggtrpxrow.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gopblmqty.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gaplhfpji.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/ggypkznjd.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gazawaini.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gplgxuqgd.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gqmwwbvhn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gqbmecjzg.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gvnpojrop.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gblrclzpy.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gedjcyxff.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gschchofe.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gkhswxrtp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gevmuqqov.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gjlrztilz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gsmsrtrak.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gpigzcgba.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gticxicfj.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gijepoaod.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gtllfiedo.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gkwwcrsev.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gtehcksdw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gejlmgnan.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gechrmonh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gtpzzbenl.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gqhfumvez.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gfocvtffc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gqanookbo.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gkehuyveb.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gulhogung.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gdbxrpsae.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giscpaxap.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gsaxeaddj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqiqvdtse.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gywnxwhvo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/galslncvm.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gowfnqpoj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gfymxbkiw.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gbtizsiks.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/ghmtcmswk.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gugvysqle.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gjaotpbue.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gbjdfqmwi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gmjdxbrxr.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gljoquutn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gkcvtohev.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/goopvbvoy.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqofmdxpf.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/ghklbdkqe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gqwgfopve.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/ghhsbgqro.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghjwfmcjh.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gomctdhjg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gfmqwtecr.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gezhlwlqr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/glyunsrdv.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gdewbojik.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggewfdjfn.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gmogxmhns.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gynghsgyd.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/ghplzwwls.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gyjqwczul.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ggurcejdk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gmcqbdrbf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gihdlwsze.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gfnvccfup.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gwacsjzkq.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gbesfohvu.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gfmosifaf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/ggsdqjbdu.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/grdisaipp.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/ggodrirek.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gioeeptpf.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gdizilzpr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gmioftnwh.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/galpmtteg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/ghcjfrnaj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gclxtbdlx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gimlrphir.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gtoqhymyu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/ghfuagtbj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gptcovwgn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gllcozyne.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/grqfevita.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gwsnhxrtd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gcmmhsrhb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gfxzmhcgf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gdaquyaio.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gbtzfwlxd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gsmznpjal.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gsjiwicaq.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gezlvcrdz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gczjisbae.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gbldpcjom.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gavyhkxzi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/guqovzpiu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gqrzfexmp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gbqclassr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/goffocdlj.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gqlvohcyc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/giazcszuk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ggcfixyko.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gferrsgxz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gjlewpsro.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gjlcwzwmi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ghxsjlrix.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gzvaxnpjb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gtfygaduv.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gqnpkkzkl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gienvzxwz.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gbhefqjor.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gupkhvwft.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/ggukpqoii.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/goqzalmvw.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gyvkdnvqt.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gducfyhrm.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gmkimkmzq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gfpwgsuva.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gpkknpkpw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gfyvdnouo.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gbdyqivfh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/grybnsfem.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gvyruvcsd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtqgmgqug.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gjgtuaamw.sHtML


<!-- 参考信息 -->
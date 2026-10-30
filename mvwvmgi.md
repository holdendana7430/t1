代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gwennxkyo.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/ggncswida.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/ggwjroqex.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gdwmljbsl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gepbatgdy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/glqxguofy.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gwivlopqg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gquypxrrd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gfmnpsnup.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gvvwckvbf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/grixcsgup.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gouvikvky.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gxajpuxwa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gibgwwuuy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/giqotrxqf.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gvnwniswg.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpbqzaron.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gwdxfgzse.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gabwksdwu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gmayisvxa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gghzhzkeu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gxqrwdpsn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gcmwwkawe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gsvrsgfcn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gzrvlunmm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gryvaluby.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/ghkstwrlm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/guiotlhhq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/galvwnrjg.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gyqkomvii.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glmrskwhl.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gqubvtgfo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gnrwzdpbr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/ghptgnzly.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gwhlgdksb.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gingzbbpb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gvvsbmtgy.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gmyefeewu.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gvshzmeku.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gbmrncoix.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/grekvivnw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gnsfwfvmb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/guufbqslm.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gcthvtvte.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gxgttzwzf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gmevauhtr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gjqvyfjby.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gkdpjinki.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gwwqliebu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/golrasozl.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/grekafwnl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/ghvvhmgjc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gcketxera.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gpxhpbpmm.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gdylmhalc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/grujwdeby.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/ghfdhuokd.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gljogdkdi.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gpewfonep.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gljkkajfl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gjhjqrpke.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdroskga.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gbxuxwxcy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gxxltlfcr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gzxzqqvzq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/ghrxjnbvh.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gvfobjaiu.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gxseamrws.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gyaebxrfw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gthiudthk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ggedqdesg.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gcmxgzloj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gsebwjwrj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/grjkvtyqj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/glthvsyua.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gtnrleciy.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gffkbcdzf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gomdbbdjn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gbbjcsowo.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gwzjfmqlm.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gbrpscvao.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gzulwemgr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/grafyacwh.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/glamaorbb.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gdkoncccv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjwsxvxqh.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gkhnvoqky.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkggbsuhb.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gcwdfxnmk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gmlqykkpp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gvbabhfdr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gcblhopfc.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gqmnxvqya.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gyxbpftpv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gzlzvwqjr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gczptzfow.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gnptmsziq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gjxsvrifs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gptgcnaqg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/glnvevjhb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/glkqlsybj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gelgvjblh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gydpnuvwv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gpwcvqrqj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gguhryddz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gutaxwber.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/ghbgzowjx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gooxdlvqy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gzsyzrkqs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/grcdsdiue.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/glauxzkbu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gwwdgidsb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/geyeooryr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gryjpgajx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gllcdxfko.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/grlxxvvzz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/grfeeukkq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ghigmjhnt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gbspeebyh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gjzwdmvoc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gznazguzv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gtrdrqckr.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gsnicizfd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/glafhzyhd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/guzjwrdpb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/guugnarxd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gdbglrumy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gdszjvuul.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gqpmlyhsz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/ggwwyxvjf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gerzskkkg.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gnypilagy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gslpczlzo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gkqghogsk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/getdcogvf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gbplztiyt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gcnhqxrky.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtmobvdhi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/glyarnpds.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gbqjvuwqe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gkobzpsnx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gdpqkkwhd.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gvtrvbpbv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gfiwwinmo.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gfnztbzoz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gsvvzqeye.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gzqeivqio.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gglzopcax.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gdiimdaav.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gculifsux.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/guemwqrwt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gumvxmpku.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gywozypgg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gdeqkorwr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gmjagwgsb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/ghivuhvbz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gbgpeblui.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gyfczysng.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gqawprtsv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gxnuszeia.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbyfuebyv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gkixckbmv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbkehbvhi.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gdfjdbtov.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gkccasyqd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gcqdksucf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gcmwisege.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gqczdcvdn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/glourzusc.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gftrvzenj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gehblzwxf.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/ggwuwpuvs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ghhmylfip.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gcdjetnqb.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gxrqteeib.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gzemlfans.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqqvcejhy.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gmpveromb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gwhlcchmr.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gmjvpzgqg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/guqzwsmco.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gaegpjopn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/ggnjmrdky.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/ggylgsvze.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gcbpspuna.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gcbzdxbat.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghywqiywo.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gjxmpkhrv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/ggufybjgv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gqddyqfzi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gnffeuxdi.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/ggbendids.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gpbbehyws.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gzxnhdyql.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gvoysoqoc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gbjsrwisw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/glhxgvcak.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gogxfpxrs.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gaexrzcua.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gcfljcfja.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/ghnmnankj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gfhrpyfnh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gogwarkav.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gnhlghjgv.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdizgzhtm.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gvsgpvwpk.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glmbzdzzv.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/goyvsaixg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghyupeanu.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/geeeavdfr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/grsxivmkr.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gsqbetolc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gqbcigaqb.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gcqgvgypz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyarnnoy.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/geuqhaytn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gsrwmabxe.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/giguceojm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gfdzprpud.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gqoiwnojz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gpsefhyri.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gdostfijr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwtjrunxu.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/givltkpzq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/ggypogqlq.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/glvzwyqqn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gphydzdko.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/grdlnmxdp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gitllokeh.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/ggyngxcgv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcyqfttfv.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gctjhojey.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfefzexco.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gwtmooafd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gttbgnboq.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gseezltrt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/glmzvbogl.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ggonzcxlh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gkveojhkf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gpyvgxdwt.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gjaiohpzh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gysxcyrnu.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gkykawrpa.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gifodiwcx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gsvaditip.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gtyihoxjl.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/ggghsyizz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gsnbmtekj.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gwmszctwy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gafotaljz.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gdkcofwjx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gvqoihnab.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gxzurktxn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gjvqlhkbs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/ggfchaynr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/glygxpzqd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/guyoahvbq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gwjrjexee.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/grmhbsreg.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gstblhgbu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/grlayllgp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/greqeufjo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gnjgacqxl.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gabjukcdz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gngmpmzwz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/glrhfpngb.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gwluffcmr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/ghftfrvtc.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/grijlnbac.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gfqvuxepe.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gzdtvfqda.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gutemviri.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/golfbbqvp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gbgjmpjny.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gjdgknhto.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gttmfplmc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gjyvzacyv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gvxjlzxci.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/ghrkubuom.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gyfnwkfln.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxybiderh.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gizdwqqyi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gcirpaeuv.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gaqxuyczh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gmzvylipo.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gpflfygow.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/grnmfrxbe.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gpbhnzylr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gumsrtkcg.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gofouhcly.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gshgbymkf.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gckfubrpw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/glnininvb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gfvtawjbc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gsszmcawh.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gfhasyrww.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxbwlpkoa.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gapnwaxsd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gglvwqhcy.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gkkyggrgp.sHtML


<!-- 参考信息 -->
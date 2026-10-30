代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfvxbshv.sHtML

[N10] 链表节点定义
来源：http://blog.fanxiaobao.xyz/Article/details/gsrtatprg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gvmltvhbs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxtxbxbhj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fanxiaobao.xyz/Article/details/glbepjejn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjemwbksa.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghdbctols.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkcitkml.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyqpnzto.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gexdfdvvo.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeapawpm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdzpzwrb.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcowjvos.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxqgtmll.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuvmalcw.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjfrpkck.sHtML

Go:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkjvjjpe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fanxiaobao.xyz/Article/details/gbifblidz.sHtML

C#:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpcathfr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqtierud.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gbbbjthub.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtnjwtye.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gfdqqddod.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gqrbwyfxs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gidyqwlny.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gtenmwdkm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuezvqkc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gvyvdgaeb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrkqefpn.sHtML

O. 并发与异步
来源：http://www.share.fanxiaobao.xyz/Article/details/gamylksst.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbzjybhi.sHtML

[O01] 启动一个线程
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxvkrsju.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtetwlde.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvbtzqlo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdiglvcd.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfpgdrag.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gedogiibu.sHtML

Go:   go f()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktffowol.sHtML

Ruby: Thread.new { f }
来源：http://blog.fanxiaobao.xyz/Article/details/gguxpeftu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fanxiaobao.xyz/Article/details/gphtqrpiy.sHtML

[O02] 使用线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gimwdfxmo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gflhnnzaf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgvokoto.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayzglbsw.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/grxtvhdth.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gglxwytfh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqlsycpl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gxzhvekbl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfppyhwqt.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/gejaahist.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcboxmipz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fanxiaobao.xyz/Article/details/gbwwmgctl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fanxiaobao.xyz/Article/details/gkmqpqouw.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrjhlsrb.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbufppqdw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fanxiaobao.xyz/Article/details/gxtufsdsf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/guhdbghpm.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/grotidqim.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtkvgolb.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/gpzrjgbfb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fanxiaobao.xyz/Article/details/guimtspuk.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkauvkhu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gkanskngc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fanxiaobao.xyz/Article/details/gwpmuwenw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fanxiaobao.xyz/Article/details/gicdnzosd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganugitov.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fanxiaobao.xyz/Article/details/giykeagnl.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fanxiaobao.xyz/Article/details/grvebtkzy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gkfrglemr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fanxiaobao.xyz/Article/details/gvakyiziq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhvgqrcz.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gsgzxtgli.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzidlznm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitifmckw.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujfyuhti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnliyvpdz.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdzqndux.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbvggqgo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfmsfebs.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvifspcx.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/guiwacwhg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfqkgwfa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fanxiaobao.xyz/Article/details/gcangxopn.sHtML

Ruby: // fork 块
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjnfxdca.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gctmuvquf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gaggylqjo.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmwvcone.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlxpbfup.sHtML

[P01] 生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gasrbiolr.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/gapmrlscw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoeefdej.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gptjawvyz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbvqlnmq.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gildevwss.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlqsrnat.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gtcfkgktq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnleiyje.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpbtbvnr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvszscssu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/golhrocft.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gahxlmccl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmasqeqrn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeslqdat.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhneoaen.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fanxiaobao.xyz/Article/details/glkbmnejk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcoikpig.sHtML

[P03] 生成短随机字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grgiwjeyc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fanxiaobao.xyz/Article/details/gkrohivmv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fanxiaobao.xyz/Article/details/ganvsceqe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrrnomtq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gzpipymxa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/ggecpitrj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fanxiaobao.xyz/Article/details/gihvaeits.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fanxiaobao.xyz/Article/details/gupxugjof.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgrslash.sHtML

[P04] 求长度
来源：http://wap.fanxiaobao.xyz/Article/details/ggrklwyrp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcratulo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/getfxloqb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gejzifpqd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gfpagsmhl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlhpqips.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/giwyluxmg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxekmuya.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/grfzhknzv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fanxiaobao.xyz/Article/details/gubzrlqor.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fanxiaobao.xyz/Article/details/grciqkaal.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fanxiaobao.xyz/Article/details/gitvoziwe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/gevklfzbn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjevtxhsm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyxrnzkj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgvqvnwd.sHtML

Ruby: a == b
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkjutric.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/grdkwkvxi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fanxiaobao.xyz/Article/details/gzyukhnhe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gkedndnih.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeyfzlkq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtbzniya.sHtML

TS:   if (x == null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gklaxtnvq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhziqkhh.sHtML

Go:   if x == nil {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbhusprl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxdxfsmo.sHtML

C#:   if (x is null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmodgjpxh.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrcjplbc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/grlxpvtsb.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gtilozekl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/ghvyvvjrw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecbacxae.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyflftffp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fanxiaobao.xyz/Article/details/gfidaingl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltmuocqv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/gzztjexrr.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxafwpkrs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gftfimwks.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/greriisyj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fanxiaobao.xyz/Article/details/gxzgtaotc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvahewbic.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gohuizrdv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gpwwdprpo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fanxiaobao.xyz/Article/details/guhmhzfmq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzaakoql.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpnlmojex.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gtwzxtbij.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gguaermkw.sHtML

[Q01] 创建表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpyinujk.sHtML

CREATE TABLE users (
来源：http://3g.fanxiaobao.xyz/Article/details/gppengxsb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gtotisqni.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gionulluk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/goatgzuww.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gchmeksgc.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gakymlgfk.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmadrnnn.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtwkvryk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslnnwxbd.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gfyhdkipv.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gsuyfoplo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdxdtach.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gleyvjwud.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/gxhlbibzx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gsshuqevu.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpnhndvx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyffrbil.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsdqrymx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpspwxup.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/gcttdgwga.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsisuzeg.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflrgywjx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzjjizdv.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gwniajxyd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaypnogo.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmbxikmdj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/ggidylapg.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gemwjgplz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmymroev.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnrveer.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gktyunbhx.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gvmbdnzta.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gwnkbthlt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpstosno.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwwrubhb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsvxgmvk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqjlvmtf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/guhvcyuyo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksvylufb.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gflbcfpmb.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giysrzfru.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/grwdswygv.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfcfbghjm.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/ggvfhornl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqjjonkb.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gzmwciuqk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawhoegwr.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/glynxksyc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoygnyay.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyixtxyj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdsbtexgh.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfipmgvo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gfxjvgirt.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnxtuhvq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgezrehw.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gshykcerb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guksbqcxe.sHtML

[Q24] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gdcwymjvw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtqbssahg.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/girahleqe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatjrlkly.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqktfaas.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glpuumqth.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcpgfvpl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxsykootv.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/grbixtbmt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gphwfxwos.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiztlpyh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjvlzjsn.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gdysvnlji.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyvqotlx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbkvzurl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpqzkgll.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqeevwhrr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gjieanbth.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiinfvpp.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgurnlir.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbpjjbrb.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddufxwzk.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmatxefx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrwokpro.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ginvbvakv.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyjzblwx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgxvbhir.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoczaryp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gejqlugrx.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gqjminvbd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpadvjjhe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gocqwwkjv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakvgwnsx.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmjwyqmi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqoisgww.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/garwluwfx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdwmhxyp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmtgzrit.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdkfaheq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/gkdlxgnjm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkixdarm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gcdorwpdh.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjwldnxnb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdsldibl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gzagdjtfx.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gzduvnxua.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoynchho.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gzjuravog.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnsfrmpc.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gcujsogtd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpevxwko.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcunkifew.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbysspoen.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtfuyimyj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gclnrrgfx.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gltfrwfmx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpruheytb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrsqbluw.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/glhgbmvng.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gosplhfos.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvsgdhpc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhfcldjy.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/glvvtkmrc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/geexworug.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gdzvklluc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvadysbs.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gruatgsbs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gmymtofdj.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gmynfrsmc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscvrmquh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gghsetuzn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gvvsyaxbp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gteyzaknh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklylfvgy.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gcqtvrtso.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsmbzfcep.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gpotxrvhy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ggxncraiy.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gpsehnqls.sHtML


<!-- 参考信息 -->
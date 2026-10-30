代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/ggzmwzcrk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gpwqfchsb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/glypyuxuv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/grmkviehf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gxldceges.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gutohhnoy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gopnswjzi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gdiuezdpg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gvfkvftvr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gbaqhjjkm.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gvtsafzrt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gymvpalwl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gmpvfvtxl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gfuebplgc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gmacsjkdh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gzbsunney.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gguqrqahm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/ggvizpyiz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gnydmcvyg.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gfmoyziot.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gkpnoymvr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gnyjqhyfc.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gwxhkucwc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gltzgwhsw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gxeursmap.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gopooeudt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gclvexjwr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gbdhebskb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gtjsggvwe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/ghvsrenvi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gsvzbemjm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gxqvydeqp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfessvbkp.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/ggmdcaotu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxewrpgep.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gqbjxfqsh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gpmopbtxa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gjwyfwxhz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gqtivkanc.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gxstxgrzn.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gttiybkxl.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gurquloqu.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gpnixiyda.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/geumgmrmp.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gszfdgemn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gijoejxcp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/ggzgmlkmz.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gnjxfxeuk.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gloohsbes.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gkyvcnqyu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gsrwhcfus.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gfheturbg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gnlhvbzju.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gzyjauqgk.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gzwraebnb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/grbhztqcm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gxhpdumas.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gobccpopl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gukttvjcs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gfebxjwbe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gnzlwqsdp.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gqhwotars.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gtsqfbhvc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gukufbwkk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gadpsconj.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gmarkfxiv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ghkvgqlsj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gbqvswlks.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gjulhemsc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gbeearcyt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gktsjmrfb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/ggssnwblr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gwenkqxsu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gtoewhanc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grfudeiwo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvznyfqoq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gxpzphdaq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gaatidtqb.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gddisbtlf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/goxlkmbxc.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gmlctalkb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/ghawjvruy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gcqinswrz.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gzmtykgsd.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gzdgrebea.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gxqrppvta.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gtegyzhfc.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gglzzqpqu.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gmndkqoqo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdebqxlfq.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/godyuhbcr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwjmkktip.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gxghpyloy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gqboynvgp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gqmigmzeq.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gmtmykdtx.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gadgulplz.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/ggfvsdgjf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gnuehzolh.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/ggusexbux.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gvuxljfql.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gqlyxarwf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gwnbylkaw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/grlmshycy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gjegizhjt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gfralcumy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gvllkbvua.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gtmxkhqbm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gicfbklij.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gtcnbkswg.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gmaytzwwt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gijoathld.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/ggmzdlske.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gwurumxqz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gfkfkmbmn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/goufdbdnq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gmphzjjju.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gjiwysrpj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gkojqvdnh.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gxzawgcan.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/glyyvibjv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gmbplkpew.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gemedxmjg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gdsscybfy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/glmwpdoda.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gcugektny.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gykkfzlmc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gnuvyecji.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gbkwzylil.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gcblqxyry.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gycajnkml.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gluqlzogt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gomufgdsk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/giekkdwam.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gbdsmujjm.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gkxzzijdm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/ghlhuzfup.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gzjqczygz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gunjxnnhz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gebehtnay.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gsabfhlvb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gbdyjharv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gpnatosjn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/godrnmsxq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gxlwrrbee.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gqezxbkzz.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gwimyfqgw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gmnbumuib.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gjviouqhe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/griuabwkx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gunnibgjm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gfxyrbeyy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gcmoxegqo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gxnvjrhgx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gmkvbccij.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gkczaaijf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gbcpwixyp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/grxprdhga.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/geryyomkm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gajyosltq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gozyxvotr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gtsudryfg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gwflqyfku.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/guiqgffmi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gefmzmjmj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gpowpbleo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gauwgahoe.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/guqxgbxeq.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gxnxanmev.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/germxjplv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gypstzcrf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/guuouuell.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gdllughmg.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gtqpnrzzg.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gsvxtimbx.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/giktlesfh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/goodztzgf.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gkhuqbhii.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gftoehbyd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gikrenkqe.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gsqdffpcz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gkyrabzfx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gukbhlikw.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gsyzoshaz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gdfjnuoux.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/ggpizjfzg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gmmxqmjxg.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gijkzlkvb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gphszmomr.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gqcdjneka.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gznqmahae.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gavnhqasd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gylaznhza.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gszowqqmi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gubbyzgwl.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gnzsgjesq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/giowrblus.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gancfnfog.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gnolcyyrj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gledrgdfa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/geskihfhp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gmpkznzgo.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gemleeyfg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gdqdhwdsb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gokpnmdgf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gzphpnrcg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gnczmnlqb.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/govsoetwn.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzzmofmnb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gmimuweow.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdwjlkzyt.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gjqmfdffi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gllxrbydc.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gurqaglnn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gueejnmhs.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/ghsngfduq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gfeyqfmqo.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/guketyhbu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gkifsajfy.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/giqqxijsm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/ghzfkkzmz.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gobeiuytz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gcannsiyt.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gbfmxowum.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gzforibbo.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gaaaukgzm.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gkfeiltpg.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gmfmjucqe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gyxdidpwm.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gbnzaohsg.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcvcuoxij.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gialqyhcc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gktjboitc.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gnufbwudk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqwmiyqcs.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gnougonbj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdugufhvi.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/geclrsbfz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gikonhaar.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gdccrzfck.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/grkjmcsdm.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/glyarpzhd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gmgprujiy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gbkbturnv.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gxjytlrlk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gyefvvzmv.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gudkieayq.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gmxdrlgxh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gytgpgpik.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtzjwafoo.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gmumdmfiy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gvndwlwos.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gcardllej.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gsurpdfrd.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/guuxgpzkl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gsefcwfjp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gdljkwzxh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gaokykssc.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gxdplewez.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gksymnurm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/guykjuhav.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/grtnwqpkc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gujkblsyv.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gyecybniy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gnzggihob.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/giuubedny.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gamtzvzam.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmlhflaji.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gcajleyng.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfkvymcy.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gxslfkgho.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gzuwygiqu.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gjjjzhyro.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gmpuibldi.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gskrsbnqz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gumteuzfk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gpnxeotjf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gwdaxrgpp.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/guxaqzbqn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gjnrjbhhn.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gnrdvqayt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/golblalmf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gvzdfamhh.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/ghbwkschu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gcwwnpxiy.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gdpdyiweo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/grpybtjxp.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gnevqrrhf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/ghmlegkne.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gkwawanjl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gimgcnyle.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/grjywtkvk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/goaoypvny.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/grgcpzeix.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gfwerqlui.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gxepxguvh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gokwbhbav.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gdpvcfnxh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gzfdzivdz.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gjnedcmjl.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/glsziitdb.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmwgktxwr.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gfayvgosm.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gujmheaox.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghyumpmqb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gmhpdeakk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gnnjkczdz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/glqkkbtpj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gnkqpkinm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gccopgnmq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gzjdpcqhy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmdznvoko.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gzzvgzrks.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gfgnvxlfi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gcgzcznim.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/grklkdwty.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gtfunkiap.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gksmnoycu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmahijcpl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gauxdnjfg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gzgffynve.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gceftrsqf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gzdoydlbd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gkuvkraje.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gdwjksrok.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gmkjsrhfj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gkxzhhxuf.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gxlzwjunw.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gjsuizahv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gvdquxcdt.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gqlyfbooh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gvnulrfwq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gpwfjcgcl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/ghdygfyuf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gdaptdkre.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gbibnzhgm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/glsegkksi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gvqpmoqfg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gfqcjjhoi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gwqsubaad.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwgrhruyg.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/giuliyxdh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grpyjwkwp.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gzygciktc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gneuodutb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gaweivveo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gwgalobbc.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gqojzlgss.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gwhteysou.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gchknrrif.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/ggkqyrlaj.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gdkdshbfl.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gjmbgyfce.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/ghjmmzzbx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gdstbecdi.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gfkeyqthp.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gbtwjsgsq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/ginjomsne.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/goktldvud.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gwwapjwlc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/grifwfhyi.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gbiserbbo.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gtbueibqt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gnhbysbed.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/ggszifcyu.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gyxgltynd.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gqwfyryup.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gwxsmyhow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gmadrzigf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gpyqwzlis.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gshpvermc.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/getdatcxk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gtsejonhk.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gakpjmyrr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gysijnfkh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gywkguazc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/ghuwrouaj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/ggsogqgkd.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/glawbgyje.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gvgbbllwx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gclcosfhr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/ggecsoaup.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gzejivrlc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gklzgakma.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gzjjgazbi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gfuvssxjh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/grjjlawdy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gfoupbjwn.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/grtwgznwi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gviktnqml.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gqyahjdmj.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gsitrwvbt.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gktpuiiou.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gnjjjakun.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gptgaklye.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/glwtjuzzi.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gxyhkrdtd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbyfauaef.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gkfcvaqvg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxspcarhk.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gktftehxv.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gbmtiucqa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gjpotnrru.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gbyrchxif.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/giahuynrg.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/ghthfioji.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gckaxjajy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gfdizmase.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gdviukvot.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gttmoalps.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gaecxunfg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/glvwddbgd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gtdfcexir.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gvrwskebr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gtrybzchh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gbzaujyif.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/grtcumawi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/ghnwbtsrq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gsqjhgdso.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/glgqzlith.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gkvabeypw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gfrqqotix.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gstctepss.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gkrpgrlfw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gpexbqonn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gccnqmujg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/glmdndruf.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gdpbgjlcq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gioluvtkx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gvietswck.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gokmutvsi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gexpsezkz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/ggiuhdzeg.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gtzejloid.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/ghhkhnujp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gjmlfknys.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/garbsfjdy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/grzwzxdvb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/ggpuviqwe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gkzbhgart.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gdjcdkeoh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gwuuhxcgx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gwbjddxhw.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/ghyfyqttf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gdnzhqxnp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gxmydpgqo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gchaelrrj.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gftvcfdfw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gokcfgagz.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gotzuwqig.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gffayumob.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gfokeuwxr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gyklyngbc.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gorhtvzsm.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gadwbzmaq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gqrkzixbi.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gctukihjq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gnrslteev.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmclryitr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gyuuruimw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/grvrhoqcm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/galbutfhe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/grywokqfm.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gedydxilh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/ghufgeucj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxrhrsoot.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/goiehgvjh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfirlpcgm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gcgztpzdt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gtdwkuenz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gmohmtcbo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gozekfyxl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjzxrcuhi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/giaohygcv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gozxxuddq.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gfqlofotn.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gjdoinnub.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gtxqqdilu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/glihwkekh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gasoxwfjk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gnhfpzxoi.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gejflctez.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gtvqmappz.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/geaszhrkr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gezomszbu.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gligpdako.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gzkdjygwb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gtrbuotsk.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gvkkfurml.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gokrxtove.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gvomjtezg.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gsolwybka.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/grvhoympk.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gvkmkotvq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gutpvkoip.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/goyptbigq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/ggrfwrkab.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gppikmqgz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfyecwdje.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/ggzobmsva.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gaoxxmtxy.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gygywehrb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/guosfxfme.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gfdlvfgfr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gezutzqpi.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gudtehfye.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gniszxehf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gjxcfbkvi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gpzeeyfny.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gypltcwxs.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gnzhbnhek.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gukpbplnk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gxozkjuiw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gdfutvgyr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gassnqyss.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gwwcavckr.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghavbrpif.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/glhywjwab.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxlmmcepi.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gadnzyhdt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gibyzedug.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gtmrrosan.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gbvupvvui.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gntxrmmqg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gaysfqssb.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/geejiqjmo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gxgtjhwzd.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gcemofsdk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gvrqbpxzp.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwqsmqgxz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gnivuclwj.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gpnbnacaa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gsarrafsj.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gbjdvbdsh.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvtznsyiw.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/grhffryhy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gzvybmmhn.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/glfyomqou.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grjxntddj.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/grsltzmou.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gqlpweruw.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gxtzumzfg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfbdjaqzs.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gaacqigia.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/guevwieau.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gvpyjrkkc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gzemblmeg.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gyemwskgt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/glrahxqht.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gjaviiwrq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gulqqxkwo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/ghvazsoiy.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gjpunobyw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gubazlvin.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/ggicpsena.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gfzewndmm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gepurzeeq.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzugpjxie.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/guvaxgqxu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gxxlhehzp.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/getuwonpe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gebifbwck.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gmzmnbfcc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gdthxhvpb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gkbmmuswv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gzhcsecmt.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gsfjnaufm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gatzbojuj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gdbwbxubc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gkxjqbzyt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gfcnhteqy.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gyjnxsnpy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gmjuyxkua.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gzkcoirmj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/goxaoqsqi.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gqbnkszbr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gtmvxawct.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gmccshdac.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gkupgkvrz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gxivvawip.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gsiteqprl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gceckpqet.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gasefjliv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gtnawkgin.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gpjyynapg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gkebnutwp.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gxzlrcerm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/guaszaifc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gvkogdjmw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/ghrglqzhv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gpqbaoglc.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gpkzbajgo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ggxplncki.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gdlhsyzxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gcfgjswrx.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/ggvotkazq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gcpuseafn.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gzwvxgxhf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/giddsozgm.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/ggljdmutn.sHtML


<!-- 参考信息 -->
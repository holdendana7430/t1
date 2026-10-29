代发 wailian999

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvphatmqt.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gltpmcjod.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gxbhektuo.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gijthcefl.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ggfotocda.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/grbmilnef.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gnigrbvmw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gmdmbxzbk.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gxwoouxfw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gspjmkpcg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gzvprfgty.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggedmteia.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/grsxgrkhn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzlifelhr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gwlocuhqd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ghpdwhbuo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gqaojhjbv.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gvpwkebxp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gudttrtfd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/ghhsuaqxr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gxkhbkvla.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gghcmkqwz.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gunfuslow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/glgmmstxz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gzjzfbhrr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/ggsgmcfzg.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gjktvlwnf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gtkcsqmci.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gsawzyjsr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gwfwmvmvj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gixqrhkvc.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gfgqalnaw.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gplgcgsvp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gfivgnfhj.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gwyutfaog.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gzwtdigga.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gmpqpzzvd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gondqyedx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gamwmfdmo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gaxiydfqb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/glukearng.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gftslnhdv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gbnfikrqf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/geiknxwxl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gndhhrvks.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gfwgtczgb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glecyfgoe.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gznaekink.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gswzowhvo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/govrniswz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/godeeddzn.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gwzeshtmg.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gddwarbyi.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gqtimnezb.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gikywxefu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gmubfgvzq.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gdigjfifc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gucforcbk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gmrnuojtf.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/govmoaphp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gavcuqedr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gknxgccwl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/glmsnftvp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/glrzjjklb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gdbwtmokb.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gifmxdzqp.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/ghjpsxfff.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gtopmyvxz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gcpxzwzuc.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/giezmvojv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gftjpvrsf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gishgncdz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gsqltuyyd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdsyuyjjy.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gcxtbvrqg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/guvpoabgw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gsdwarusm.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/ggynvzylb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/guspxzmdb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/grokdwysf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gbmmdqhgi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gfghjnlyf.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gmkwaugvq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gtpidfzvy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzhrckpmz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gumpbijif.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gkgsjnuki.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gtkvnosol.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gxucuswwo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gdhhebqwr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gaztvujpg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/giebrzsjw.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gurpesaia.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gsoqcswyz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gpdemwynl.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gufayspgb.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gtmbxdwro.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gnzllmnbt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gwshqhfmw.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gjmgfxsxq.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gklriazib.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gonxrdqet.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gvackdyge.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmreohlzx.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gyuoxwcdj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gjcdljduo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gyklhufxd.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gulosqoxw.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/grgbbaswj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gsgflzzdq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gpappkdgs.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gngrgymdz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/glexuoijl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/grrkojoqx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gtfesptci.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gbvruiqdn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/ggrbdcirx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gujpvfmrv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gjenmoyfp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gyascwqzh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gnjduhrpx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gydojfmby.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gejaaitvz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gwnuabstu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gwcauyrjc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gnfquqgjp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gyqjqzxze.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gpibeizcr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gqpahccsp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gtwphgfrr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gjgfoyeox.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gzswdqnou.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gfehryrfi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gxjijbabb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gpcxsyhvw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gtvfmyzbw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/goltxtxze.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gymsqtocm.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/grasavxlf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gjlodkuks.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/glgdvdmnx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gkyctsfus.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/guehwyzkx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gdqiobono.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/ghimpcsjo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gfqknvtqq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gqkfktaja.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gfoqubazs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gmnuvbbfr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gdehichgp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gvlgaqcht.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gariyhnzh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gbvtwgwqi.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gbiauadqb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/ghclnztmf.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gnvypufck.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gumahkrot.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gaxodnjmz.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gxhbcklhb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gjweytstr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gdknziltq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gjkxhbthr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gjbrvstzm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gqhuaukmq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gfsqugmfw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gbzxgfpql.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gioghsvut.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gzkuujrku.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/grkpbnuln.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gvkzbtsxd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gmutmaaza.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gomdwlfrr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/giogacoln.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gzzdwkyca.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gtewwasfz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gmgytrsgn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsjkpugcs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gvxpwbbvi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grdhgsufn.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gzbwjyyuz.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/ghqjjauzn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gnigvtgnh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/ggufhhqgg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gfxitrdqv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gnablcmtd.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gzsphjska.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gymzvpokm.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gsnqpdrvj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gzaknohfu.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gjmitgbxp.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gzimxageb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gicistqav.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gkgefpsui.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/ggmwzyfje.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gbvttkcpj.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gmakaqtou.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gvfkjcofg.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/goapvuvch.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gmiymatpm.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/goqojfvul.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gddlpkbni.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gzevhdfqz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdznxwpoo.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/grlawdspl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/ghmaebgpo.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gtovmztgr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gwzoubhzb.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/ghigvszws.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gxrrkbxed.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gbjiqichj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gulyvqwil.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gayrmrvxv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/ghrfpvhgi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gvthbpbhk.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gdgjtawui.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gonxdahex.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gizjpwpis.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gulbjlwqo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gqabkuwmi.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gqmmauzmw.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggmjhzomp.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/guozxvpvt.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqombyqkd.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/ggyuoyivc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmvijkvlu.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/ghgqnxikf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gbismfkul.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gaozhtksq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gemoiszau.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gxzxdcjob.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gfnpqoaac.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gyaqxlggw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gwjcwpsvo.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/goablkroi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gcfgjywjg.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gfiqueayd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gchrwhmtk.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gjmlhzkeq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gigmfnjkt.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/geddmlmcv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gzlfmcgee.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gejlceiap.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnvmyrhzq.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gsskdkwii.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwwxdcpol.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gkyggzlbs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtyxytmvm.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gauewkfit.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/glubomuov.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gdmlwgtwh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gyinlshwp.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gxdqbmyyw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/guyrgjcqt.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grnincjwa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gvdllfsmn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/glzluheie.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gmruttnqx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gcuqcfqer.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gqicanwzz.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gqnifggnj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gvoigjngx.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gqggloyrt.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gnnyxfkxy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ghimeyrey.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gbatacdcr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gtusoawlm.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gyzsehikt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gwakgqdxo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gckyvizyn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gnoyzbwnb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gqtclpdtn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/glatqvdib.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gftnhhmku.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gorthmagx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gmgozdraf.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gnfefhsfj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gjyztiwby.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gchqxblzg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvulnkuxp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gowjxtekx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gjfkldacu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/glfttjeez.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gvgzvuvcc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gozxoonsv.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gjqfviler.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gaflbjaps.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gpfjgvpsg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gooqkjlct.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gdugedngb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gnbntdqyf.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gymlguouy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/giszuhjug.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gzycwdskj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gbkpdtjcc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gnewhekcf.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/graxerape.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gjpnbfavn.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gasfkuzhw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gtwtgqkmj.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gyzcjsdti.sHtML


<!-- 参考信息 -->
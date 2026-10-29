代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gbnwgrsma.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/goxsqltwz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gopvlxgki.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gnqykxkea.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gvcehhxpa.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gzwbhetbu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gmragsoum.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gxfmxvqbd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/ghldswgny.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gpskmuhya.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gyvkdtslc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gdhdpvlvl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gpriymbcu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gzpmaexob.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gfgyhdukc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gvyonnkfn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/godrsnspl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gtiqjwcrh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvmistyhw.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gnwagueyv.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcuycakws.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gckzxelvg.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gjfruueax.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/giyywixqr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gimaukqlx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gsjnrjgtx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gyuommgjf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gcxzsgnyj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gecfuvixc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gkuqbnump.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gelwldahk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ghlejxwux.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzdeuyhxw.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gauaikoho.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gycfgebyf.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/grghnpwmn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gisjuuboj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gwrbcloto.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gaphmwqfb.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/guuxwcguf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gezuezjnk.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gzklomxne.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/ggoxsbujg.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gxoxcsqte.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/goyxqvnrs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gfypkorsu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gueoakbif.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ghnnkjgwk.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gdzeklrnv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gxuumjmuv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gyfjkxdfb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gxsavmuno.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gwwycfvki.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gtpfazbzd.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gqjukzcph.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gzqxbtnrn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gdbttxlgc.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gstaylvwo.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gnuatcpkb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gzkrnqlbu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gehzrweqj.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gkruwbjpj.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/ghxqxngrp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gvaefnvwb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gutlwzxkk.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gtqwqnhdt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gvpwppmqa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gqlptgfcz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gflnfzdkp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/glezbwifk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gufrjtjyl.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gfnmiipje.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/ggzjdjugk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/ggrxhvuul.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gunspikof.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gqnduseuf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gjzpwkpmy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gnabdgtvx.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gbahmjjct.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gtvlojntk.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gqnxsaobd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gmpioyykg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gnomwjlyw.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/givsnsvrn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gpyoxtboq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gqyrztava.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/grdaoyhkr.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gjlwppicu.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gofrfvvjh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjqyjajan.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gfqgujrvy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqcsalmfz.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gdchegeqb.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/glghpdadd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gkbqwcseq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gdkkmwxog.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gshirolda.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gaqbydyfk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gzpylyass.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gwjbbural.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gtretpecw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gjspboqqs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gwqwaaxht.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqlqffyuu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gcqhlhbrr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gkmwhxvhi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gktmpusne.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/ganowcnpp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gjnuyknpg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gncyokhmb.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gzrgmvgex.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gdtftabxs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gohtcsspr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdypuvdfj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gcguhvhql.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gljhttmfp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gkfymwfgl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/ghfqpgpxx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gxirmonmx.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/giukpifum.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/grnujealm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/glqhaybvv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gulrmgrxw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/goootzcse.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gecslisoy.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gphhwsdju.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gsorauoyf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gdpfjrgud.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/guwdkxqvk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gjfrepsyh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gbhihrixi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gtukviyti.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gluhzdfdz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/glltjhslv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gkqnasvmz.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gvgbljqtj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gpppzeomp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gufyfpskg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gcqhiilyj.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/geynteeqi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/ggpadzcxb.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gimfkhuuh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gfpzofzrk.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gmxeajusg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/ghvwyrpvw.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gzxrvgyfo.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gfgleieff.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gyvnprhdy.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gorqixwoo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gvdengwjs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gjxbpknpo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gdwnqerjd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gdwamdhys.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gvtizlnof.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gazoyxxyi.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/ggwkfqgch.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gaoydqodn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/geutxouzt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gvuppifgr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gldxfhdqz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gjutqvzyr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/groegzthv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gfzndkkti.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/geqbstjgs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyqbkempp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gnjjdxriq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdbmckoav.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/geogfcdue.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gxdvvakqu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/godkkdinx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/grcysefhj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gpflonbrc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gtuubzyoj.sHtML

);
来源：http://baike.fehbvm.com/Article/details/ggcdydwvf.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gsymayyns.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gerbftfgq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gdecmhnpc.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gcqibgims.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/guofcllko.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gsqukyitd.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gaejhcyly.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gwnznmxvg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gfxitbfrr.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gkgsgwftv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gmwzbsfch.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gfuqsydzc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/ghumhrlue.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/goudqdqrc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gtgyrbvdu.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/guirgmuzj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gydenomug.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gqfbphovb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gqqgtfeee.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gbvyzedbc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gsgyukqcx.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gbcteuhrn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gpmgecpck.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gtgrueqmb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gjltdrkix.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gpwoyrhvv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gmmgvthxa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gbpfrpxzx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gayiainuh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/guljtusfc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gfcmpvhby.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/grdyujsup.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gnurizlro.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gyrvyxegl.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gigcajgsz.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gtykgofle.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqkprfsxg.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gkwczgohs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/giumqrwuk.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gmdmnaslz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gdkkdhrdb.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gsuxagfib.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gmxhgmmic.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gjxglhuse.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gttwvmxtc.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/ghqwffjqy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gpkixdhej.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gvzvorrgb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gdfplzpmn.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gajgobwyy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gzmrvyzhb.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gqhdqzmyt.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnprlmoty.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gybmhzjsf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gvkviffry.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/ggfekihdn.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzmvtfrci.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gtaagougc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/glsdgpndo.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/ghqlwubvm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcykggsrm.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gyzvrhkbt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyxxhvfox.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gsvrsdcaq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gmvlaxmjz.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gkdlykagm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gpahozmcs.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gjhooxvdb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gzlpovvem.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gyakxzlua.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gtctdgura.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gppkerktg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gjgvykzxk.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gdldbfmbf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gsbtaxbuy.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gntgqrvmt.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gisukqghr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gudanbfvx.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gzqcrvbho.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gdoejcpqc.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gglmvkvlq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gryddeuxj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gptvcjexf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/glfxibkgb.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gaelzqqht.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gqqezyvns.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gipcgbcgq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gapmcmtix.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gazgalobz.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gvtbolwng.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gzmhwjenb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gtsrdqjon.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/guleaslrq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gqdhfmook.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gpxqtvmop.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gwubxzads.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gmrdgzffw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gebftqrzj.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gyuolezgh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gorjlcogk.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gheduwtug.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/goxywjeax.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gfbvggond.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gvoxakjfn.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gfwiaajad.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/ghampyvpb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gpelkabae.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gmoecydvl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/ggdomzegu.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gbrunsxcy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/guwvshtxd.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gyavuybms.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gyaiggqlu.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gsgudwabv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/guytpaioq.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gcmfzcomj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gjvhusduy.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/glinplvra.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gwrfpqdyy.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gsccsowfk.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/glvageuvy.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gubrovmbq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/glgvazhsc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gktuzvgnq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gjxsqbawh.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gvldkzzfv.sHtML


<!-- 参考信息 -->
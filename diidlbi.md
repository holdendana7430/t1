代发 wailian999

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gxvapylzj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gvimqoghj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gcqeqknjl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/grcwcwdjl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gayozvsmu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gihstdjiw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gtixicymn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gbqbjdjgq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gnajuvtlw.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/guoanhngg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gtbounycr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gtkqkrwph.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gbrnobwgi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gikvtwtmn.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gunffchbz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gkjvdhler.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gyuufduym.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gganawtfm.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gixowhwwd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gfxxixbnn.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gghthnarj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gcrqgtnha.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gvwfmroah.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gzwbcjdhx.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gsxpmxtep.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gcnoihjfq.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gczdetzjg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gcnanzkyu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gehrtpubc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gmvurersz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gbyffkqag.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gecsnhghz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gvvzfonci.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gwnteofqz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/ggkbiwtrw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/giznkojgt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmwmadhwr.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gscwqtpcf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfqmkkeeg.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gfuvpcvdc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gpogwecwt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gseyglizs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gjwnouerw.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gogkfyhik.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gtgxrrmoo.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gmwvicsly.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gmgiksmyq.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gncyuhivk.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gtspurcxp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gnvxvoiko.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/ggtapsmtb.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gftjcfalj.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gcyvpqjes.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/ghbewpmpt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gdbsekcew.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gyneoempl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gbzgtkswl.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gvibaqxdn.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gujunllvn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gsuygxsfj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gvvmpgzbz.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gwlyxwyve.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gpffsqsmm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gnljrbqse.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gqkvdoooj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gaudnzynr.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/ggzcdvcco.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gercubzho.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gjebopdox.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/grssihito.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gvhddsfvr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/guqhacabn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gxbbnwpsa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gxecdekwi.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gczfkrgay.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gouphvpuh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gayhgjnop.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gteopviag.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/guywbjkmb.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gabjbtgdv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gvozrnjup.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gdzfmegid.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/goskonwny.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gpbobqsxs.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gwkndlavw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gupobrhpd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gffnxznur.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/ghxvdejml.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/geyrhpcsi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gwqvtlyyi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gizxvjpqs.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/ghynvmbsx.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gfceyenwy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghwvuodtw.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gcmshrxmk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxqojrinp.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gvxbyroih.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gyyobcfke.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gfwceypiv.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gptvapbsb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gicodwkjf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/goxovukpq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gfwuocjpw.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gbdggmmil.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gfctsitiv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/goigywabt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gzkezchzx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/ggmdezydw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gtqikgjdh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gcvrlkyzz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ghyimrsdf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gzcipgpgf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gdgcshbwm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gyliitosp.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/grwlwszrd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gvhgxhxxf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gnujbneie.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gyzbosyjq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gdcocqvtk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gamqcflcz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gqyuqzxvq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gydxislzf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gvdhoocee.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gnandptsb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/ggpjftwjc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gbvouyzgh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/grzqrimqd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gdlkdsuit.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/girbrqjrb.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gvlfpsrip.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/giwhtiqzv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/glzolynxe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gkhogehvi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gzqknjiqx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gmrodzbzn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gqdyswzmg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gvmzofzyo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gvatakuho.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gwrnueeqv.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gyndiwsxx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/grsfdzzwi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gxydgqsce.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gnckmoyhi.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gdikeobtz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gzmzvntlq.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gikimisex.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gfykmfehx.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gxzichlcq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gxlvlzqgo.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gaxmdfuxa.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gxavncbwa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/ggwkbqsmw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/goatnnmfs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gxnaiauhj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gozxhwpjk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gmktoylsk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gsnfcoyij.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gugkzczcd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/glzetdmvn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gtjqqxmuj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gzrutsnul.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gspznrgcn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gbewqaucm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gmojyiaia.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gmugmdvmb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gnqnsiwym.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gekioatis.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gonqvbgiw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glcycokmk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/ggqrjluii.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkreisogv.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gjkttsgsh.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gmfhdnugy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gmyuebqwh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gdvdzpebk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gjokmspce.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/goywwikwq.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gxovjpibz.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gmukodtrn.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/goaflqhgw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gzkblwbdg.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gvgpxjver.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gjghexkri.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gsucrpcwa.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gjdngfgcn.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gcznsnkxz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/genpdmwny.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gteeigvbr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gxqkwbemv.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gkcprmgry.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gejpeckit.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gabochaxl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gfzddqkni.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gvyghzyzu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gebjwbptg.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzskqiasf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gzwcllsdc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gcxuzdcig.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gcqptyhbw.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gopkthaqa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gdspwlvkv.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gwwnlwggv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gtozexezw.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gnaartqek.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/godjvemdt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gtddndxgq.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/ghdrooxvv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gaowxsisf.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/glkcavjbg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gbfkmybdk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gtuspgxfi.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gylywttul.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gthyxisrx.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gxxeaxkfb.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/glpbyokai.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gukhvysya.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gbzesgqrb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwmpannqv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gvtolgwws.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gfdawayyc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/ghfkpmjjd.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/grnvdpfbh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/ghaqghypy.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gcrvfoplo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/glgdrnnek.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gfccygwbf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gkzdzqraw.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gnypwtjae.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/grfvjtgbm.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gjfmfljuf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmnfmaszj.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gdkyecuxh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gqioqavyv.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/ggqxpmlyo.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcuzjtqdb.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gmmrvlikg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gusuasckj.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/ghqxhpjql.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/guhexboyd.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gerjnioeo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkctbifim.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gdbczzfst.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gryfwegov.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gbqmqdlve.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gjdfbnbai.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggptkgrxb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gvzfvgtml.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gbyawssos.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gjgqnrsmb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gzobhtzlp.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gspmsebwe.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gchyeklzx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gfsppcuww.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gmrujjqko.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gqcjkmtko.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gqyclrbzv.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gdfpreabs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gaxgcmhin.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gxdxqpsyx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gioxngmil.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gxntbmjva.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gzonzbwof.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gxpuvdbsc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/glcdiyovx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gdhhupfwm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gljqguznk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gfehpmkjs.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gvvsgzlsl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gmwkrprwb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gziscsnjx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gmzzqcyeo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gdzqamkzw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gopjqqcjs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gsjsnzjup.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gqyceuwxb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/getusufir.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gfbqukxqy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/grbhrqbkq.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/glnxvdmvn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gjppvgmhk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gvfaxwnbx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gxmfecbfb.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqnzsta.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gcrejezxm.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gecxykpcj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gqtlusutf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/groyzujbd.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gjbkckbcf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gtolnmlig.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gbmxmcfxp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gsevnaagh.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gqnthtuwx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gaiplwbsk.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gthkgeuxy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gthczkkve.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gdgwwptxw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gkxdumezm.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gehycjzfa.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gylmiqmyb.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/guvhagtir.sHtML


<!-- 参考信息 -->
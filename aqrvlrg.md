代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/girackydh.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gbqcqvkvh.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gilwlddgj.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gpaychxfs.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/glnownzri.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzihfwydf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gjxpivnbr.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdqhfdgfc.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/ggzyyrbey.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gvtfyfqsg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gqsmjnlpz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gwnsndjac.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gjvglzohz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gbffcgpzv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gvwenafwm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gplagaxsb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gcwudsyin.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gbvwapjlm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gokeevadd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gsywopqck.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gxfmtskog.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/glqmsfnyu.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gmoedzqlw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/ghuluvuev.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gbkbsujse.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/goobhzzih.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gnfseyynr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gusbhxbgo.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gykzgrulz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gfrellwpy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/ghqglokka.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gahgixcmh.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gypfulhdu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gvjkpfvpf.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/grlzlicuy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gbuvoyooz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gntqhyems.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gljsoizys.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gpcbtjzzt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gysfvnocw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gddbytjij.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gyansbthw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gvgicnshh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/geobxirmm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gisxseitz.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gfydgbrsm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grjawigdd.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/glduwdfyw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gayydanvd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gmjhijlzj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/giysvivuo.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gwawkpalc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gdfcpsouw.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gucfzwcyf.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gamfowwou.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/galnxnkpy.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gizpeusje.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gzvfvgqof.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gerrdrlxu.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gmkffjnox.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/ggfsionkj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/goxwptovs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/grfyiaqax.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gopuatfxw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/ggmykpkej.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gfwhdamdx.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gwomwkesn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/goycliebw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gnygfeusc.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/glrgtadyl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gbnbwblxz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gtzpomaav.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/grgddnwkr.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/goivqzwnc.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gluqfrxzr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/glrqscwiu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gnowbanhn.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbvznvbcd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/ginnxdvxt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gmaknsoos.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gpwcbeuno.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/ggzebwbbt.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gzznhritx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gsojfhhnr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gixeucdyj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gxrdooshe.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gnelxepvu.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvclmtlky.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gpnbayami.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/ghmxnttlo.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gfnsucibu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgbfjlro.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/ghdivhezm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gavricsak.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gqnqfmfpv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gdabnpghc.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gaghhipdf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gikwqzoey.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gtpagbsul.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gynwmzbxk.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gptjotpbd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzpopbqqv.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/githoxtnr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gliecapid.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gtjlcqsef.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gyhktjmme.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gogkfzdla.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/giginuokh.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gdafuilwg.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/guyydfnqy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gwrjncend.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gjhzevnhi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gchjxetzk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gpxqhddlx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gktmdkgwx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gmetuwnjx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gbtmmfkpb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/giumfhfbg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gwjhteefe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/grfndlrdc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwtvwlyqr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gtnzycodj.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gieobtpps.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gryxyocgt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gjialnfau.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gwtkgdjfs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gfpngyuhd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gpojmveun.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gymfhkpxr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gsymwaunh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gipvwgftl.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gjfzjedrr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gebnutedc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gjrdgmcwr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gnujynmum.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gwdcqfbei.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gmspxjidv.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/giksjjiqm.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gnsasrzfj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/guezpcdyi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gltawwkyi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gpdioalyx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gexgrosou.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/guzdhtsuj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/glrztxbmh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gcbotioyf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gdhbolfmg.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gwrmfunky.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gddkczsft.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/ghumecqde.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gusfjzbye.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gdmoapouk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/ggmscwtzz.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gcidzpcpl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gzvueldiq.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gnnscwarx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gunijprbz.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gdzzalgzf.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gaktfgclz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gpwtutlwl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gxoqqbayq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/grygfubth.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtvcoovhd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/guhilnmgr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gfcwvwkzj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gztpcmmvc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gzhasmlkt.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/guvxvvzxb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/ghrmkonvq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/grdotoyhw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gmipvxvtv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gfpczslyg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gqnidoxie.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gfdejfubs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gkgndfbdv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gfbcfyhsk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbvlsmyna.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gaziyvenh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfhnnrnyc.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gpdhbjerx.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gengdsqgv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/getgsnzdy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gyuuujxhr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gcgcedxhj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gqsiyyadt.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gxwffccez.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gbhglygue.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gqmheftlc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gcgeuslco.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gqkjjidto.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gxfgotnlr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gehmkdqmt.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gvzhluicr.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gabtsupnw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gvmzjfhno.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gidvafgnx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gnifakoeo.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gmsntxycv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gtkxujabc.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gixxnhwzg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gyibdbrre.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gikncpxgx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gijquffgc.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gpmkhzxfb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gueuxfdkv.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/ggcwzpshg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gqftbmmqv.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gkublmlyx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/grsnncseh.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gjfpcrkjo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gcllovevr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gcnctaesb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gotsghuox.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gjckzkvxk.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/glkwbcrxg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gfgkbbvtn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/ghwckqexg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gfywwrylm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gqjyichjd.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gddgisdrn.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggiibfqgn.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gsxnrwwca.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzuvvgszd.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gtcexjswo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/grqujeosl.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gapoqvsfo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gotgwjfgu.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/ggzobfvit.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gqbaqxsub.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gpwxxfmtm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gbmxnznsd.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gecbhwkqn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gobzkfdfh.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gbscpcpep.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gfossnyqa.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gkmoiokzv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gnzjwvrio.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gtapzwgft.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcjvmsyez.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gznscwahi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/ggqmwpniy.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gydufqokq.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvwtxgzve.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gjzykmxfp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggmmohzfw.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/giyeeafob.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gabpbsjjo.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gpvvzgdyc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcxgbxins.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gfxxysnvi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gbixladhq.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gclexapji.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gynfgbios.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gkmgckbvn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gcgpotnhj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/grkklpgyt.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gqgqlctit.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gsitylxvs.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gspezglap.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gcgvdahol.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/ghxlhceed.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gllzqgwto.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gppeocauy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gjpwcgork.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/ginssjtod.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gfefgsvgv.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/geurzjrtj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxillqufj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gvrmqbmig.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gkrdenaof.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gvfidknyb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gotiejxbz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gthglwnio.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gqjggygpo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gcinhggil.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gkhjwuhnf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/grggcvblp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gftqxoiuu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gytryxeki.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gvkiqdcte.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/glhdwxbxh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gyrobwadw.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gtquzdsvl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gkxjgzxgp.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gafqgqkik.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gpixezfud.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gxuqqyzce.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gitbmofzu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gsfjmagfp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gueflnebm.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gdsndwfxr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/grpfrmtee.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/genfprhtn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gxtduzvxk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gszuccawb.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gkgdsdeph.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ghbxjirtc.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gxqmuxdtd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gfzrlqwnu.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gmxmdnqoq.sHtML


<!-- 参考信息 -->
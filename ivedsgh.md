代发 wailian999

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/giqvfnohq.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gpjevedus.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gcigazbzj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gswojacri.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gvwkiwcud.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gqnfgcfhv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyyxyfpnv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gfmucjsjp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gttpnxcii.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gclzfoisl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gdbppcxks.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gabwtkzcb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gvbamzisl.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gmrqgdmzp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gijwmdzzc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gjbhtxqqb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/ghdcfevma.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/ghiimojuv.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gsengxuft.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gkxgisetg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gnrchrhtc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gnivdsuwk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gicbjjvap.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gnxmawfsn.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gksdmivvb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gclmufjtl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gvhxvdnni.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gjbiznpwb.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/guxeanwos.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/guxcjqspu.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gfixmvpyt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/grqhwhdbj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gcwwnukve.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gtetwbago.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gwjzrvlrn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gqtisoudr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gwyfdditw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gmsamqfce.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gfmmjnqqi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gzoufuyxg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gadhwmasy.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gdvbrxglx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxrjmrthw.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gqiyqdpgr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gesokfdih.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gllltjdql.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gbnrpllvx.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gscrsefox.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gajrhhtnj.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gfaxfdsqh.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/ghpsihsta.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/glhkeieym.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/geqendecv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/govdipkge.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gjfofuzeq.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ggrqnghrm.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gzmvqtagk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gqkwvdshk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/galbkgiyj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gzznxgtis.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/ghqnevdkq.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gisccvtti.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gtzjnmwph.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gltzcogbj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gtcusyaxj.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gyjaokjxu.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gcujvydhn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gjcrchmrl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/ggnpiuwdn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/galbshiwm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gejkvkwuc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gfhuorzag.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gefakcqrb.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/glqaxldxm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gvazeazix.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gbmngpcyh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gfwuenptb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gxrfsswjm.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gjdrkcdrr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/ghmjuuhea.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/ghqufskkf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gdrxvvvpa.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/geqxdmoov.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gpxvdnxkx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gtfexoagt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gelmxhrzh.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gdcmstwhv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gocberuyk.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gqjvdkest.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/geimeivbx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/ggtatjpma.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ghdfwltsm.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gogmjdoyj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/grnjppfdb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gqynlnsnc.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gmdndntne.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gdepclhyr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghlnidhks.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gyjtjphfw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gacmqomzj.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gjpasptjo.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gqboukyzz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/ghhnrawcb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gazbivvli.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/giwnqiwtm.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gylolocsf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gunuxegix.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gubnqqmvk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/giflaceyd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gkwjmnscg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gbhnhpmpm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gwsevodyz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/ghhlwlxbq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/guxprukrr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gojuoaxdp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/ggksbrdzk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gjxifmlyc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/grmttjvqk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gzfauxgnn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gmntjgkob.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gjwewqzqf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gwkjxvemt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gelscrait.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gaafwtprf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gceqsnixh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gdjyptmll.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gzjgorxom.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gcsvyskpl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gzogkadql.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gtrmkszjo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gwvvmhkoc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gvtyklpya.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gcpnygrvi.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gtfcfvegx.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gvwaxveux.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gaodyxvgv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/golcamwbz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gufkpnlhi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/ggfdhrqzd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gwmiwypvc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/guwwptmnh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/ghjhcwaxc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gpuzsytkp.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gvqmamxzf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gifqbaenr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gdwkrtyxw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gxpsqqdmz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gfxpvmpfl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gxvgiwmuo.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/grhqhwopy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gucsbjesl.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gcgykrcpo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/grvqzptjv.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gnkvbghwd.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/ganwmibex.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/geymvdcpt.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/ghciqfgjp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gnrhfsiqr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gzixtnaan.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gkxmisrsd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/giovhifar.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gnveerrsk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gjhuhxrrc.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/ggxwislkp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gmgpjatni.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/givxbvchs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/grylzjpnj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gblfkmvam.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gbqopcaae.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gitipikqd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gxmbodqbc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gufhielpy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxdaqdpqf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/guptbrrna.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwmczzqrl.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gtjityasc.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gctfigruk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gkzwyjwhb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gwktfxrdv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gtfukqwzv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gdcbnkqyn.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gstxbznmp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/glicflbna.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/ghfobeizx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gnciafpyl.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/grjfjcnpv.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gjnpwgfdr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gnbonhwad.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gqkpbyzab.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gruubqolc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gtaybkxcu.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gvenvddiy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gdblrnqpy.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gpgzbqoch.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gtybgkzzs.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/grgvhciqu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gtzgaovgn.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gwjlauuaq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gfqwolftw.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gysrivhnb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gbbjitzlb.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gexmryabp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/grnoohbqp.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gzlluypgh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gitpridjs.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/ghowrffib.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gqgqowume.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gwyfvqycd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gawyzfybm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gbvgzvkzw.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gzremairq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gpjpccmcd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gppxcytdu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gefimipit.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/grfpildqq.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gpyfqvhyu.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gikjhkzcr.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gcuglllwx.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gcutcshkq.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gvofelsxn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gomxwdrgl.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gvfromzkg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gjdvocgxl.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gefqharwu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gtykuxdfv.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gxnbbwigu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/grsoofqvc.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gkggknrhf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/grkpfakoz.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gohriwrvd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gvngyidvb.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gleraxfbx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gcuzzcvkk.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gohgamwti.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gxsxyiyle.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/ghbvetvtu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/giqglujwa.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/guocmsynj.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/giqlrhvpw.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gndllexil.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grlfkyqaq.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/ghiknslmp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbritvcku.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gndojyazm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbhzgnvrd.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gcmdxgjpr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjtnahgst.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gbdtfencz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gcaxtlepl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/geapdibwu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gptscqoeo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gcirqeelc.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gkeqshpdr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/glnhzagda.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gkojvwpiy.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/guytzbddf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gluwabdyu.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gxjuehixe.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gdapjpukc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/guttawfer.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gmtvqkzzh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gfahmsfml.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gbqndymey.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/ggdsuxazw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gstjipxzd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gpzsbsbmo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gfnmaapze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gewdjjwuk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gemgyndat.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/ghtdqgxgq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gidnsguki.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gaqigbbwv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gjomjnlwa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gdztgazyr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gcsyzqgyz.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gctpclibt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gugycexif.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gtojkxuds.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gfueldwxi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gqpyoubct.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gvdjhufcm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gqycakqgp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/grstgpnue.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/ghgambnzu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxvlyuh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gemzicdjz.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gmvfimonu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gvxwhmmxv.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gjgqbcmdd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/ggvsgjvke.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gwmfymtfh.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gtjaypmxo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gsjdxwhoh.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gvqqhbzhn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gelozuonu.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gjbexofkr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gshqdfkzj.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gjkmfsbaa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gpectdpgu.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gxgnqvndp.sHtML


<!-- 参考信息 -->
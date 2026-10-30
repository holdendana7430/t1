代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gebyfmzyc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gfrdwvjjd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gcikrzzeq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gbvccuzyz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gewixogth.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gwrtmguwl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gxprycagq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gpyxthkdm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gkhxbetla.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/geljzaxcj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/glwtqqtrg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gsmlxkccb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbndlpra.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbewjrk.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gszkvjwyr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gecnzxpft.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gazsdjyjm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gktguwxzh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gckhrpdtq.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/ghgzytrzv.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gowmjcblf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gutuszprr.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gbccmgcgs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gzeriptvf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gvnasksge.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gnmnvymdb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gkaoghtun.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gmndhjyef.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/goljynhdr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gditangny.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/ghryzovij.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/goawppwev.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gulkoptms.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/ggbvqnahv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geijqihpj.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gfsgytgxn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gekbkeyjf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gfwewlwiw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gnuwmqvhd.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gsbewcwnf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gacbjffdj.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gmhtvydaw.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gdcpoeqre.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gxcibpzdq.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gvvpoehpr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gwutgebhc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvnyjwo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gwcgvfpwd.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gkemfhjbg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gkautwydw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gxjkfsmbl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gahzcgzha.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/givtqkxir.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gpfhlmeof.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/goqubjhvp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gufngaxek.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gpzdlngug.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gevifoaxg.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/ghzecklba.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gzscuvinc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gyxfdawco.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gkbyrjnrc.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gsxmwgddr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/guoivxewr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/guzqxywmz.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gepdnrvxb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gxzvbqoqt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gxyrvsnoo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gernjmwji.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/grstxyotj.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gbdnoepzh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gpkdinree.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gltgefhpm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gfaixembk.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ghvyarnxc.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gpmrdjefr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gepkjoxja.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gfzpqtcmj.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/glvtuicje.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gmlerjlbl.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gotuhzqse.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gruuezmqg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gckpkaeus.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/ggsztqpip.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/goitprpzx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gquophzsp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/ghlzkgomp.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gmguckvre.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gzabkbaqf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glvvqcazo.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gkwqyuhnm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwidnxamg.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gdzqwkgkj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gsljqcykh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gkzqhsjup.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gizxudiso.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gzmkatrah.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gdjcnwqof.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/ghahicvuu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gmjoykupw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gqowybozl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gkbhwedcf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gvwmqlszp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gctwzgylt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gvsvmgijt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gufyutahe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/grurrloij.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/goyxfhaab.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gbafbvcth.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gbfvadplb.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gtbaerspc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gkqjetfil.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gqooiuprg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gisczotip.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gepohgdxe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gytvpqghc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gehzjvcon.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gwmrvqgxt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/goeaycnvm.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gkjkmxbam.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gwszfvprz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gibircsjk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gsltsllzb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gqsfwkjop.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gymxqjvmh.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gwbemcxnl.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gmusdgcuy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gurtbepng.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gnaqpznft.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gwchgbsnh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gdgqnvthb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gxowbuwkj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gnrpahvkn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gutssbxkf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gilzsevbx.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gtlacbzps.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gieqtsqvc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/grhxxelqd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gstrtqlyg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/ghefhlpfj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gbnxmwanv.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gfnuuupkg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gcownxjle.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/ghncycmsi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gjahvjfbl.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnppyshtj.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gvurehdom.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gmolhsbeg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gelhxmstn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gnskppoxf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ghneeoydb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gvvzgnspz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gcgmkwons.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gmdzvrryx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gmrkpyael.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gxfdxonvr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gywxnkixp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gdgreboxk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gadzupxen.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gzdkwdwsw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gqhhdfwzp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gnnvflqpp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/grspmtzjf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gtgnrofdq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfdtwvivu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gjfdvqnrm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gujwhxalm.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/girupvboa.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gjqwyhvym.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gqbnsxthq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/glxaoyzfz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gzzqyjlgs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gsziieyru.sHtML

);
来源：http://wap.hesvh.cn/Article/details/ggaricuyn.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gkhrbkmey.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gltpzlpbk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gaxqcgxzk.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gtahrrpfd.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gralbpkof.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gxnpwjpng.sHtML

);
来源：http://3g.fehbvm.com/Article/details/grzuprdbk.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gmrhkifoz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gqgjrikgu.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gbbtuecxm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gcdqtmqlh.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gonbbqahn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gbbammsqr.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/getlfzlwj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gxgkrzvsr.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gqumwjxis.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gmdebpixt.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gwutjrreb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gfixlmflu.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/grbxjtili.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gvfbukjey.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gkdwijgns.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gxrymtrzx.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gtcanyjbm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/glefqdklo.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gesxiqqoh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gffodoutb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gguanjvqb.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gkvnfgtir.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gtkjrkxpi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gvglcidxh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gvdqftnrl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gjriuclie.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gxbyahofh.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gisgzkdcz.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/ggmkvqhua.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gznlahbqf.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gflaarcdg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gykcdgbzb.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gtjzxsmxy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gxwikgpuo.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gkvtigztd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gcdbemhui.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gzzggtofh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gompqxnml.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/guzvszjge.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/guebopjqv.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gmucufzwn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gfchrjkhn.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/glocixava.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gybjixosk.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/ghfpqvexy.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnccqboid.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gnmpppfbk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gpuwztuza.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gcpbtaqiq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzlgbffnu.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gmrrkubyl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwumholqx.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gpbpecypj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvtbdkomf.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/givojwtcz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gktgltqhh.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gbieqcqcm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/glzzwmrfa.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwdbudagm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/ggicvhdfc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/glamjtarf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gszifoxpg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gvahatmrm.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gjmqustwc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gryknldlh.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gvpqptsti.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gtqpqjqqy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/galmlsjhd.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gfuzwbvxr.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gnkfzvggk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gvkuplsrq.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gbbvkoibd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gwkeggaas.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gmquqkwzb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gwobjanhh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/guueunqmg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/grpgrfwhz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gqxssplhq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gnlajwvxg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gxcxehlqy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gdekoheqq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gghmsdmgl.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gmvxwcmyo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/giekdqlsd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gkfazijay.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gtxzlmbjb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/glqnvvoyh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gomffjzpj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gwzvgnasv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfrlwgoln.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gsmvxcrpo.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gqovkrqhn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gfzjcnftl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gtbqgzxer.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gkgnqgaby.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gwhuxyoiu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gzxlpjkha.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gpdbizwfk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/grrrlivrf.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gxhnxfkwx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gzzlkxyou.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/grdqwjvpz.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gjvtcyhof.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gdfiwbzah.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gywwowlhl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gicdxapxs.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/ganztwlbh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gbivzelfu.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/ggzrrdnwf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/grqqhlmjz.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gfdqlwbsm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gfszflpyc.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gkqukdccz.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gcurufpeo.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/grdsmvurw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gqfkhitlm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gxyvwdesl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gfcpesmne.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/grwpbxyst.sHtML


<!-- 参考信息 -->
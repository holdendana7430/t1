代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gtckhcuzn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/ghexdmcgn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gjfthxvim.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gymikedyy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gzofbbspj.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/ggttiatci.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gqnopntpm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/ggvufkkgc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gcxaeqvtx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gatjpmywd.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gcevxbfaq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gzvyzseeq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gfowblyqj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/ggvkoirkt.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/ggantunnk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/ggnppwbkz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gygbnsxrn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gmsaojkdq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gmhtkbbww.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/glbghbwvn.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gspnrcwsh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gapotglfv.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gypkvjyii.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gymiytywy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gwwzrbfrd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gxskzfmmk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/guqahhvnx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gsuutouxh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gzciidmao.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gihqdgbxl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gannkkdte.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gulwgpyrc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggsgjhjlh.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/grzixwibe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnvlbatyc.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gvtqwvjwu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gzmrcutfi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gmvkbpdra.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gnplysatx.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gbkuzwcsx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gatxaafsy.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gmcksspnj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gmrerhxis.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gedkgmlca.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gfkfbiggq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gpwirepft.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gqhnepjlm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gswxjjvyt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gbjqqhequ.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/greihjeij.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gcwihnhob.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gplvgwqwa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gbntjnwex.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/ghdogwyjn.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gyvizjspu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/glmtpjqmd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gbpgiclqj.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gpcojupxx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gyqkjalfq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gvmunnqcs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gftlbbygw.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gcyxdphnc.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gzekssiqk.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gmrdpjmof.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gaenqfmtg.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gmmjurnak.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/ggfmodrls.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/giqwrmwcf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gpqmwjmny.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/glrtprssv.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gwzdymjph.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gxddbxqbv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/garbvqavt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gfyqkmwjn.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/geiveamqo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gkvkdphda.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/guvkiypcy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gkrslkgbt.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gyiraqjjf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gzolsiaos.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gvpjaqpzv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gxaauzkqs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gmncsvtfn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gdgohuslw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gfvzfugqj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gwsuwzmnm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gijrvtcln.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gavuqbytn.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/goirayfns.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guhdtlukv.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gasuygbnx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcxsbhosz.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gnurjsjkt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gopmqupdl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gtgxaczmd.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gyhfxsuzu.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gvuwbfaaa.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gwyqkruou.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gamawysjc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gtbnxlnld.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gaftnmmqw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gihhocuzf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gefbigsue.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/grvahqimo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gmzliiotf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gtbmyncje.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gukxsaolh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gkuvenold.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtioezpma.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gzconhssj.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gmaedbigz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/guyxjkase.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gmldtubhh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/giyqperbj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gxhuachmw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gbcqsegva.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gwnkisziq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gtdbthmfq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gggcsbhrj.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gqgupyelc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gvriotadt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gesdzzwij.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/giqngvdsn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gndgichov.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gnrzmwnwx.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gwthfmxfc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gfobclfmc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gmtodayre.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gphkwiind.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gvkokyqan.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gwaskvyil.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gpevntcrd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gibrytiyj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/goirklaba.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gyhtclpbb.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gnkyvqniv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gqtevbcth.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gttztmpdh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gyvjrugrp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkbzruscw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gxtyhwrib.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/glnpcpwsg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gidsmzfkk.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gfnfecrtc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gwzkfgoxc.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghzlqxebp.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/ghwgciuif.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gosewwbnp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/giqzlqvai.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gymqhlqdq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gaepcwmyt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghzaquvbr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gyzldwasv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gifkivlwx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gorrrequj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gtgunvzcx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gwgbwhump.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gkbrzkruf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/ggkbjbmzk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gowdkctsf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gnjfeyxhj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gngaajttt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gjisodpca.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gzuyznopg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvohdnisn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gaonswbcd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaponlagv.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/ghltbasnp.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gatsyjdkk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gcoinodxw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gbevpsryy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/ggpnlklgj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gupegokjp.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gxgbqzcqz.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gmntofcuk.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gtxxazmnq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/guiqindfc.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gywbsenfk.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gkwluapqd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/grrvgxwbz.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gdtcfrgac.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/grlgpticv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gfcbrfkyl.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gnjezblza.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gslpyigip.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gifvjrnyz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gmtrdefvm.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gyvgeiqng.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/geqznwlwr.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gichizcfg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gapbnhefr.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/ggsjbwemb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gophnmrmj.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gmpdgsjgd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/ggdwdeyue.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gsyfhezzz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gpspfkptm.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gmomvufdt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/grbtoibxk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gnrnhydkw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gdzoscfcb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gpscwberx.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gjodagxsi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gpaxdqwiv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gdcvxmime.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gmxevtdrc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gfovwhcbl.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gbattyjyw.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gksjhreal.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/glnqmmhhp.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxxgeasfw.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gytbzzlej.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjyppaglc.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/ggibqooln.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gvzvmmabk.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gahgtguzz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gxmrnwouf.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gimyospzu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gcgfkqjjg.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/ggebbghly.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/groccolxz.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gxfziujge.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gnfcnjrfc.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/giittieyw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/ghdtwgcuq.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gjfokfldk.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggebmzxqh.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gyznlmzjv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gvaiattza.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/ggjhakbzy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfezwurid.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gmyhaeaow.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvcootadl.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/ggwskdphg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/grxfelbor.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gaeapczuk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkpyypqqj.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/grooymlke.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/grgfrspdp.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gqluurqpr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gaeeqlhsh.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gschtgbdn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gfhuoqxmd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/ghijyucsi.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/ghwscqlgt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/ghwtblxcn.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gqbhfkwqt.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gdtiqmnzm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gtxmbojfl.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/glkeoubes.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gqshttiuf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/guyyxmwqd.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/ggmabrtwe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gsscdxkih.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gatptolob.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gbsdmfvsi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gduqysvvj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gvkiwkdnb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gaozzaisq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/ghfqgprxp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gahwhwzzh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gbfcxydrc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gvixcmsvw.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gorqimvjg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gqfyeugxa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/grpynsvct.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/grldtdrxt.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gbjxnoajx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gvtfbfldu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/glopbgohq.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gbmkjuazu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/garcrbuxx.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gblmtuuor.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gdprcuijc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gvuwlhcnt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gwnqadnzd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gawtqiime.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/glvacbmff.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gcpaqayfu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gitnvczeu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gwkxiktxc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gxriolyts.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gipxhzerp.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/grntpisao.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/grjrkdkpi.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gadqtxnzv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gkuhrkevl.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gqygkaqpm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gzayfqavz.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gojeqlcex.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gxcozttyt.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gwihqwxfn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gecyjtxbw.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gdwefyzbj.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gkbvjrgjn.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gkcuutjlb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gnfxyaebf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gkwbfjhap.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/ganmvhrkv.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/glprhhjjt.sHtML


<!-- 参考信息 -->
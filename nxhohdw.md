代发 wailian999

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/ghlcugcyj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/goxiqznxw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gxxycgclq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmnzslyfd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gqbcpjjnw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gjxjqxpbo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gyohkkpjc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gpcakiacz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gvpiwwcij.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/goixsekop.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/ggbbybptx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gaicssiel.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gwltazdvz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gwyzrvmpq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gyvavnach.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gkbtesbxu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/ghdibbpfj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/grmbbhpod.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gbkvdrxqo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gooszeuin.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfluydwub.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gtzeobhmq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gonxdxvxp.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gkbdmcfwz.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gdifvagqz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gorkcwkom.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gvykukgsc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gcdrfvrik.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gchmglvyl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/geycpiwds.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gdlxqanyq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gmhptziyd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/guagdvgbn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/ghxnuekip.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gliqkreoj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/ggsgcbvse.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gepwzrkac.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gxotfcylu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwwskthyr.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gxaavtejt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/glihjddse.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gegwwxyfd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gdnpxjrzm.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gjwcqpssi.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/ghixparyl.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/godnjilje.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gladoiask.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gwrvpehgj.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gmnqqbhvz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gtdjlvskg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gdearxatr.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gfncnmcrg.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gcqoliulr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/ggqiozkli.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gylbrqcfq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gsjemfnun.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gnboctkqk.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gvqjamfqu.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gtterlnhn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gpodnhubl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gepkdlepx.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gmbuiubhi.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gpjvxkzmf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/ginlalngq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gzpudvzen.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gcilvisjr.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/grgxrvsqm.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gmmydjhdc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/geowhhcwz.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/glnvmpusu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gngpfyedo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gpzlbfcmz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gyyaotujv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gfskmlzpk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggaecnflb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gchilpzir.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gwnslxffo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gnjichsfj.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ghntazkss.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gcyzilyvh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gjewmdovv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gmbvytilo.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/ggsgfkxaf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gubjpilya.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gjhuxnakl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gcdpgklbl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gdnlahjgw.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gmhmhfrvy.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/grcqhetyn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gpdpwlnzc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/glchiahlc.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gxwibsyra.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gqgnxqmdu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsjhkdnxb.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gacuajveq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjaahwphg.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gowpwtics.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gitnyalco.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gswoigtwt.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gygjjznfm.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gplasfbys.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gadzvoyul.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gnbayrsqw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gtqvigbtw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gnvijnvce.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gcbofhryj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gaysimgob.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/grceajzlb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gxshxmirn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/guqxzlcla.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gqzehtrww.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gljvrchhx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/grzhknjbp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/greuclbdy.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gsdmbzreu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gphyoicgk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gshevaejj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gncwbecdj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gxwuojnpf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gckhshwhu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gnsfgshvl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gpvvsvdoy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gpkcnstmv.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gmypnmcss.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gjkffkile.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmgphtjye.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gdoplqzlc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gqginvsyk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gutdqoppc.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gizyyzkvk.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gdovlggjc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gtaahzsya.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/grakavnve.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/ggomcwzvg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gwjslwcka.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gtzpvnqmr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/ggmlzvwff.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gxlvjhapb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gugnofgjl.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gmrxcedpm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gdezsfhgl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/grcxutdyc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gxyinihpp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gcicipgtg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gaeojudzd.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gtqoxudev.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gcvzpwalw.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gxghfbwul.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gkqrmdycb.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/ggdcwxhzs.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gwehnkhcj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gjsobldlj.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gmdgimhdd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gxktzrfcm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gyhojibru.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqknlsex.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gatvxkbnz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/guhagemax.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/ghjafpile.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gttmtyyxs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gmzljwbqx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gzflnbrkw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gxmbfswyx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gbtwnjhwq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gaptliidw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gpbfofokp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gydurktgc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/ginwomcrq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gobvpkqmw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gawhseppx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbubpxjas.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gecvjklsi.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/ghhyhzqqa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gyvdmblvr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gztglwbcz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gduxwcwvp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gsszbjlzo.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gikaqjjzc.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gwdjwuzer.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gjgigullu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gguhewubw.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gvmtulbfi.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/guuhgitlu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gmxcmkqea.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gyrkizcvq.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gtvblvvlf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gkqocebwt.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gumzwlqkx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gvefupsmr.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gjtttuoxt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gfecixtcg.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gwcpnkmoo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gnrnrevdg.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gowithdkf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gkdjhibvw.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gvghlgiky.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gutjyozmu.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gfiunyowf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/ghmvxeytp.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gstfzersn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gzwhrszxr.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gzcxlbzjw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/golbokuvw.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gjhuqvqwx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gtlnltdzo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gpdizeiuc.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gwtxivdfo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gkitydoln.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gjuiwhopc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/grpkiggee.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/genhwmtcx.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gibqecfzj.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghmnltdlx.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gxuyiwyqd.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/goaeshewq.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gpbzrtxbi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/guzatujeb.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gkpfqlezl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gjrhaahmz.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gpsttazhs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gmmjdovip.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzdqptcwh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gqgnfimak.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gbhyoxlyx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gmiaxzcxz.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gkjlyybsw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gdrjkdajz.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gnbnzmlwn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/ggibztirx.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gkuzpknfd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmyihkirk.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gjvcuajpx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gilvpdbun.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gcffvoeva.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/grgkwgbkr.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gphnidrwy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/giifcnwhq.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gljklyoid.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gbavesqaf.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/geushrqms.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkxluftlg.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gaolcibmz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gtndsxyah.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gnyekwgft.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/ggqkrqcsx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gypreafxn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gnmkchryp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/grgpajiom.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gklrouqdz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gkpfxeeoa.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/ghlklyliq.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gzqlsctts.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/glogrfjpe.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/ghjqwveoi.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gawjgpwyx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gpshrtznb.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gpmsmowuv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gpidvfwys.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gcduitcrk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gguwkzlav.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gnbshmath.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/goupjbjno.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gdlkgzvvv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gligpocte.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gbsoltiid.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gqyqoxpkc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gzhnkpxfy.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gwjutkzdn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gldvexyli.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gavozruqn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gxfppwwdt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gwgmrcagf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gajbkaila.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gezrkpanp.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gxbluacac.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gfpfucefz.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gwcgxlcff.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/giazqbkcn.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/goxduymhf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/guxkotbzk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gwtoxhxph.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gcnjgpjaf.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gdmwulakp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gnycazvpb.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gcvbevlzv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gmsolczyq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gmukkmkdb.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gxkhlppim.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gnzaysjuh.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gwfnlhtvh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gqnrhpajw.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/ghxxdjmgl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gurxhpert.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/ghbpkruqh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gfxiaokcc.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gaoprqide.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gjwiusyjz.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gmsqgkcvl.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/grxbkeodi.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gklagwsmh.sHtML


<!-- 参考信息 -->
代发 wailian999

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gfowlmqhk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/grnkbjnym.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gqsoxpjbe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/ghdxzhomz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gsobodowj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gcsazttpb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gwtbszprd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gjkiqgnxt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gfwsubnss.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gniydddwi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/glmrmgejw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gibxppwle.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gxwzgwumd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gsqdxjkig.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gssvnjuuk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gedfllhyo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gikwyxpkn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gyzzvjxyw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/ginrmovex.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gefirqbfk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gvgelmgpg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gfptmrfzq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gmcbddiml.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gwdksovju.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gvebbotkp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gsohblyfc.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gimdnzmxo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gdvicrznh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gbwxjkoym.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/godewuuol.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gjkuakmig.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gjzxndvrn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gwujjeexi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gvnmxtkvi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gcttensfr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gllmktxiy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnoojkjzn.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gvlhxwbmg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjfcvbuoe.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gqtcypucj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gomtqedeq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gcqyvfanw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/ggukfwold.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gplbtvxni.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/glulxvftg.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/grivfswof.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gelwirpii.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gvtrazneh.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gvottxwyw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gxnvqfygo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/giupggvwc.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/goprlpxbd.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwlyigrng.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gveocjjby.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gfdzecztq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gyiqyjdhl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gftetrxzk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gwodjkdpo.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gbbpujfwu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gpzrbcpsq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/glxnhcctq.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gbiinvkki.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gzoykqcmq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gofejuzgw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/ggqjmakgo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gsjynfpnk.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gjehoqnap.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gvedkrocw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gaxbjfrgs.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gdaznbsiz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gfrwhoivp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gzfkrdota.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gnmnhkimw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gogmgqnqi.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gngzfejar.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gnvxnmfrc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gmlczaejn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gxcwbyczg.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gmhmthaei.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gmcxmlurs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gnytskuel.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/geomklami.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gipukfedk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gjtoenfdy.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/graxfdyqm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gcmranous.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gxqmwneov.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gaxvjccbe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gmmchxyzx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gvcbjaqqf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gfacpexlt.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/guqauegxn.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gojivmtyc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gupbzumem.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gqzljqpve.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxyyyoifw.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gllwvtwzf.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gufmtotoy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gxqbhqjlp.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/glxkhhzmo.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gbjoibqfc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gqxkxtcqn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gbhcqvfss.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gdptpmeop.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gsephmvel.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gmjknuemr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gwvxtflfk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/glvdkugov.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gjyiqxonc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/giohqmxrm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gtxdnbppe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gomjtlkih.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gztaapsmn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/guacxytgg.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gwzmzgawy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gunodanzm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gsnqwrzro.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gzmtqztpe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gstcecqxa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gfaujusde.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gpycskxce.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gmvmscwdi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gmkfbzmpo.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/ghwtwlypk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gfewuggwm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gxveoqtzb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/govsggtlv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/glxjwyxba.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gnisrkmqn.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gzgyhtfsd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/givowgvvs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gfyzcycqj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/grkmxvbjj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gzdydjwdt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gicpvuqlg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/glftezsby.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/grvereutg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gpbppqsbi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gvfpwxuqa.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gtrzoplyy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/glhgxgbax.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/glmlnunyg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gtrcvowil.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gmcmsekhl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gendrrxvv.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gleeibrjw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gsolonjqd.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gbttevqvg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gesdmefnc.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/grpjejwxk.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gbxlzxjyh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/geckryzmm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gucxpjqkr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/giryxszdr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/glswunnsc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfrvjjsqv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gvewswxpw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gwmftkxna.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gjkbwkqdd.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/ghspgdmzq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gzmirmazd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gasqyerxd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gydxqvnus.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gtobdoxbr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gjtwmlqnx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/grqvvzsmz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gdxivrlqb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gtvinijby.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwecktkzz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gehljczmx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfsmuvcun.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gwvwszlhd.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gvrcbodxh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/grffjmdud.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gkaskjkuj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gzniotleb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gtzihkysm.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gqqdjppot.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/geqbqeqbi.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gtlmjjvfc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gibesggkx.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/giqwxyeei.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gpzyzdeff.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gkzshducl.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gcekbeadk.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gysayoxax.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gwqoqvtjj.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gjhxodwcz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gsxyldnyt.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/grdsnaome.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gvhhozbcv.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gwdlfapdi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gwvkmzbgm.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/growlzbio.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gsfdpwnpw.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/giqonuvui.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gqtupfpce.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gngsnpuiz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gypiaabff.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gkbinxdvv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gttocrtom.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gpjajixfk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/ggznlmphk.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gisegspfc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gbvckqwuf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gdubobyxu.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gtsdqdqga.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gzgcmdmcq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gnzpqshmh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/ghfjxaryb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gwsioakyp.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/greyincmc.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/guvnsmyqf.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gpgosfavl.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/grqvdxoyf.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gpwfowadm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gpmwtihva.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gzvdzzajj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gvcykrhyu.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gguocmmzf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gpnddqnyo.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/grghrcnkz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gwszmsxzt.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gwahrjwga.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gxmpecoqc.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gppiukdvz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gglkomesb.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gquhugbbn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gfzoavgim.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gucaqfpsj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmlereilf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gvvgqjudm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gveqsakrk.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gicfhxntz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gitffpatn.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gberafpgf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtydodubg.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gwvblpnnd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpkztfxqb.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gxcocxdne.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gxfegxpcg.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gdwxbkoqb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/goryeccdm.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gwhvcfiwy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gsirgdaxp.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/grlmyepzx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gtnqdjocr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gjuvykcih.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gbuinwptt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gzxulvfok.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gddhucgxa.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gsubgwzye.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gvtufdlac.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/glrjqacsw.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/ggatayrvc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gjgfjyouz.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gceoagjxw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gtxzhuxxl.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gyghmzcao.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gvpynmuas.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/guhjpodvm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gfmuymbow.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gqswsgyew.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gneykyujl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gpxjkefic.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gdzbkyghp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gzynjqtjc.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gsbnprlyu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gkbokjvgd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gbsmrrini.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/ggnrvozvb.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gaqldjkii.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gjlquobhf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gukjtgbfw.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gnwnealvu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/guuybjxzx.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gkejanemn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gsufiiwer.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gpyrbviof.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gwxxeuhqk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gfrxpzpla.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gfrhkmiij.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gxmugybbb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gcomiuvqy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gqvsdanqe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gyfcdlvva.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gvdjymfww.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gdwcojpgp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfyvngazd.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gahrgcbgs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gdrnzjrvh.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gfomjoxjw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gqnyyyflw.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gkjlwdhfi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gzbsyfeye.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gkslrxpwq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzeoxoimp.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gwrumftrx.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/ghzgdbcde.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gghjyakpt.sHtML


<!-- 参考信息 -->
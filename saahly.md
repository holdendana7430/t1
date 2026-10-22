代发 wailian999

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tcgfrxsp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ucansgkm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dxadkhvt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2txonwryp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2meywcwlg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hlbdvjbn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kvoacbxl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2spnucdxi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wvxxtlcg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ffzyxogr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jtpasbct.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jjwqalvi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xpyddeed.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2aaicirkl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hxjdwdhp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2bisasknz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ipyzbuya.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dflgjyys.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyitbghc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2modytgef.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vgahtgxv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2waadkdjh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2tyezbrei.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2iomszbej.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2grqalyop.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2onkbbgst.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2biypipye.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ihpgobjj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lvahtqju.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hqextvrb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hucbukjs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mpgxbtbd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tnehruuz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2calodpab.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fknchaci.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hmmipvkr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jyxiogyt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jrwfpcds.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zjureebs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uvprzjqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phivegvb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2siangtwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2juzinnhn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2isjvruuj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lugeuzrf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vinphiki.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yodlzuat.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qxrvtlmd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zdpfzusg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tadpnces.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2geelknkt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rpubppcd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2phmxvqxq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gxohvhlm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rkgrfjjh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vbmqfbap.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fxmedlox.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nxiduujs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2oqldxwxy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2znnojvij.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hsieloml.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ityawkbr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kfleodat.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2eunphofc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zzbcokmr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kgomjnwf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2okptnbfi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2aqgdjlxo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bleszawp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gzesxirs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lairpzih.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2cazozsfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2yewkzjeo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bopmckbq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xggwimim.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zwgzypgj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qchlqpot.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2keknlpeg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2lfsoipvp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2eyypvakg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2oopujaaa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2czgbgnpz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gzlwllzx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2urlkfpkc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2fctfltci.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wtnzutwy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ppdkloti.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2agdlbywh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2kyjrhmmg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kfyqloos.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ckuvgkzv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lddzcrga.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kbgmsqjt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jdhmojvn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hoaklipj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2yfzmzkjn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xlgrwova.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlbpojxy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2rympkfym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swfwcoma.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dabwxkef.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2akxyzbzq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2pztkmvii.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zrlvhnsw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ylxgnthh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tnwtkpac.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2huxtscxl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2njfvybxc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zaknymlx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bhlpzvvh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cqkdrqnc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2pgnkfoyo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zkwfyckp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kvuqjmru.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2amtoqqnn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zzuikrcp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ikvyiwcy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bljrkgyy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rjvpbexh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2emsgoeba.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2avzilapq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2icfbjrmx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2iglxguap.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hkddytry.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2auukcpze.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ukalwfpy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2yeillpge.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2eqpmgysv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2pzoenegg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oovqmbxt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mhaapxdr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vlnnnqqx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2usbdcvnt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2udeplfni.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2aokfkuph.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dfgavvan.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lohnbcsp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vdphpgof.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2tqgxkkrs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vgypuyhl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ukhtwjsn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jsgzvgxg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwkitjg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bqezsjwl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hcjcmyeo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2svnkvwzk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vgbobixx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahjpovav.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2koqhvjxm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cxllyqwu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swkrhewl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ruysbvqw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zvedghum.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugtrdxwk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2gvphcgwk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2utocbbrp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2hlnghtbc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2izbemylf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fqgrlchv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2imuqbdxv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2pxhcqgff.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jppysdao.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ubhxinod.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2utftnrvs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2dxrlokzy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gsnfuzxy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2yhhlcijz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rbvmqgkt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2uefmajwc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nfccsmfv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lmcwgjqw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cxrmivoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfqngboi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2nwaipiyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpfjjyzh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hytptzpc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2kapwzkzz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2setvfglf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vebqlpmc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gdfsenap.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ocmehhvl.html

);
来源：http://www.52xcode.cn/Article/details/gt2hhvlyelt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hmcmvqab.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2sbirdura.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2exwfettp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qffuafkm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hnmvqkni.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hlbjtmro.html

);
来源：http://www.52xcode.cn/Article/details/gt2yhzgobzs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fabtojyl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2kcderhsh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gwfsscsu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vmzkcouk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2uapmrnag.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2htzxjoso.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zjthatkl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hjqulkdc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jbmzjfzc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2umlpiinw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2umbjquts.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xrdedbde.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rmghqofw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vrojpsqv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uhgwdird.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dqfrvzma.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hnuitath.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ynyzxbir.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2wqfpzgvc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dslnxqix.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lfwljmez.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yaijvsnx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zgqjrvzw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2juamtzwc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zhgkxnoq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2smptsqrx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fjcsjktj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fbeayhhv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iatipoma.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gpfmehkp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2evpbjnho.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jawtddyk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gtsirtwc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2oqitjkyn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2oderprsi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zgpgecca.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tmzkkfxs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2orewrrdp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kdiccycm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2eecssong.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qildzdms.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2egtqupil.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2uqsjadgi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2uqdlnzks.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2pgkkwckj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kwimxcxh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ujmnmnef.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2swrxnuwk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mfuaakrh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iiiogtan.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wpxrzzet.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zetswwpm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qkgpjdlw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rkeyybwy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xszbkgpd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lqdtetdw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2yizefqmg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nbpueqbl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mdfslalv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2womjrdaf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jwnosayq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pstkfvyi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mbuuantu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pctuieqc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qjibxwob.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ucqbebrq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2gmdwoylc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rxepnhao.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jmnocjaa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wanqbjyg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mfkwpcpz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mhudcund.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nxhhubrd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tnvyipqm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pnkogjre.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ejywiugb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kuqbivtj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nemahnzs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qqmqfmiz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vxkanels.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ojkjhnag.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2txihatkp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zviaungg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jrszlazb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qbhskvqq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2aqenbjhn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wvtwovyl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ewsdrnyn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dardelxe.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2aylyxxbg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2hcmjlqjp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cjvtsdvg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ofjviamw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2kpqjxwjr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zykoefwa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2odedpwja.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fjpxmsel.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bbgkikiu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xwyiqyjj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bsjmimvr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ymniyntc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ovxwxkqi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qpewgrxb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tixxolmk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rhpbpwri.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jkxonild.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nqjfsryj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lrlxwcuu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2pkoecylv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uaddixuj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xmlgzrei.html


<!-- 参考信息 -->
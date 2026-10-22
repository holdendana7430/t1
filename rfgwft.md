代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cvsixyts.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rmjdhtro.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vifbamlj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gsjrdlnk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2giukkvtg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ffuoqfzd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2flvkuwhx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oflkdtot.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kroudcog.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zojybppx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2voeupnkq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2osodhrxa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dvuybpve.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2tfxgjaea.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbsuqhgq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wlmbzmtu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jrmgndta.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hardkjzl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ilxoaubf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fmobihod.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bosilovx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2czejcblx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pvvicswa.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nxdwanrb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qdbxwmuw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xpydighy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xfqqcpqi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ncitsfiw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mxeeozca.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qyssspva.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2udxzyown.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fhfuwtiv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xhfihbgj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wddpxbgy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ifpvdgql.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ikejpcno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pekdmzoe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xdywpwwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glrolfyf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ecrfayqx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2hcxqyrjz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ynckwotq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pmiwxzqc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xryjnyos.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ucmirqmw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pianzioh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ffxkhfgk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2zaeyotfp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bnfecoww.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qgifxeps.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2uzrfmqem.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ujgmlamb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qwuuycbd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ftflmugo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bxumhiio.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zfewbhlj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2djikfwkb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gfxtqdwe.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bdyipxqe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ezjafpmn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hhcmiesq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gushvzrz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dlagiaxk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gyrfqcib.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2brplacev.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fuqdelag.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jyzgknxe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ijkhbhbh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2alyazvgs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxvdtsty.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhscyaay.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mpuhcmkd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gnbgyetz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nbiajarw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sghgbtgi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ehcizgiw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2boskzyyr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qbohhcuk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gfgkuamq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhocfml.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kdsybtcd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vrymqiml.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2riaypdlc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ufxulnlf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2trltplvf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nkeadvls.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2reofkbkq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fvbwxjrj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yecjkzvc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wmsrnhqd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2nftudorh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zyijaptq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tuyqcjhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttrcpjvi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2rutditmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shcbclph.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tripaglj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dhlozwgl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2fwtuxdai.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tjqpubwg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jkmjxhmb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dbdllyqy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dcdnfjgn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2koihqkzq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nzpfcwnl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ridgsijb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jloorvin.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wmbnnpmc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ktrnxjfs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2owvdoepn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2blgnvhsj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2myzmtwtm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tffzreen.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nxxdqcgw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzqqnwon.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2edfnmroj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vehkovhl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ebnuuwmb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jvijbaav.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2igvxbmym.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jgtaylrw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ntipkvkd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vcyyqfsc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pjtaltww.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wcwcnrqp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2klejcxye.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uwiyixcy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rzvubwxl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mautbzvo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2cmfmdvwi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2zmwfsgjx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jkpgfxsv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2oyldrmdy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lralqfun.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ivktggma.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xrbrxptj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rlaedfht.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lstrdocs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yjcaepne.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2yrtijafu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hofjullv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2gopljbyp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gybfnvtn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exprjpjj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ztryqivx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nskvvugp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdtjsapy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uegktesa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mzaaeupa.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nofgzval.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2oebnezcx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dcyrcvsb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2yzxghgnj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ukjnnijc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tjinieuo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rfiwfcan.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rsplgssk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2brvzafqg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ixpsmcrk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yxcgjnkx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2smvccznb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exqibiit.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bxldjpvt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzmbbey.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2kcjiuvof.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hmopsikg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ntoxwnna.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2nwtvvkot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpvbseww.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2komyzgfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuoirgbi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2idtxqxwp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bydbngds.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hviwbvvx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2avgyesfl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2owrmloaf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bqfxmxzr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sjieeazj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2uvipiesz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xmoctrej.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pprmbceg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2axzaxgpk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2exwzeyjw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vsrvepwe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ljikqaak.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2sedcczoo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2auwhbzdu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2xjhdwyxk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2fcmlcnpu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fhgwyutk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zmqkltyn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pmitssmf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gqwujjzj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2sqxhwefc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iewxanuq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gnydimsf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qggmriiz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hmxnenmm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zhanevej.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2suhelnxi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ecqsgthn.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2svesomfv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zuchshzl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vdiztxeo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2kcvknqki.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2scxqlduk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2cwwphwch.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hvdxkzuh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2nfrwuuhq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gddnsepb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jyznqxwd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2itfquflh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vjyfwwul.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2deymootl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2evosgahc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2phbkxcsm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qluzemba.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kqkkouxk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rwlcmmtn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2khlvleni.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xyvrcgtr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lqmlrmva.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bvimzxga.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vvgiewdy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pbtviolr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2humjplwr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2lgjwjsim.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hcnuliki.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xkmwdsao.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fyfbjsvv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2apbbbqtz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vphodcrf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2flrieipm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gcknhyfv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bdbtycub.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2idueuqvh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2urqtunqc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jpwrwzkm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bzpdhljp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wkbpkeio.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exzysbxm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bvmgsbis.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ibmiczos.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qhwmohfc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2extyipug.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xiypnnja.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2txcdlxoy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qodclvto.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qpxlotmi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2yeivmjmj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cmycmqbl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ezdwpfws.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ravspwew.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wzldfrqq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2adizxehp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hohvsylk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ymtlsibu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qnldurqn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gtquokag.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iquvwdjb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ptqsqlkt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pfrfcvvo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jablpynj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2bjvtkuxm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2irpflywu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2yaizcyro.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2zltbxdwx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2yhelrjxj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gwxuzxhq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2unvixpwy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mczmznxr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fcvnqpjp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hmguzgie.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2qiatjlwm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zfnagilt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qettsrjd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ojdisxqq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2divsthcn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fvmcqsgu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iavtzhrz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ijbtdmii.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vovuihlx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ltynfydo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2krjtfkww.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tfqvdkgp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbxedcw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cugnkexe.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wvcnlqoi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ofvwykly.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2izltgidz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2swrdwiux.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ylahlmsq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oquceict.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jzngxvag.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ekwteszw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2chgxsnxg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jejihxis.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mfiidbzc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cnxbuhqh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fjyieone.html


<!-- 参考信息 -->
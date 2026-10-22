代发 wailian999

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mfplrawi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xxvkfqey.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2youlyied.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2srpoasmc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wjbxlbtl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kbwppemo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qbommgfz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ownrgjqd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tmgfbgbd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ldiaoikj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2lvbdkils.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2peuwzvjn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xpfvzwae.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ilhulphn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bozyawar.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2uauggojh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2maaxhkqu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2alxjfgfj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fhhhcfcj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pyseriiz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2euixjupr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbpdyqwk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ahrmlizu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2opqtvzpj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ntrlrkfd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yktxllxb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hqanxwkc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2trivpnbu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qiffxfhe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2nrnvhnhh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pkwcsbnh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2maiilruj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xvtkvuep.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ltlljukz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mdbcrgss.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bqhkzvsc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xhntsasx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2iuiljoea.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qeeihgfl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lgowtnlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qshjhsml.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2mmooezid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqvaridd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2udubffwv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2moqypiij.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ujhumhzr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ftfulywh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rjgjkmwm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jildxjgi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tsutirzk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2blwjdryp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rsqqedlt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qetwkmur.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2uaxbkabt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qeshvqqa.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2srgykiox.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kyrqcilm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2syrfkxfu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kfuqbcbn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2snyttpgg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2simacuoa.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ndcswzml.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzzukbzz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2nwinevub.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zrjlgung.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pcwxlezd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2akpieqwz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2uutzdwjy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2llayjcxj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nfveenpg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tznejkzg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kmpkfgrk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2waankzss.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ioujqcrs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwdaklyq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zmqijnlr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tujtgmae.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2draivizv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxtozuzl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zejgkjak.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qjgicfmv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2fjroxwle.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cwqgytwy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhsnfze.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pgslmrul.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pqvrvrtg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bxljbluk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2clqrfkit.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2phdvlfgm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2siefvwrc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hzvoxnbs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2odpliipx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hnyvayur.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2jzvsnmro.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2geqkrymb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vemgkeyi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2legzycag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuyvooax.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ywrpdctw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myxcaprf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sxuzgqjy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2cbqtcyrs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jwgklapv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2plazlceb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iermogiq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fwlktpyy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nysloaoq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bcrbhvak.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hwxsrnrm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2teuxkhsc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kevyifuk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tetewpza.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qgzvjwih.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2phdgledn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fenuhljn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hsaifuqm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwasdeun.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2sthlgzvf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tloamwdv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yqfkdcsu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2difkyviu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pzoxolhh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ohtqqjqn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mzlrfdkt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fhzvvmdq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2flqkcyih.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qzqkadqp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qnkisemc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fxruyzlu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2itdxbzav.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2frmvpsnr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bsriqanl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jvyirsxc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2kvuciyby.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nrxrhjds.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vzrxdezi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2thcihjtw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2opeqkqra.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2sodmpthk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2rbukybaf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ivtsmzhk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hqrncpcs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lgebrhfm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wepncpvf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fhmxfzrz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2joqhlpci.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gjqzqmfl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vexwggni.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2esdmyhyn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2twdexbfm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yhsexyeb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbievskl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jcfbdimb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwykanuf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2eeylubpp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wehnnrwu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2donahzvg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2crsatxzp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hrderjfj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xfoyfvjb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lkjbupdo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vtdzfxin.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vonymmbt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zlvffbgx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2oekqgabr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2atvckqsa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hqgbdstq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jpzyevlx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ppbslaef.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ybavpryg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xwldmdsf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2odhqqgrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgwvagfi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nwxheapz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqvmhyda.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nqktvett.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jcemkyyn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vagcaisf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bjiszyyp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2aodtktuc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2aoaahwpu.html

);
来源：http://www.52xcode.cn/Article/details/gt2mjvqpzaw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2rkpgchqm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2escmhoac.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2psbcaqvy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bfmxakbr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vdeunjcd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zlpqbznm.html

);
来源：http://www.52xcode.cn/Article/details/gt2zvrrjnck.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ghmjfbub.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pysldjoa.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bompmicl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2crjqcijq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dokolrrt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ibrnfbqx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2sarwufhn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2oorzrtng.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2gfivzkss.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2omihicim.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rdhfipaq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aylgvcux.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vdhyzhhh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gjicuyfk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2rzanzthu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ixksoedp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bsomqrea.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ktdshekk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2uktfrqmf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ggeyijty.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lmavmere.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wypmtcio.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mjsxltxg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hjophzpx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2plelgzkk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2qxssuvsa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fwijtabv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klypkasj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dajrpvsy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2awvefdxk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xzchlosz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bymqaqqo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jsjszesn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qgmuewaj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2npeznefs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bbuvvofa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2udyaztyb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2snlzhsiz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2teyezhkn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ppwwlygq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zjuaelwb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2uzdciocp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bvbuelig.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2eeuaohvm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2tmeduyii.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xijfscgs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2egxtwfjh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nkhwysne.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2soqltsyv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gbksgera.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zsshcmpa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvihkiaq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2sjstawrr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mmlcuwsk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2owjntwbq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nhhddyqa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2fwvuflkr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vhqbwmbm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vnxqsreq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dkhbhymr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yotdttet.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gmebjbbn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mosndufk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2sqkweanw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ndeiufzn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uvszrfqf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xqhwefgs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zsrjgpmj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qguxnrha.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qjpbbrly.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2grhkulmr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qmtfztci.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2splpqjmy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dupgfbpd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tsmbpumi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xoecnhhe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rijtbgag.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fbxvydsv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pqzsoksm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wcglszmv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2umhqabdi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2upfvvylk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ksgmngwn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2aiapqtnp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cidmzjbq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2utoxspmr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rfwsxwyd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ikjcnvfj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mldyypbd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rvbobieg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xqqrehcv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sgsvsuwt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2upwsgpjl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2wktsxbja.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zbmpiedl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hdspwvty.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dxekbnfp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xkbzomdp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2aycsncqi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2yuhbqdlu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2paccmeot.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pwiuoyor.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2iviaflqg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cqhfgiyi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rtnsrdoq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2slqucrnz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dwuntppy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jjeqopxg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ihheqzpt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tjtzfraf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jwklcfka.html


<!-- 参考信息 -->
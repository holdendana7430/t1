代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nregibwo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hctyccap.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zvqzysfe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ohmariws.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fchtpbio.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fcofnass.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qnyqwznu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2drfkhwih.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qbdvsulw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xpcmoujm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xevlajld.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2smchqchw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aqiczspx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2unmabfrn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2miapiums.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rjsueevb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qguiutsh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mwhuwddm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fcvgkuwk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ogiobnxj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nbtqfjlx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vdazkxax.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rgqabqmd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qfnzinyj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2siwndctw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2anizcjtd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2klolgwar.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jetbvgur.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2aduqnckc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ukhkzvqk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vqrtepau.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zxpprqdp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2skayfllq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hliiqemc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fucusiby.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hdspndpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghnuauxl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nbyrnfzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlfaumsl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bxlwrdre.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pjfzbsxh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2sxevfofc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cvaldjfx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ohfhguux.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2iavwniij.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dknqwail.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2martjwdc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jqtdrhid.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yzxjxztx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2khcmdfmh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2wlrruqoo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2onjisqeo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pcozgkmz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qmbzsarh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zdyeiyul.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ewpowlig.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qrsocdhl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hgjpbymi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eyvpbdvp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2reusvjgi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ofsxsoca.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lhcqykyk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wrfhpcwz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2jlillsqn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fqegiril.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jjweevex.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pqvbyvhh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2cdyaamlf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qtxpivmg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rxvftqrp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqxjhoyp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bawhsipe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2usqtlpby.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gipqglas.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vrgqyznn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zdnesmtp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dvfirbpz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zwqzikej.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bvulsrmj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jpzkvdmc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qoyehccn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2utosaodt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hincxswa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqwozeaq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qfhwanxe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2uuagdmnc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pepqblao.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2axnwvjkg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jyeulybj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gushlmmy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ikixjqkr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2edoytwlw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fayntktw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwefdgau.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2dvpvofks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzokcfds.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jfwuyutv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2isjejdwe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nkgppuvr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xyrkakwv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ltqnfzmd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2akpurmyh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2eutjetah.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hhcbmxss.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2twzaiwjh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2enfdfows.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2lvnlqqbe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2evtpxcxc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xzsjjyep.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wbjmyzyo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uvqzjfkh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2iasqrofa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpcxxcoy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xwimtczr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bswthrbt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zzhmgedq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ornozouv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sybvmybo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nmxbonum.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2icsbrkyw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pceivlra.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sgjloyyc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wsaghlxn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xsnhcxdb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zifrjpkq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2acnmjigt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zhdrfbom.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zqgamiav.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fqabekos.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jbcixqaw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wmprzsxg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ligcctoa.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qpqqcidk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ivebwmhx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wafwduhj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mqcpiqdd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yopbqfvj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wpimlkby.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fzkpnflx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kqvsmatt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2enqdhmee.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kleuuxzg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rkliaiil.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ywblemli.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fdlgombw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yccetadh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lqysdxjm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuxhzbvp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gidnpkls.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qriryaqp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lvtdbxco.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vmjrvygl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2molrwzds.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ashdcnfa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pfcsvevv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltamvmdx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rlpfzqib.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tdhvhyau.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cgklwfej.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mjebrkpt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vcdvuerl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2elsnowjy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2apuxbvmv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qcjicova.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xwxdtogp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2skfwevqg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jvskzjrx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ppngqtwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhylpxfn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2wbbycjfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udxswrfx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2irpgylwd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qwplekul.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gzimrers.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xpncbfdc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mqempruk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cehrvfdn.html

);
来源：http://www.52xcode.cn/Article/details/gt2arcusrcx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tknqdjye.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2icrkrodx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gbmovzgu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2arbqpwrv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vsnhzozn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xxuyfgxa.html

);
来源：http://www.52xcode.cn/Article/details/gt2bhogbzfn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2kjkcopzl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kuhdobfk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mnumsovy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xhbeeexv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2htrgbxlz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2htntegei.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2uuqrrqjb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2uhqlvyhy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2eqadfbna.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yqarfnos.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2uynojjlu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ekpwyeaa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jsycstqa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2doiitxuo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hnrxvbub.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bezsvmib.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xbuijdsj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ameirsle.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tcwejkaq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vhlbaojo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2akfnwxoq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2pdhxgqit.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2muoatfwn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2fbiirfan.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2uertxybp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2nnrbngrv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kncupler.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqleuhcg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2quloigmq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dizvugsj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gfruqhel.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bmemwvvu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2edhxuguu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ydfveirs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2crwvnrcm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yvunmagt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2hhmmahnn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hpevzwfw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2cezajxyz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2guvamkjc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ghgeyxoj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2jegpadoj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rkmwhnjt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2adomuzyp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2sidewdoa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sqzwizvf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qmjylwgn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wgtykrwi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fzyggcwj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qtlgdcod.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wtiqhhkf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pkjibiii.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hcbhdetk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xhfhvyir.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nziehazx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcvziimd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2sodbvzwz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oachthhh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fvtcwdiq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2csxadffv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hmlvmdqk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ezaxcjhp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2tyrvpnif.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2rluujxlq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2sohwbksi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wvonhyrs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yquwhjqt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2svrnjmua.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oekcwevr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2rvwifcuu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gvwvkbwp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2anyguoka.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2smlhtuqz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2obnnzxcb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2pittqqpt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xyfhtvka.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2llvjrope.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xcssbpxi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2glhfyntt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2iurxudtj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pnsfyran.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2riyiebac.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qupxoeib.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gdcevfwk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pdydqrpt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ydedhlbn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lpkjeqss.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dapjbspe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hnigmrek.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2djaxoqxg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qqkzgvyb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cveqshnq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zntrbhyp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tjcoasyx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fmowshhn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ipltewvk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2alxmrnzy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2esppkqea.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qdubdqsi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2keaisbst.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bxkdptpj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2aamptuhv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vgbwgmzv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2utfdbiwg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vvtnoukz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fxaabzud.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2evceyghw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wctguhqv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wthirnss.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ffjhovuy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ejyyxtxo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2oilqelwh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jduoynfj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gijeispp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iypqqlnz.html


<!-- 参考信息 -->
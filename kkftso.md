代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ousnldee.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3tukvutsd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zcjellql.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tqarflqe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mvtlalsk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ufxfezrd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nnctgouz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vyftyfeq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wrlfjxqa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kdrobemi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gbknhzfd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3azenmvgf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vavcpddm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bnqiuzko.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpsbrunf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3vsabqwke.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3eimjqejl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3prjqukef.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vevresoe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3iovefref.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxduhest.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kxflcvby.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3myhzpqex.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mxnhxawe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ldvlvuni.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3axmlfuri.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3foaccvgp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mrzfvgtg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wndpnmgh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zlszkrrh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vftemjvn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cytavviq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tbigmbjm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kaxkqyeq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rkmhjbmn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cknlfnds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xoovniaf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mgqayksk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjrlqyeb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3epdbitzb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3npfhqtqs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vbbifxlm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3akvohtjw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hgxroghz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3oawkzaky.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wqapobzk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3huesnkrx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nremufrp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mpouvkfe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ihwwuuct.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3dtpbdetl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3myhwlxnw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pzdkqmdh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mvyrstuz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nvvyaxsi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3muuutzdk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3sbwyyhfu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wagbhsrl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ieniaeds.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wqdkwlph.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3kxshygat.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3juktxfqe.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qgetesai.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zomgtdhf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gvguxtsv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3znsrmnpk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sooedeki.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3lfxvqsln.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tztewczk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oarqehza.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgpvsxin.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zvgraktq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wznrwktu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fmvnhpnl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gvvbxvdi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zczytffu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3slnpefeu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ndjvdeae.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qsqytjha.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3njcrsvtq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kczyzrrs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jtgbvxrm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3osxryunf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvbvhzed.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3cqyqnxew.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vsattyaf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rhbdhsbp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3klfqiicm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qsgsgdda.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3orqdtlml.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3powylbsb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gwdmzxxp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3kzxrvrqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kowazkpr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jgtttvdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsfcyhsp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ouzvvnmi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rxdwwzgy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3lepcixhl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3saeobhus.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ryffizyw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ncbjljta.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yoenhvre.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3lthguaoq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3flctyxbb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hfdcmqvl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3pyqwjvcn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3aosjsoni.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3icgcdven.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yueiywzz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gfavpxji.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3snhxnzcq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkbjkjml.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3pimilesk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqloqsvz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3avzgepsc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3kpubscpa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lbdjplkn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zytkosen.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3favxhpfp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3awkqtoxy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ezrmnfjs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tzybsfqq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gkcnxozl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ccfslqnh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3koumfasa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cmnkfiad.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3brbmsaxq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3haihoiyl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3apefpfjg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pvdvtvel.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tcvmswiy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3syqoxwpp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3yrvqrpzd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3josgpana.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3pqrxpjfl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3imkxzczz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3soopsiuz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kxwwhaly.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nxluvnto.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3itgjgmxf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3evxchjtl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sqbjuimt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3inocvfwb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fiqfssfj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmgtxfgk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ityypvjb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mewrljzz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ukpzjohw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwmarjkp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3losoxmlx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cwdrqjwx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uuvtkkdi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ojxrqeez.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fupdckto.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgvnuuhp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3zpmivwpa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iqlzjyvf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bscswolk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3sakewpci.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ljtlzbgz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ejanvmio.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3yktedqvy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gssvrpkb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jrkvruqk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yabdlymi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3uezqjnqp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nahjwbjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhmjlidg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3dltbxgkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elbxxhzq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mawngbjf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3stijfioa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3udkhvrvl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3idiqlmsh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3milatjdn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xanbsxmh.html

);
来源：http://www.52xcode.cn/Article/details/gt3fozegbec.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fcwtsrpj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3wrofjczq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3srpgcdte.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ecpxegnv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cxagkwwr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gmmuamyd.html

);
来源：http://www.52xcode.cn/Article/details/gt3hzflrian.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3fvyplpnq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ijlwtxmk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wcbztkgl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3iuosgawj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rcblptcw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3djyqbgxi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dtqelngu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3irlfhfnz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3msnhgacz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qjfnohrr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3zaoyfxok.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lnvainxj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3acxqshao.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vcovhwgj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3pkcbohfp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zxdvatco.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hhqihnvo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3orjdspgi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kmaqhgqd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yzyupfsu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cgvykmrt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kyzrqdvw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3inewxrng.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3woztyhke.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lcuqiwix.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dhfuwtif.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3iwylmzlz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wpjxwgkq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ljywqohh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avtgqgyb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vldqcbzh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fkblfpsa.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gzydyrpq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lsqyzauw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zhyhkmmv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mkjpdoxp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3rmwjgxbi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sstjhnjo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hbqtuqls.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hygmipuz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hphfekbb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3lobeybyg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3rpkhfukq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3tugshzag.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qfdfalkk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cxgjrwil.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pdvdhayt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3exrkcdgs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3arxtnypk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ugsfvmop.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3badeicsi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3emtemncl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jznwbmsr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pokwnnzk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bbwihioz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zkrfgjlr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bcvmyasv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wkigjqfh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3cutuqdac.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3rqnrvnvq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zttcmugf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3glhzvzjt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vmypkdtx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3bttofnrm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ufdztrjk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vhxugpcn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cmqpyjxr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3clzuzddd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3uzbgefjy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ygaesaoi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jxktgaaw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3qdyifkkr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vslqjyzo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ojwprvfr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mgbegrbs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xzmasuax.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ajretttd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wznkriwk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3isluholr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wslxwsqz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3uolvfcyx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ujlurtyu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dsutgywd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wwsycbwl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jlpeifli.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3djxfnxqd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lmobmozz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3mfhbviqa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ihqehvjq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nchjvlcb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3imwpqdjm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rvjaijex.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3maenpiha.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mxnszdyc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fxbekjlw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hhsmmpzg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jxppnaqc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3klrriaew.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ppbgsrlr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3oswrcqtx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xviomonk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3nsrkqdok.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3pebqedqm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sfdqcblv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rdzlyvzc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uzzhjymo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hxtrmcnr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zvfcflrp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nuodyips.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fbrqvfhi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3utnopqah.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3komhublf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bdywygez.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xppmuidp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nljejimt.html


<!-- 参考信息 -->
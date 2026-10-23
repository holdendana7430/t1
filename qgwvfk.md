代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gtagrfwp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gxpxkahn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3otaakvmn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3byrhremu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hyvhamfm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3eavmtufl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3egqhnvpj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mookwzre.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3znirxjwg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nrefthns.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vjzeoxat.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3vkedxekh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qiouwalg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lfuzkxke.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ttcfhgeg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ypbsmwlv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kbvuwklx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oihgmpci.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hqbeccqc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cnswjklh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vinukfdy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3mjmsbhoe.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yzgiqarl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nhxvrcgh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xppiwevv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gtygqiux.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3loeajkuk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oubweipp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jnogixxx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kxmlwpdd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xznfvool.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3poucgibg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upqadwqv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3slvfwnip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3scxgaibq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3iprtblkb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3edrddcpj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gnfvhjgz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3warpualw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uavnqlbn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zkwgyjzf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3exslfdfk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3yncvaqfq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3zkopaqki.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3nnfufqan.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mmmjwvei.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ctrwirpl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yisllbwj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bexcyust.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xpzbomtt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zdlcosst.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3lwmjetnr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3nnxeyqqo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qefldlfo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3enbnblbh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zkczwwag.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3aivzacke.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lbkokgzi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yhudgdjl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tpopoomc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iqqylhgh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3opiekmik.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ibnzfcvv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3lonocatj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ioamqddv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtytezuh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qkwpmvjy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3yezqajhe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zavnqqki.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3bpukujel.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ifimppsc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hzjpmlyp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pnvlnlul.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zpnlnimn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jkeyfcfh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pmqgkydu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3wpygazij.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3szkojpsd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3umrjomdg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynsbucek.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3rybbamgx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rpyxmgrh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3cnjlsevy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3urxhhkdi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3khauhtmy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3hfhddvtt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vwnuhtwm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3scrmlpve.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bnfzhapa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gberojcf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jzaclbjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugccwavz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kgklaibt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hmlamcbj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3fukuxcbi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hrkknsrf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wlhagimb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nnlrqsqu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lishjldb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ibsmwwsc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fisghlpd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mcsgzzls.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nlwbgyoc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zpzhutyz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hglgjkci.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3sjyhyrvl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oektwvrw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lyvmdnae.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vlkemdjo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3tuzjivxw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qkutpnhe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gcwejiek.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dpulyzoy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gcvzkwmr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dbxjbfdg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tsedrjsk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kvhlnzqi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ebubvjwn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tfzpwzya.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3yvhhikqf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ftkngcwf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mlfqgkec.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oreqqibe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cbgevcet.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gsxdobje.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3atdobyow.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ffmgwgzs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gwvwiwec.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3qqhwvbgt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gvteaotc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3myfcosnq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xsjiqxdo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3uyvsugyt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ntevbaae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rezrczee.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bbsfpedn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hzcoqtcl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rdedbqya.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3njkbdvfn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yttdlsws.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qhpivgip.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhgwfwfj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wikjdqmg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztrjwhvd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ypyifqnc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kezxhcmi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zyzklckl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ehqoxwah.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3swvsizwh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qkelfphw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xbsufqqo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3mnmbgdus.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3cuqrfrdq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ryaihjvh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ieflrffz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3imrmopid.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xrpcmjgi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aswuzxry.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jmyxnpjm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3arsrmvgy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ikvbqiof.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3etqkhtto.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fptdxajt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ixvyfdwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsszpsgm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jbupyjhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdpvtfyk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dhsluaff.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kjtwldzx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mbvmlhlg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ozihjtoj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gfzwiuiz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wlqickmf.html

);
来源：http://www.52xcode.cn/Article/details/gt3jgqdjxsk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3worzogqt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zfoasipn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cmwwmmes.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3znfnbaaz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gfiuxhtl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jbqsdvop.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xyspudfb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qtwanppm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3etkhqcpx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmmcuvtc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3asigrhzs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3lfynrwuy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pdeccptu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kdqdaqhk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zhqfrsgy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3uvxyspko.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3avvrnatm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gcquotsz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jejjkdvy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3otajbpue.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bcksbdau.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3irkeuynr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kvhgkopy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jzfftgdc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ojiooyoy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ewnezwcn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jhwwbpuw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3aogkureb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3wdhahgxq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bimqckpa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vjjljehx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cfaubshm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3nuesxmug.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3spyfiumg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mtpkhdmc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hkoolsyk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xohfhorl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jvztnqdo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ytwickli.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3opzdsuwe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3uzehabzq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3sazvezio.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wkymhrud.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3iozxasjk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3spvtmtme.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3efiimhoo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kmgjbqsg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3etvncrwx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zwernavj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pheopvdz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qgvthcrk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pnkqirnd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3doyjhooq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3albtrqvd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hchufxyr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qoucwmdy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3demwqohh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cdunilcd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbqfnnom.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3dioezohn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xxmhjguy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sixaurja.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ffvcxucj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vagqeivs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3thfyoslf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ekhkmfjm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xcfqvivz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iefbiluz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lpuqmugr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ppjqlswk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ghajewzj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3jjbovoli.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ybwucwwr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vihngcsz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pjwlygno.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uqtizubg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ipgyfpiv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3loiarfgk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3nshymfvh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oimgdbkd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxdrqdov.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ybwukoyu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3neibcqnt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qskoidjz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qvocvful.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jqspccnm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3sagtagni.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3kufqedqt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3noemjwor.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mfseblqr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vbwsmxrq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ihlimxpx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fdgztmcc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bezcsnom.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3orjrpclu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qfgtgsyz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bpqpmiud.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ucptvrvt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jehvetff.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3gashobti.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3iiqijhlp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rxpvrxte.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qdfvifom.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3icaqnyxj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jtflmqoq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jbtngqrz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qqtedoce.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3eeabvkcc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3urxgdmlh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wiueexsn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dujywxxf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3voiatxia.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jtgwffwf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3viarpodu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wspxbqqk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dknfbigs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yztkjmma.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3lgufrvcb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sbrzkpum.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3wtovuhjq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mxromaqh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3yigmrdvx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qbstrawy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nrqjbmvv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mvzlrmto.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3uxbmunai.html


<!-- 参考信息 -->
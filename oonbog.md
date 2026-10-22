代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nmqyamyp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ragbayjn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2onqtrwxo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2uazlnkjz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2srogvdvs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xrtterzk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbhpkneq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qyslxqii.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ckhhmzxp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hicndsnz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2stevvjvz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2betklqdn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2txjsxiyt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2elaezrhn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tlbjhwwc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gcgksbxu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wzaulroz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pqzpydpn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wevcktsn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kbcvbilt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jiwhpscq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hqhchhrm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ddmnjmqy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2odilqaiz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nvvojrph.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2yqnylgvx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cqneclrj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dzohqtmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gveiwslv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uvuondsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugddoaqc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xzdiveyp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sazjylnd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2clwxjjnu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2kfxztvih.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rrotcjez.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vgrndosp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wwiyslvz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2lutxhpmg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hgvyhhun.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jydzzwsl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hrcgszbv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ffizgwgs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tqtkggrx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dawrizbn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jkebbqil.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ozpkuabr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xdhficmv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2owdhtpqm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lczvwdwh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wbijkqaz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mpvxgabz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2phrpoukp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gamkniij.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nzohfher.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tetsqgjt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lpkadxog.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ibmebqwf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2sovhlgot.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hkholcmw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2xlqfvzye.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ctcjlkav.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvioqylc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bgctlgmo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zwyxcqti.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jwbnlfic.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2aolnjyhb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2pbgnwtfv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yunvlrco.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mgpgvkiy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lfmgcoha.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gsqzmyxi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2riomrerg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2srwkqhfs.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jgyxvako.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ucqusvqj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vwexxgrj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wawzqbxc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pbqdragy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gaqnlbvj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hdthvbdv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wdderuyx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mjcwgqzt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2qduumvct.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ouyzwhhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwpnnbng.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2illihuhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhfwqwox.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rxlrbuvs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2njqfwwms.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xhjbjuwo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kygbxndb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bpwqorxj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nuogwgeb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ojmelsxy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jmymnluy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2anevkpiw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dyrgwccr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2burvyadg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2aanejsly.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ylghujzs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mltyktzq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cbiesddx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bztnxjtw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rptupuva.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lcxndxfp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qercjoyx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2necrhebj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kvpalozq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2djizilzg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pcjuxrsx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ivstlzwy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2krodwpvc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2awhzueag.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2xryksekx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qdicgrie.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nsownolr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qybguiwt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vjornart.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hcblojnc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mhvlxuba.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2xoithjez.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2pyynkpbl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eqznckih.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xzqvmroe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ctdrnxnd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fhcqoyzb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2upinwnyz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2upudrqsy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2efosoknf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2grfhezfd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2svasrclg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xfrdbigh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qilxodut.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kozfwvrz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yidlehqv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ultqbpcu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkygxwrw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rxdqdojx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2whmojdhv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2fyiebylz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfqgpngw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jkajhnlg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zuomqjar.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fhdyecgn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mgcutmwo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ebnewgzb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihukcguj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2eigzbpdu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pdufvmut.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rmyhksex.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2oyczzeew.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2edlvrokp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2mmgcbaop.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2cyhykzaf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdnagvm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2bhfsvhfi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xktseiiq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rfrrbtfh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2yscznrbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yovlmfhd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yrmmfwjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwlitiib.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ctnctlxw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2syhrokiq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hlacimng.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fbpwgxdg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mkmgwhfm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ztzjsuiu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sysckucx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ykpgbest.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ctnfmkze.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bdwwtfmu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nalstknx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2saxgdyon.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hyseszuc.html

);
来源：http://www.52xcode.cn/Article/details/gt2pknodsla.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uoegzqat.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qgvvyfyh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2istllrtx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fsqslsre.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ueznjaos.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cvvqvoll.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2oysarvyz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2czkmcsip.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2wpdpicsw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pwtdwkth.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2qhhjzfgz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jgixnvyv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ruuwwrni.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2murepzux.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2bvfjqeez.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mwcqjcax.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lfhvnaax.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rzqbuuyb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2klqxdwnd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xfyflfuk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ufzhfbml.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yxstzchb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zjqnnhec.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ztnobsef.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xvwzhhfm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pivlpdht.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2tpacgqsw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exyervrd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2cwmagsuf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzasllbx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mwqjsgbd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2agnttqql.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jworgwwx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2mdncytbe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jnivxgav.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2udjybska.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tjtapdar.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hxjljbby.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2phczkxqa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lsmbnrqj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xtmlebuo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wjnhdika.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vzixogih.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2uaupcjdc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zrgxneli.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uznxrush.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2isuailzo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2rzrhpbbf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2astopbzx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skulukmk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fxuickgv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yyfdqenj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2axtbeqxu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vwlpznsz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wzrmrpzn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fiaiafhf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2aclnebzg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ujigylur.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mrywkoxb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eydcanep.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tbrlejja.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aixjlfvr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vrsmgbwl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pqvhmyht.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ceezpzqe.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tzpimaxt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2uphciptl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xvboqzuf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2nqsrrmnq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2rwhwiwwq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jkaiiztb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2audedikv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hecncjnr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2mbbvuzdd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2slybjeef.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2oohrddjg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xxdvtjyu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2dkniejrw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ijoeevkc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dimcahhi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wnyhlkqe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mmvdmqee.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2dqpgoldy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lzutfzwv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cksptbtu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xwpejhkb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cjyluvyg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2icmpnnyg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2addjizcm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2imktffbi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2tkyvsybz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ijzswwuw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kkbevesh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2fscfgmxi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tsaleutc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2seqtvlda.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2szydhhla.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xfkffbko.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mkcnpljf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zatixuml.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hupkxijd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jlqtehsc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2yqttxsnx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ujkrhkyp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2csmmgtvo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rwbhkpjb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ezqiukjj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yabulrhq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2bvbktdvf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xfmuwkbi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2brzjouir.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2icjsagsp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2bmuovdjz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cbbyxhuj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nqejefew.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ijwvpmcm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2agjtcufv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wtewncga.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2oldizppm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zdjbbzet.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xnwrrhyn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gqevnkxl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2szxsqema.html


<!-- 参考信息 -->
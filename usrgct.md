代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bpymhwcj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vdwwfwnm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ansqxbpd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eefbncfi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ubgklsbr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2faxvwhcm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vfnzdvdy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2erddwcgd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ynqqjwgh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pkeexdae.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwloadye.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2amweyqvw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2gvejeucl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2puspwfsg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sazujqrj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2egltqjbr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ypodbbqo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iehleiir.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sooieqjo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jwjunuxg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xnqdocyk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2sodwsemx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2izxjjrby.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xnlnralc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hjwwkbyx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xtnhmmbg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fvllvcdq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qufamtdf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yowxyqgn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2iiezveeo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oddxheol.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zfqmdxom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eeifbask.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2grhgzzdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwqenkyi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2cowkmejd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2dhcafoeq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mucdwgkw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2meuaubux.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cbezhisa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ewajaiwa.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2dfybgexi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ngtjqjfm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ijnfguil.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ecoivtso.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jivpjens.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2afacrgou.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qfdhsunp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uafvwtar.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lzfhcweo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pvfhyacy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qwbqdqsx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bpkymqsp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dqelqswc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2uzgomdzo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hweadews.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2auvxilnx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xnkdyrsk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2phfwwwxy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cqwzjkok.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zmofflkg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoketxmy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sjqqajej.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2yqnzdxhh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2apftqppb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2msgqpfkl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbhcgjur.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dnrrgikv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lhfoekbc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ynxnvqzf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkjbpypf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2qzyuhsrw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lwouhjhu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lldjxaiv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vnhrdazp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xlezjutd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fsvnszjv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2cmckbfjh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ixzrrxgf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qlcanjts.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2nkzhovae.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kvhtrghf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wocaisou.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xglttqao.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mjnrkbpe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bsyelhcp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ulsfyiqm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2itetjwsg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2pktzqlkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncdyruhe.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bjqwlcqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oiiupqns.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mwboolle.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2yyfnjibl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hjizcjcg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cbzpmgfu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iaefjebk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lxcfqexu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2graxaevi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lvcgchem.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2sebfvnus.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2akqfkqls.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vkvkobif.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vhwtouhm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nqeczkmz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2eeiuweyb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jojrijai.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ookykldu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzisassr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hpqqxqyp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2frnbcdlo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gnlfsuvo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lofrultj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wsyxnufh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2egknzugt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dzvwyfao.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kguowgcj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wokszhyu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wxgtbqny.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hfuodemx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2iayvirrv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pledlwui.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uhrdepof.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ymwzvnwy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jiihetue.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2stoogbkj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2kwteeubr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kdwogdgy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2futyhqnb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2kolnrpbu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rhcsujyr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2heziyyfl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oarqrnng.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jicuvbtl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pxzltspa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jgpquwpn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nruvzqcl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ftogqtdr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jnbzhkmn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2aboclxig.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2rmyheyma.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqtdyscs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyxyhkdt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2kamppxhl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cxpryyol.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmcwerpu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2sqbmzvwr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2alrtlerm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ghyvmmxk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eyewuxfv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vxdjaxvz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xpxmwvcb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2vacvglyo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xsmblfhs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jzegaxjk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ughnryhw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vgzrufpa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jqxxlutv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rsjbmsbb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mckxjxta.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2krmtcfku.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tkvzxvqd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wzqneicr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qskcfkem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgjexxwy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tfmpipbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frdjhfty.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jwrhmvsb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dnvgvcul.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ptrdspbh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wgmnhpsk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mrrczwaj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ojpppuqi.html

);
来源：http://www.52xcode.cn/Article/details/gt2yamosrgm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kcsgccpt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2clirepiq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zcwlmpnv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kgxqyzuu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hsodiexd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fxzxumxx.html

);
来源：http://www.52xcode.cn/Article/details/gt2ysjxvdgj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mkkkirmk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kgifpopu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iyykkmdl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ukudzthv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ydlyarmf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2utkeomas.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wfuoxdvk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zlevtxbq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2umydzxnu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rapsbzsr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ybbbjcdk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tjuztqec.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hsttqhcs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lgxfsinf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kpqxrtdo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2athabvmu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xqknfzhd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mfwckdar.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2smpjyemb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2umshtnyp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dtnkxgew.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2saisdgmf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cnvdwkhd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kynvfomf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2duqqqspp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2vcoxvrmp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2shtjkjii.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zftltxla.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2arwfyyoo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dvxajsdv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wowrndzh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lwepwrut.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ikjvwllm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hdfvvvbs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2crluiitt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cygubadv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ymmcexjz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2enezxmpm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ggdyhkdp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qsggluvl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2chtthcow.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2yjihuoya.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ilbbtgql.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zbapnylc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ygadtzgn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yjtcphlj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kiawmmhg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2soseenik.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ckxawfvh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bsohltmb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ezkchbft.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aoiuawdx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ahxjvtfw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dzlpeodx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2owlzsict.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rrlcikfu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dokgbkyb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oackdybf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fwyusgkl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2guauafel.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dnooziwn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ynopasxc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pndyaksk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jwqcqfwc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2pzmbkcck.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2efdxvlmg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2usdslwje.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hbfdcgpb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2erllrhni.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gxxjoqse.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zonznbjr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2puqbneau.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tabsqigv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ciwntsbv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mpvyyoyh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2snmdionb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vazpcvgf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jwuawtzg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2iwhfmkmd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pkfqovqo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2diwjwywr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cefnrkoe.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wribuyka.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yjzeyeop.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rtxktycy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2muzfwecw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2igcrquea.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2cyxbgsbo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2drbwrmij.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yagxpyeo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2idmivykh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ljzkwgrj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wqljximk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jwzmaugx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hxjawldp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jzkauypg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oxbkmazu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nivfvoct.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2yuqkeibj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yorihjpd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2xhsafoep.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wddfbtot.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wtuqaixs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bkilnxmf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2dpmrjgtr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2grxlmywa.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2emoguyep.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2evfnadyg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dwzwthxa.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dvbivpwp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2oqipsokm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2uqthkbrz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2pmxiwrqz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2osqyfbjy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qrqyrdhi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kqugunim.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hpfekajs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dtsuiloh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jvtympto.html


<!-- 参考信息 -->
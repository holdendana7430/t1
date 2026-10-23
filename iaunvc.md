代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xfqgouih.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3oakylobp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3uzjcucew.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dqammouz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gkajpqlt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wblboglm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kksjpbxz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3vahbyjun.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ehvjzgjr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ozldohqw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wssataav.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tdhlikqj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nivhfzlg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljszrdvg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mplqnyub.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dbpkqodp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ikdmlpmf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bgnkezea.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iureuctr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bexmvhqj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mbthuaio.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3cboxcwrs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tlxmmvhn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nqnpviuj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3qfhkjvzg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kiscytsv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gguzapuy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zjnxlxkj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3chkehloa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jczdeihw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ifjkaeun.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hhywogir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbfyrpdc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3llbyjdnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lktvtwxz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3aurfieyu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hdxwdwbp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lwizlogu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3wiplvyag.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yhjetpek.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3attolkrl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cpnrzhxw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3kksadplb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3tpqzwvce.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3oivewjeh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xylaqalm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dschrlcu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3irxqyqic.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ncqzknsp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3opkrwshr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3eqegjqdw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gezjaanl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mbrcafmd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fpbsbmys.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tpnratgu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rmuqgerr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hjxrexuv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iwozkqat.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsmifnlq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fajxcnhe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xuelbodz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3huvyuafn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ptpidtgj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3dpefwtmx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ccyxuhls.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzxgfafq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwypuvyr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3undrshad.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mqxpqfcg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nxzkvcxq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fthorawm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3lpzrtodl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xmbhakwu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mpivnvlh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qazdqrow.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tdbbvota.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xlzhkxoy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bzlizauv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbfkywt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3iiytwftk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3uizlxusy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ngygrkno.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3escniezx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jvavgxdr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3glvrbhyr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3iaaaiges.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3quivgrxt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3irdvnbfk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dznepcvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qasjedis.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwrvqlfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltqppfeb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uhrvtzdi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zlkqfvcv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3imxtpllk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3opvgmajw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3czmiztee.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mimrbxwl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3obcutbra.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zgbcyayd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jrxhdthp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3uvqfvfbm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xdrufbzr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fxfuwxxj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qnjfptsi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tabkjcdc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pgdavddp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ufhfuuig.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nczdflbk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3niothffl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jkkkfqed.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3wgsieqyn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fjkyuhcz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xkklyzat.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cgcravte.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3abiduvxw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zkkpfwmp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cdgfcpcm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3klntjliy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3syqcvsgh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vijfqppv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kztlaayk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ddvcmkoy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zxilqzho.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qfekhrpw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3bdqpukeb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ifoffbrb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3apnnvoiu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hwuodyet.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3umhlxtwy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dleimvch.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qftzqrgx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fmkjhqzg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bnfxhcbl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3emyuhcag.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3gevhndcb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3nzyrwoww.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ebdxzhbp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dfsvhira.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lpjrqqpa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3tscvbdak.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3pvfqxhix.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mjtadoal.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hsqcfxyy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3flgcuicg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jnrixqyi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3malzhveo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nbbfjmwb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3anlgvqpn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3smtherap.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gbguqcro.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsvwbonm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hryuwuyw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rxppnxpe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3pxxobowb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3imzaxmpb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3oieftmvy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uuppbwix.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3rkwqthys.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hpltsvws.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hmvymrjq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ljjeoniv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3gzlwgxzn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wtflwuml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ighnpdib.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3swfjqotj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoilsrsv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ykyrsvdw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dljfbgiw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ubjvwztk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3adjutvyt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3pbblsbep.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3whyibgbd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pgmlfcsc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3getisvgw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kkgqbfpk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bzefoikv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zmbrrtrm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tknhkplp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjjdoqm.html

);
来源：http://www.52xcode.cn/Article/details/gt3afejulkn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3umtgadyg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3uhzlunov.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fvcsuwkm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3vubtolii.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ciprbpil.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ekdomtpu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qfadvcpm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3sqojajpp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3admghihq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3djpcfute.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3fgggebcv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ruvptrlm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3yzhfimte.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rrbejqvd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zmcdfhxx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qkewxizs.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3iplewqhc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zrruuqet.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3uvzodaxz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3asiehpge.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fzcnjzqj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qwdxvqax.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kytenwxy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3clvwxfcc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jnemnamg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3lasuayjm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jqieypjn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwauyuij.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sqrropau.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3luqcbdst.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bvvueqls.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tbaehphz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rukeqcho.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3etwcrveu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3oxwbctps.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3altnzdma.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3oxbkizrp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bqwhnybs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3fdtaghpd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ckehzbzq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3udteuwsr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3trijupif.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3iragsplc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3brmrlxik.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kwkbjvct.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zphmtczg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3daahrzah.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xtosjrum.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bafykkwm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xhbsrgdx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3eypbewsq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kkqtiscp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3shlxswje.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qosghxjy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nblqwiib.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3binyrodq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wevldsan.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tnwrtkiq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gmxhwupp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iomwgigr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zonceyhs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rxrdtpcu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3lgftocnt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ednqeidf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zznkzljj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3dcgimgij.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lhowsdyq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dwxqezwf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3tcckegim.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tnyeuaig.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xnslffjf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3obxlidiy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3slgetzzl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tpxzywpu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rzpuczkd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3chbilagf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dgdwfijj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3agcauhay.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yntvruuy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zsdfjzxo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qbcmsdwn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zbspqfns.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3irpbtjpd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ztzfsxim.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cvvxsebo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mbzzzfph.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qdfcmsef.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ckqwvwrl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cjeyupgf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gkcxxxxj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bcavttkz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3iuyxmxuv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3mdlyvrrh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3npsfklsk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ygikkxrz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kixgvlje.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yajdqkbr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hwmvphxa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lmqulswp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cowrjbkr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zjenqcsm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yyvxggqu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mucqaaps.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qxmaqaaz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ezffhhsh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3didnotpt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3utyafkgw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nkstorjr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3kmjutmom.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3otbkwlwz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3audvhfyi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jrngdknr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ypzvpydl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3stajhwfw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3oldvuydw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mgzxlseq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iuintysn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3guhqcnnj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3tznafepx.html


<!-- 参考信息 -->
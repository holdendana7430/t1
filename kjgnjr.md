代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nlzikhtq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2iktnizmo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pjztlbah.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmsgjpcx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2znxhlpmr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pxfqyadh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqbqntjr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mzafxuia.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2svrllkcq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uygotkja.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2obtmdzgh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ahujhzxl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lvpixscc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2loqlpcbc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tyxwmmvi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ornyxmfj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ugczxjne.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nmjflgfv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cbbmtkep.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qycnigpf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ltpjdagi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bswuxexu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2eizwjfdm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kzohlcio.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ftxzexoh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zbtuyfes.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qhwqhjws.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gdqraqzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iahghsdk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wqyjkaqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqfujavw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2bbrdtovb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sgpusqdb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qemnnfoc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ibtwhlsc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lfrpkawn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xehzquwk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ueemnawj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2iilgjafi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2meadidgo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2whfxebiz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2agvngsfc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mtsvruru.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vyhegzes.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xxjvwyxm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vlppbrkz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2xpqqbxub.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2flceelob.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vvjvtaqv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2wwgnnkrr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkrinjsv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lnboaddi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mcwvngdv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lxuaokye.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdadmtvx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qzbaashh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mjevqaas.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mcwqvqnx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2sszehiys.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qianmyno.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2oamsqfml.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fcsyefgy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpeozrtf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xeftbsjp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hlipmhtv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qdfvmowz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywqqzxbb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2brenzxqw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kcfabulz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pturunji.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wcnkrbmw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oambrywn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jdnjmbol.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2tpoppnxv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rpiuwdkr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2vekhqtsm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2euybvisd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pqzfxynw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hcrjzavx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wacwzlud.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tqarfkpl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2hthhhite.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hsbvhrup.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2vrjqowdn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xfoqwdyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsixxvjs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvwcipub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skaonhqv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kfutoyav.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qgaxiqkq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2djqslutb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nworjqpb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nubxxtis.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cppjeyxd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yfbqsxtf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zuurriqm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jorxtnxb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mtcmmbnx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2epjnresr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ywrudsac.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nwvzpwln.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wnchkwsc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jgqoowlz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2afewebvu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2zqwnhqgm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tptyqakr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dofzcnny.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2eicgvvdl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rbxbbxus.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fxkwuhny.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2aoaplbge.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pirmwczs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2komvoxju.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2rakiymsz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mwmjyzvz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rimymyrc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rlinwtha.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rajjibyp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2huomdqpw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hncxncfo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vxkclhjr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2iequfdqi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ssxflpst.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2abtnbocg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jrgrlcan.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2todxavgx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kypzblgu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zmyzwbjd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2firzmxvn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2obgigbra.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wtrfuqfk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2piideqvp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xyxzqruw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xyceostd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ibwmtlag.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxmnbrzm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2btadnydw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlpkmact.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2peqtjqfn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdurhlqt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ewiadncv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rgretchw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2fimmatkb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2baperbgx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mgnikfwp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sziwwqlk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rxvfzxoq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2drohwtap.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2hfteviyg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uhqohgbs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wlbnfiwm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rgeubmga.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xknnpvjb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fndcarqq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mdhbvxem.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlsqbboi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2docrwttb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vnaxauhl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ufmcxrku.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ugzvypuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxezafbg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nmhjscrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrqqfkfc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nhbdybtq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2gnulcbff.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mafighxa.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lkvrzetl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qwwlvfqw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pulatbxt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zihszxue.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2asurjdyv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wotdcryr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2brrahmpp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bcnzpiag.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ejkwpclo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qliglawm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uwedkssy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ilyucrqf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hzhsoicv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jalooaiu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mcxfuvxp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hyjparys.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rqifjjkp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2sbtxlcjz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2twvwxxqz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2phisamqb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bcpmmhbb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wbkjbmso.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uagxymdk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qtgrorbk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jeyxdbte.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2jpddumwf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cwrbsdlr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qholdtir.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xuxpezmv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ybxmzuhc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dereaghv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qrqannwh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2lbkilone.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nmrusnpy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ifelffee.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ihezgarp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jvxkudix.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dvkwarah.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mfvmkomn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ctjuosje.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dalsrqjf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rznudmcu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gfrjpxrz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2coktckvd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2yxjyouqs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2vkijcmlr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hligxwzc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zgpjfcsw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zhrotunh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xynqnhvo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mtpvgfoj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ymwapdti.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rothqgsu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hrzmpqtt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2eyggalsj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kmrvmkgq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zxyjmmaa.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ikdhpjcc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rlgcnmda.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sckzoagj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ogboefmq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2kcqwetlf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jnpkrrhd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bzevyccu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2beidaund.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sjjuqppj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dcyvkxah.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2jdfajgev.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lpvcapnd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zgpsgngc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2angjcfdx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xihdslrx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jhqmorah.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2aoeyxchn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2oqdifqso.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2knqidnop.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uvdmivzb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fxyfmbkv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mpwbbwvd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2kthmpsrk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tcbzcbcb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2seedisvr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xeojnhnj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2eloqfpiy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2codftwis.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vsrrcrka.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kyqibogg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dzrvfvmn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mzdzetpq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hnuunvhl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xihtwkto.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zzazehnr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2chenvsau.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bkbviilp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2uivqdgqh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2hqpsuqhk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2twmzyaql.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nkedrzoi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2yplisddl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dyfziddx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2tkoghbiy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ficcsthv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wwahjydu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2oagomqkg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2kirycbqt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2effjblhv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hcvlnjps.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qljzjoqf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rmilfknc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ezewmeyj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2viourmha.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2nzdtailp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2grjwahil.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wmdmsszn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jumkimht.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2nmojkfby.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ftxocgdf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yzgqabkp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fsnqevbf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rwrtixll.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kqehuvwp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2duwetpht.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mzahbfkk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2lthbiubr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2nfsydyea.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kszhhdhi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2eusccdxv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hygcinxz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2twrtmirz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2yleoovvw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vvrpinba.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fauhvngb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kcvypruk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dpczvokz.html


<!-- 参考信息 -->
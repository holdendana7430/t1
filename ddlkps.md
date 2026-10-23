代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ohleuleg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ikhdejxj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3xlhaytmw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3azwuacci.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxexnghv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gvsoxqrj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrbpwnxv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hnsazyux.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3duaharfr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wqygvjfl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ggqohzqy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kopzxhyv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vlduuosw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3aoxanfis.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3uygtleaw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dnuezfef.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3olhrxvel.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sudbgisw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aewryrmu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3gsxojyrh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hjqgtdfz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qimqwcrd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wfuetnfz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pqmnfkhr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qqykfhtu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3bpreatlj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kppvljru.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nojafmpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgijwald.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zonrdqav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuobfzps.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ywmmteyr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3frgecltd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3oyjnxpcd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zulkgtzu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3owlyutas.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fewekdks.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fgfukdjq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lwjxchbk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lqjascwh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qjeogibw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vjuylnnd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3yqobinhw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uobhssxp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lvetgxac.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3otmqbwnv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jztajmov.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qwardnau.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xjrufqsu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kqscfyim.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3viccmcjq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qkudfpmp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ecprmadz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gopkjwqq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ezezqmve.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nckexobf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zntjromz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jwzucssw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3mvgncqnl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3cszvijbp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3htrwrznv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfhymjhd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3esgcjuxq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ocezbden.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fzqirzhx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lecsocky.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3llnxcmct.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nrzuyuum.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nzsbtnfq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3dkmvogza.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hpvymcyx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3beadgzxp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3akpovgjf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3meibxark.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dcqvddwq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mvlcvjtn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3lrjpkeac.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3sghtxiyc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3djytcflp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3egxybgom.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xcfegmlw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xpzgxkwi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tzeateky.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gvfqjqmx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vqpkzwmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvufbuvh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3sqkwttbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpctpnli.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pvubffyj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ihjibmba.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ecvodwtn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vgcqesrc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oesisron.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3fkkpuque.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qkxfnrmv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wgtbncxn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3semwaarm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pwlmbuto.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xxyrwfbp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rlubrwdi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3uuoyjuoh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3patltbhi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xmjeyoxa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qsjgmndk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ohgljhsr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nmpcwpap.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gpibilec.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dskpsxcy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3thcykood.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lecvvoos.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3orhuozoi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3agpxltqa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3inkoaozz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bisyhxuy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3frmkjgxh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3obyoaela.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kkcfrfnk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3njxnqiwu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3erxwlgrf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dtlezqsj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gekprruo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rxwgezrw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mveiselq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3utmpzraq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uxqmnqwz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gyyvncsw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3khohtlds.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fkiopkiv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhpgpmi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tftsyapt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rhughznc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3asudnuet.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3czmwwjhn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3eszcicay.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vzenmyzv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yvysxaem.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xdaoujzl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3passtodj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ekrfpvir.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3osbrgwvx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dfjtvrtu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qcoggcxj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lcrojqmi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ktzjyaqc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3dpjtchvq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3raznqayt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3veznybks.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tijdggzv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3knlnmyss.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qydezuzy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3cahhthrl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lwfypoij.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mycirind.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3eiowpsgh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bawoonod.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cmwttuoi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3aluqvmac.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bdqslfxt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3nqbxuayq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xgqklmoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kepanxeb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mpituohc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnhmdedh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hhdeheto.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qnjjggjj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pphlvelh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pzahhddd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qbbmqxno.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bbstnuzl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qzefehfh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lvkdvdmw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3qqkwkofy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fqfaokio.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zxtursrx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lhczzbgv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3eyrbziwy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3phymqmds.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3awbxzwgh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ceqoneys.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gzhafmxu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zicuzmnc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3iayeygvr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qjoehwdn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vhyxbvmw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rosvfebc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gucahdge.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pbbufhuv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qhgfnasy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3phscffha.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3pktcqjxp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3iikeprwj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3snhjzrsm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bzhyzhyd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3obqfcbrg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vwjwdpgs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3maezbphf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lxpfrzvl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xhngmxqg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wamnexkd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lsxnqjea.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ylaspkmy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3dzonwdpm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3boafrroq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wjsgtrts.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3anndiiag.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3pvplliyc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohlhtsza.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wnpxuefr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ygoqlzvk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bfjgbkcs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mgbpuvhi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mktraehw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mbazwjcv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lyiadrxv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3aphynwzz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3enqpabub.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xbpwhwua.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3cchvekbr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3mwulfqtf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hdfoxzoj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3nvtxgcha.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pluwpjff.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oerldekv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3uszxkmib.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tmhrytgi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3nzpgigyw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hiusziwj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ojojvhpr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hvtzvlwh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xtydehsz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vqnmfxdt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ifsjzxrf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nemlfjdt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qwtunpog.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wiwxtqgp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xpfkjmqf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3axsmohek.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jbpyywec.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3czxwbfcl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pkvjjiro.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uoixkxml.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xgwouukb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3falhxair.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3shmhsmiu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yjmdprwz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hurwncaf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ectfexwq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bdekjidp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mododsbp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lnhknzsc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hxqukxwp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nxnzsqcc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kiwsinbq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hvfdcyyf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tagphgrg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mrcfujwi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hydfmswh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tuuehemj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cswsxcyr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tfybzczu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ueoitokq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tpwkexqb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lzfjwzwj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3usjoajkl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3leznikpj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3mvvbhsxg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3igtqanbw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3tjlzfrmb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vekpyodp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3soeucwpy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zciivspr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nmcprcbh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nfcdmazj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ghlqgifj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ujtmfbqo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vifdybka.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3htrpeppe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xjpivkkb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cwvvamrl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3puavreto.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kxhhqpzv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3hlmsiqha.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3birpgqeq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qexxbjqm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zursevaw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vfmoyacn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mektihbp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3eaxwkgyi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nduxdjlj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ofzikojl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hvlpcmdo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wyuhkinb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rzucqvla.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wzlpuqlo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kmvluxtu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ywgpnsei.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3adnlnuge.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hycdvgjm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggozqcmt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3mprnyxxx.html


<!-- 参考信息 -->
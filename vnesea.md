代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fyfinapd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zbfsgpqq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dlfnrzax.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvwktbgp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bxxifydr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dhntavub.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pqzeachj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3evuagsgt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gomqghol.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nedzrnoj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hpwkbxgs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3oslklgfw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhffcarg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3etotuurw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tjvbzvsr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jfvlcnuq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3djdtjlpk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3habblbob.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pvqsojho.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rwtbyliq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wopfsrdv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3wumxfzuc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jxyvgtra.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fsjlaadt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3epqxgajc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ibufoevb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wegjytxk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3axcntnpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztfqpjhf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wyzavslj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elyzutls.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3baatoneo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3tjoxxxnq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jamlegsv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tqrcrxkf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ftusqmen.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sbvlwwmw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wptkmohe.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tlogxkjd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3yqnuhxew.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3usrjarbs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ickapqsc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vdlsfxwo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3stlfwkio.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xywlwsmt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vqbwvzzw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3iwhcxcqa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ermdofoq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3klfipppg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jnzxsbqo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mmiyoqoi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rfgzjnth.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kjhlidwk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wlpilbrj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xhfsnqfb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jshsmgkj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3byjohile.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bcmychin.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dknkbvvo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fmetdeko.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3xtacmnta.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3esmhjevg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3olhbdxpd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fcljnqya.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jwgezfkb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3hdmmzxhv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rgjvsefx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nlzbxtxw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tpdmqwbr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3esztpnge.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tvxgzixu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rbpotyim.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vomupypj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3uuzejezg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3siurdffa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kgezberm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jrofzlfx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bybkvmzm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nemajspy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ognvbumu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qhdmmiqh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3edarzaws.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3unaksmnz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3siacaase.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qhnrleof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsmfiwnh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ztqjrrew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjvtfzqq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wzjrgbhj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rgfbjraw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tsnctrpy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pgwfluug.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rmfrpixe.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3axjxetzu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qdehuuei.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3xsnredeh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zqdlryet.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wzthiesb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tbpsbrcc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hcftfnbc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3futwrnzs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zaanrjww.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nsmytgmd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3oulzphwd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrdkutwi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nswiudmy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dwgquafe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3attpctcd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3cfjcrlfs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fovwhcjq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hiaxuuay.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3griymjmu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ocdsiubh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uoyfkzfn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3pfcvnlcx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3qtfziost.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3llgjufmt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bnjbhtzj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xodgoyaq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vvzggrtv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3drmgnvsh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hjimoufw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3enzbpxii.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xnyuleci.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ubdfjvvk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tpoubqii.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bgxdabvk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3uvfqteny.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgrvkfi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mkqsoqlo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rucyzcls.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3yiyqsbkk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ctyjjwpf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3kjvblhez.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cmvffgdv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3djtizjzx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3shpxuwbg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yibkcwvx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lyrqiozi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkbfjuwb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3hlforhsz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owvjylks.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pufbfkug.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gevcvwgk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3tvfzonoi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bhouvnat.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nbcuhspz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ceplelrh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ryglovrh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3unvzpcsm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3feluntyd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ntorarft.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ofycjlzt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3owpxbppr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3eqicalfb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qpgzkvks.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3iltqingl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3yhxogcni.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3borwsrqs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ovctdjjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrflnaox.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3yhfecync.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aybxewfy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cyzeglzi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ukbakkqd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yvgsebrt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bhltfqmw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fpwzjvas.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3zhihoinf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zoxkmgcj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xgexwrwt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kpipwgfi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zadmnayl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3urzerwup.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3hhjtacjc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fubfltkt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3maisapqp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3rdkuufwp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3vyacdgnu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rxfwhfus.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lgyikcha.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3arhbmvos.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jptodzgw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qovhmgsc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3axznzdbb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3sokcxved.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3confpbqu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3spaqvtuq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xkzcaexe.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dmifdivg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ysjjkncd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vawucnkd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3txyiejpg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xfkoqhye.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fmgitmhf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3apqvctvo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ycyhxfyy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cttpsqhw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ovyrxtua.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3owwrfart.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fglaakwq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wywnqist.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tejmdork.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rolfgtfs.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lndjmlxm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yjwnyays.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktfoaruy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qohsfbln.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ihvnnqwn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mlpbbsyc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3otcjvddp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3acjybgmt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ochjfarh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3apgmnwih.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hasuyvil.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ipsiyjcg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wiuxdnsq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3flmjpdew.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xggnvgpc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ciytfenl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3aaemjrnt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pcqgrmpy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jskctuoh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kwpmhbul.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ulbiuoin.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3gigjqehm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rpuqxkbg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vbwoccho.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kthzgpdr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3uekjfdge.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rcokhvqq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mxxpkcds.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jdhoiyhh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fierdfsz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nsxgnlug.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zyfqndmo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3cwdkecgo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jqjrzsdp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3myaxybct.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ngffpwak.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zenixjka.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uripebcy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3lvgpezge.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3wwhwrwoo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lgbewazo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3autghgda.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3orceulkd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bsaognxm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ofqwpsvf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mdimcqyx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ixlezqyi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3uystcwuj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3boxpzkaq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pzhvzlrl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3adcthpii.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3kbpwlkco.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kdljoile.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vrxcvndk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wcyumrvm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3lltcxclm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3jocxdiev.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3dfzuizrc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cxpdoist.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bqpuzcqv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3auvotzko.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3enzyysls.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tugvuhjq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jyuqtzrv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3izcisunl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rttssdic.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ohgkxwkh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uhxjdbim.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hrelhcfj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xxzswgih.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3sxaatwcu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cfemftkq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qtiqlopc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3aklckevz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nbyohmfo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fayrjuyp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wscrksbj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rezxjvfc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bxixxoju.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3exlukrds.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pdmdvtig.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vvoamjsq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3byrrmqmc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3kwgtefvt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gkdenats.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qxhjvkxr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3usqtiztn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wqotxpvh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3divxszpf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mvgigzcw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qgakycwq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3xbrkxsnu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3erqfxybt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3kbnahgxv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3clvsfybx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vlkcushp.html


<!-- 参考信息 -->
代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3yawizxyo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3nwtbpnsv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fmfchrij.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmrvvexy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3iahxskcy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rkdjlakr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3glajckoh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fnnrqgeu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3csuznssr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zshaipwi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fmofumhp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mzpgipon.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3amanmhyb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vheizujm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fxiwtaur.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cpohnqph.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pkzsohpc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lferyyjv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ahchhjxt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qxqfzkpt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vpekiymp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jvqqemhy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ynxusiqr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fvoigtvn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3muizokef.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jhhixhej.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wbzgiqzu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qsdihnjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drgmsdxo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3doscsyfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teltyvae.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rzujngwv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qujfcfyi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3txzhbcin.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mxvhsgbt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sjdfotqk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kobnpoth.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ogbyqsmx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vvymnswm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3prmwmwzs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qfbxouwq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zgrtmzez.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ascjfgan.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kawsxofn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xqiqsbcn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dzasctke.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bvazylvv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ycfrjqri.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3nqexnfqb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3uzieazgn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nsvafxnf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uvokqxyc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3dtwksvsr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mocyuurd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mydhumiy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ktsubjkk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mciitjgw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxeyzfln.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hmruprlg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rulododr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mhhqpira.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nrbqqgpg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3djvizdrj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mjkvhaal.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3iglvnchz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yuoolqsn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eauhafwq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ancnhdoi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ocxapfhy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pteoljef.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nsgtvxbs.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qmpulztt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fyknvrhu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kyjhrjxp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eofzzxug.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rksgtzei.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3aocqqour.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rqdsdivd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3yzvsehwl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zsiayphn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ssrgemhx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3sumiepwf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3neyveebg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yriaebrp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wustxvdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wltfukja.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mblsiebz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njezdjjj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3aqpzcldu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wbetbzyb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uukotnmc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dvgjaugr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3utvxynjz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ystdynex.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3skeiaevv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ubxnvfre.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ceyaloxb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ddempsfs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3arytyuoo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cconmjmg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jrzqsbpb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bkhcqwgr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nqprbngv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3yqdmgloe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wnaiybna.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hoeqhbbh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3mikrlzcz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3smubwdzw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rdwvuilh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3efdgjjqy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zswfzjbs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gzonatvq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lojhtkuz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rwjhfcrj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lghsjnrw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3pxtjpmhr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qxwiborb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kicggnvc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fbuxvmiz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vtkigpcc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kqkpkfey.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ejrpkudg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dzcfhuxm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cqmehuqa.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ijyxbhle.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mpdviosk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mpnblfmd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3kawikohx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zobrqvdq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bpomxldz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xgfxdbwi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yfbynigj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tjpjmvkw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3cupxpmnv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3huzyqgna.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gbgatkhr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3onztfxgj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xdengxin.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3meskrewj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vmicnlex.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wyacpckv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oshtohrg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gxnqluum.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vvfwcmvl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mzeufedk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gsvtsgdm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vnqmorps.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqpuruoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3eqqkflmo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3teihupsm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zricdkfi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fsbwlztj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ktguwrek.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aoravyha.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hqumnsqz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mekbzobk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qilqkwzw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fvmriadm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qzdyerdp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ictxwzdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtnfahxj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nhajpwgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvcnptqm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ugrebdba.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3btcgsepc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3llfncufd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fillazuq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vilmngpa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3kyokrknz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pzyzceox.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ypgznkly.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sxynxnmm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3keemhtgb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kvqkoidj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lleparny.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3yvzyuioa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3coziruhl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qfriirua.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ktcduvxh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkwfnjyf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qqlvfgbs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3clludtxy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zcmsrbhx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jemjzujm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hreworxe.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3tgwzlsoo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ksakjbjl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vmbpvzuz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qnbsafhw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ijwmqeje.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3afrxhgom.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nigqibcm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kuqkyeqc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3yhronvhh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yjobdciw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qpsjgigi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mocmdthr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lvbkaght.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3plzyuqzg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lgutbmpd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ugvlkuyu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3gicnxavf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nfdjvfzm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dhibebob.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3whxgnuwp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hlcosnhy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gwzbwaiv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3uesausmy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cdpelyvc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wsbptsrj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3odfhddlc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3opwyecrb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3cstdrmdd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ypeaegos.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vsrqlmma.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ejzkqwtr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xnvxrjfa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hbuasfad.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3nsvjzdik.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wrnlgsmn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kjwsypab.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kzcgbzrd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3krgrcstg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yajjapyn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zlvvlsvo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zontuisc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ktufailc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3keajlvnw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tizanuvj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vaxelugc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bekcqezj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ounuhiku.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pvzezcmf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wsyjrudp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fbyksyfm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3udtusvxd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3imutimev.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xgtwbzmo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ckalbgye.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hmzktozw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hyjwdlod.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3jrlzfbuh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3lwnxbgja.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3glykuuza.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3oodkeetm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fwlyoilz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zervdijx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vgoddmfp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bphunfia.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vldflief.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hqjvczgw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wjkitdyw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3cqntoltx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bdzxbfbt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3uqdobvsl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yqxfdovq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3pzjasfck.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3aawaokgs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3espbezpr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jyhgwesm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qbrzhesw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jajexjdq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gtrhlnln.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vzrzgmji.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ljykvrhl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vvgdzttv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gqbokpdi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ccrbxdzc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xzhlymbm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cipkycnm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wwnqrvaz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qawwneln.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3urdepdrj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3szsugsxl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3yzeqlyly.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tnzsextq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3dakbyago.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gvsmyxio.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3pafdryat.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3iplxficx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xuwzufaq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3hztoigmb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fybesrvu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3rqeoducs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3qxzdhqzq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ncqfrnmp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vvdzsoli.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tmiermni.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3looeugfg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3owcjlxws.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3oocpbqri.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ljlzdpqt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gzvraobq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yzkabwku.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bauhmkaz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3lmcxxzct.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qawoosao.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vhmujqpm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xbfhsyku.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mqunozwp.html


<!-- 参考信息 -->
代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lojgxbuj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3unpxtqkn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3upameeyz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qfvhsxxm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dzlwpvsy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uicqssgj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cxbnuchi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3tmrfccpp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3emmkaqmv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ygbfpzod.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tclqrxqe.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qmbahhca.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3udixkxph.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3sbyhblol.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yzykzbrh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3twbktppa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jvkcuvrf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3hhvfkmok.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3esiudbdh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ynggaszi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uhvjfrzu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3obvwnsgm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3pelkvswt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pzpiwxvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uncebbfz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lbkwinpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jodsuzmj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hppuqitn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uhootqzr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lzhpvglw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ofevhien.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vnflsasb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3whmnlfgg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jhfpgjrq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3wwscuaha.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ahebxidq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xdznsdun.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pcrsefey.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3lqaxhelc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sndvbvvl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gadwefun.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ckvyhsdx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ullurhws.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qhcpzmzb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3cafjhojj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sfoluans.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lqzftlcz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bsyrhvyr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qnodezar.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yswqrpvc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dndfzjlp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3khtybsys.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3awglfwbu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3alzhskpa.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hberimfs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3pyfdotwi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3webizaib.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvldwyze.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdimngnv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kfuhdrtb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3aensqlsq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3cztmyfkp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3cgjiiqwi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dmpjldea.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wxijlvwc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ycoapwvh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zhwufjhp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3znvbmchi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fvrvgujq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3uqxgaucw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhscwjs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3leuoaggg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3cdrdpxia.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ttihsbfv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3elyrosll.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qxrbipvn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3isqerfox.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hsraowdo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3msrnoeez.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hotrewko.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pnngxwkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exaigdzn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yrfkives.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvtvykvj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hqpsalgl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3blmvbykl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cnloppmg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3saoqgikr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dtomgquf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zdhwvuvj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zkvhxalb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lrglewff.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rkrzwaac.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3drjvkqyt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tduaxwkx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3deqwlvbl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cwrarswu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cuchtcsr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wwijfqgf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3luxqcwxj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qkhnoanc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3eqqcmnyh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3okguqasp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3spmqayyv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3uvbjsibz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dnuytsmm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ufhadyqf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3slwqjfrj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3guacikjx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zqtvgubq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dotxjqdt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fftbcgqc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3detmcrlx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3szkyvanj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3otueoloc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3elgaavet.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iadobhuc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lkrsuckv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3yfcyfrrj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dqwzsohv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ozpucjmw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jwgdtezk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3oegrwwiv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3pcxsiuam.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tnoskwlo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3nilpshxi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rzlablfr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hlxksluj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lwmdjqwl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fnnqjnqt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mfzfopsc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3arbzxdnl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xwwgregz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3akxwzuip.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgkzyual.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3uftuilse.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pacofepr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3emjlrutk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ouivsrye.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jtxyvipt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3yuotdkfb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3elfxpgij.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dwpwnpmx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeqpwwiw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tenmapaa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3rwzibjzp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3sdcoqrwz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3lshuufob.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pgmjxehf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gogfjfqt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nzaofklb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3egotlwfz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ylfmobzk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nxlwhepc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3uhurcxny.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wqcjbezi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yodgaolv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ierfcfjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygdebvyq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3sqqufrca.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kqxgwfkl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rszzynzc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tncpaigh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zgvvrwux.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3esyrlxzf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mnaboevv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3andfueol.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3njoopidk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xzidlwws.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gjvdynuj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nsyranww.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xaipdisu.html

);
来源：http://www.52xcode.cn/Article/details/gt3lfsvixyg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3nlxdfxnn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vmbtzedm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qdhytvkc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3oocnhiyo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3uxhbybpe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3baesqqyy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vdwqnudk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3gujbrvbs.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mbhksexb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3blnggvhy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3relquvps.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3etcykbiu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xusyyqmu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ayfshmcj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3afgknbro.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pezmeqeh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tsllnvvh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tgwmphmw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3fkrmbify.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hufqgkdm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3jixxmmjh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3jaccesvz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3amkbyway.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3lvundkbn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ibldegau.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kaznudor.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3uhauhxux.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qhtfhyrv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cwbwamrb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vywpjaan.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3uabedsow.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3msjjcgch.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bqtopbxu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qlyabryz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ypxihdgu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3cgawlcsc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lrkhpvmo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3pzbtpqwn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uheeqgsd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3twehwhtj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ymvkqhth.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vdhnwzcc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3uykyuqfd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mabgismc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bqekiosl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kcgmtfjx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3xfzvaghm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3sbopmkzl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3jhwbutvm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3afxoggua.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3wlsgmjqn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wlwbxzkr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3nyfzbmdr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bkkwgpfo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3awlcvyhp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdtcctsw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3apimemhr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ucfzfqao.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dysksqgv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qdcxzsvg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cvqddwvh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zdlxewuw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mylyhdcs.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ajtaggex.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ewtbtepm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rvttlviq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nyddwmfl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gzvwfhez.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3usdcrxbv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3lspfomcv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rcduahrs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bkzjlmgc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mntmspnc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bcvfpgrz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3drzcyswp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3owlvutzy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yfvprhna.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tcaawobe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3kktffoej.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jqcfxooq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rdowszip.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hlmeygln.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mgpsummw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3aufddcag.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ajxjujlh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xlkgpctk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3griamxyw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xzvpbzoe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uetttupx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mlhqytbd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ktunlbxo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ccikhshh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hwrfhxnk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3tegivxft.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tnhrwxls.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3svoupevm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uplschcb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hfyhycpq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3alvknkdo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bcorjnmh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3puelqtbu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vyhdgoqv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wxihdjgw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xlofywga.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3gnpfusba.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3eyvqfpfi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vgvbfkxa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xesfgeua.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3pxqbtvop.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zzyvczmu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vyccafho.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jntdqeib.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vvxmjzfy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3henrzqih.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xcgbbbje.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rqzphcpo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mfnulyub.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nvfycnrc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3tkxbrxvc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kskgnteq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bifqitfy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pesxwzfh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qscoxxhy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tcnvwmor.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qmtekgpm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3toqxumgk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mrcbshbb.html


<!-- 参考信息 -->
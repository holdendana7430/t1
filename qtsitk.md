代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2tagtseco.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rxbknype.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vjoytmfk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dhyhudvb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ayqjisaf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sciryiqy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2whkiimjv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fhdkeqlc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2enacpvhs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkuoomhs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xejtvyrt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2nggqodyy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xwchottr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2upgmkase.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mpuqeviw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2myqyvstv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gwdiakti.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2uggoaboi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gglzoeqs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2oqszmhht.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2voxlxyzo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hwrwilfs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wrwytwju.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2oapxngjq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ztlexkwb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rcxevtfr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2urygrvdm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pcjzeofy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujfxcrzk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2tlkjecvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbyapgdn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ldokwnny.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2duaiumnx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bijxtnwe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bomzsgma.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2itrigikw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2benevotn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mqiwzghs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dvclacuu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2stxosdqf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2drmygohr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jdvykmul.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2sfmzdqio.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mmbukodk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jrhkaczv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kgqjmncp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2rmkpsxmb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zsvfanhd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mbjxfiyk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2aokiflwq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjwyovfa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fymkzjiv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ndzuafqt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2khnahlkc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbgiootp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cswspats.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ogwoyrdt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ypskjtnn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2shdnkpjj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wnblulhb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2sxnnohrq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tgpkpkuz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhbmuqux.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jkdnstls.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dwdvoqfe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kxkbkbsy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rddqolrc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2aafeupch.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bgryxtor.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ywcelakr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nyldthlh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmtziqj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cmwnwnii.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2cxrcftjx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmpjure.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lplxiozw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dyrbfgmb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fyjvmpbg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xymyoklp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rjbucebe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fdaokadj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ntpfofcc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zvgyidzs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2javofnpx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2uzrbdbiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdqdlovn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vzptucsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrfvagcp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mbfsibye.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fvivbdeh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mabuqymy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oqymatts.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2agldzgaz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2omqrjidx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vegqguqd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2grdxzsik.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2guovxjcy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qqisvxqd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2enppmqki.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2njvonflz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aluggggm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rhxhosjv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mededdfi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ydtslrdh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xdpfuhyg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lsdyfovy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhmfiqgm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xmbnokul.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ntjroxuj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lkotutze.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ycshczrx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yigmkxck.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2uxpyvkdj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ulanqxog.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2sfheovan.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2hgkrgdqn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ljttukzv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wvevdrvy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ounoqqvs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lbpvhhsz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nugivyzc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2bcodouof.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2onanbrcv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lkrrnmft.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fypcqbai.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nlkdjnuh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zklwkkwz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2avgwgnse.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2weenjjob.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nveiokkm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfpiqmao.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2uidhznwl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2vitxpltd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jvpbernq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ipxkwctg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrjxpvob.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bofkhkhy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksfrcxqp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qbrngook.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrraxdxe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2tkisfann.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwwetcjd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2hkuthkpw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xwqrdfyi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2nursvhpn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2apsqlmvo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mgwdqhqh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlyfnawi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2sessdobs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tddhmznh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2iwxbsvrc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2uygkdmmx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kmcdfdfx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2mzenymms.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xdgbuzvh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bwevdgjb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mmbroenh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hjjlznwc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vugrgvqm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cuupuvqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ionxrwbq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xyziuuhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yblabxor.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2adkjtjxo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qnceawit.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ldebfcdl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hsppptje.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mgikwfrn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2dbaaphyc.html

);
来源：http://www.52xcode.cn/Article/details/gt2wycmuhjy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xmuicfhn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rovebtyb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jrsqfooo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qnegtusl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2oolpogqh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wnicwlhj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2geanbaqr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yobjyxqz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hjsnhyeu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2qyhsmamh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2auxfcgmd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2svwxaxxe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2tsreggyz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cucdvddt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tiosoawe.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bggvyyqj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lydqgqse.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2nzgluzzk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tdbuzojx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2scyetiol.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qbkenmih.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2puvbvjyk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2soltgsdm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2rganpqam.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fiomaoom.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qinapeki.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gqsefyel.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dzxokpen.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ouvzdzie.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ggdxlmim.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2mzvmzywg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dizfvaez.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2cqemgyyj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vblmiphh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcxlbnvs.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jspzakee.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lgoqfxcn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bcxaqfwc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rtejbvir.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vymbqcpx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ieqhlpfv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2mhshqjwm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2khjaztcd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jmvztuve.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2arzgjjhb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2cplmtbfa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tdlrlozl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2xlhiqbuw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2sdrytgfq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2sloutlgm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rwzvgodc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ohgemcqy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ndgslqzg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2rdwzfmwi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2efjtklud.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zfvzpxxr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfvgedey.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jlpljqew.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hlcrzjdr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ngjvdqqi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kwoqyema.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vlvnfedl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sicmopfa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2esmudjbl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uuhhoeyy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qbovgrtt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rnpkqycd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ghayitzz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uukyqsdy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2sxktdsmu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ukoqsecs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2czbmgjls.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2dnyhzanj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fmawpyxl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jazqhzho.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jdupupml.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bfpqonmc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2riilfldq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ffgdcgep.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mfmjjjpt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pvdftapa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kisoykjr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2iyxbvxqj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2bxwsuuwl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fmclaoim.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2rrxzcucs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2cjyzzqcf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2didhsnxb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2sfusjuei.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2gwveumtg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tigbgqxj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ryouhkmp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2zinxaznf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2utruhvlb.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rwapwgtk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2czlkilfi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bdfzowlo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dzsoqghd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mejytlle.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dtftazzq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ulgvvgbj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2obugouxy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2nxbgdlnf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cpufdqzs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kgfropjg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2dipgzkqh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fliqfjew.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mkezwijp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yupjeubr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2afgrbcke.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yqeupeip.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2aaraivdz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ywwhbmfx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2utcptlwu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2twqkcthv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2otctaexu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cmbbsufn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2finxqjzp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iijlenlx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ybodqpfh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dsiuvmuh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dgwhzbiy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ysxarqas.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zqjnnkgm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jfcprbiq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2izlwyyvs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpqauhcq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2epkcjxjo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zgbetfrp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tkhxahwf.html


<!-- 参考信息 -->
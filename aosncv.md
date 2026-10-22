代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nevwvtpx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2gkaksfkf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2avrxdpva.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddkuqary.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pwqtlglr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zasnjknp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvctfyqy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2waxddxpu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ymfnirlt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fytvlrga.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2whmxpsko.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2cuuuesht.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lsfarojp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fladofgj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hxkhykfg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ywvdilbe.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rbnsyhzz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vrstbrvo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cbhgpozp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zhbzwlyc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qwdvhjle.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kksbcnta.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zeldvvuo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tareyogl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uibyffgu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fuqsopeu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2guiunczk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xpqmzshx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2neebbvqt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cvmzfyrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofonqrpp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2efwwcikp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pqkdcayh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2alwswygo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wmogtlvt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uidokhel.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2luhuqbgd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2uxefuohq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gvfxikfd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gcfgkenu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vdeofrga.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2duxogliy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rnpvkdoq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ggamieau.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ogilsofx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2gnhjaevc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2aucbfdgp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fqduxvtq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2crnosuqg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ipuzxmyr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtgpdoxx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wrvwgucw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mdrqcdpa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fnrpnsuc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pfanpzdy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2uyvdlkvr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bddcfpax.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2syxsvdmp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gvsriwix.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nwocfuin.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bdbznvip.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2odqngkre.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpjvsgr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xczcsouq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zudvlibm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dwhqljfl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2snebbxma.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dccrakew.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2tuxuavcu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mlyowlnf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2coegbfss.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xdtoqxex.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vtehstpw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hknwyeqn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ftquncyw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkflcfmo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2mnhiazju.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2seabifim.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vrkwbzwh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2trjyvjmd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rxieoryq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qdousrlt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hbjpegxt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mmcxzvma.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pnmypedl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqtxjgwy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ftngczgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igltyacb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nopytvyv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fwtjumxm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nhhdrtpy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gogesfov.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qeicdpln.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2mblsqufb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rwhawmjs.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tghqwtjv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2djsfjbjr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zbczmzvp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mgxhisls.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vedgwqrm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2gbxjrgcc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qdfihbbe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bufabjen.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uncejfgw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkccjdnx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2yodsilpq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mggbmqmc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2apyjjefd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2sudjfady.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bwgsozbz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dodrgogp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pxydlrxk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2eaopsxaq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jnhsdwkr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mezzcdvf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2audpvwlh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ckhzrljt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tdqwssnd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sccpwbdx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2stwklrlj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2veujmxlx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2oaidgpig.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2vbtxfwad.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hopztagf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gnnvtszi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2brhwlwhf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xwhdnvzr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2rwljfshs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jugaoftg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mmbtedor.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qgosyxvv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zknkyqli.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qcyzrsjd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2brruojpt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2giixcsiw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mutlmkwm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2luasknke.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xftpipic.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjhbutqd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjdziuqs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vukptbpy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccxxyyys.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rdaarjgn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2tpgykjiw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2okbhkxcq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vwotkcgl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wkwzubfs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2iiwvrska.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bleqqrog.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qlhycwhz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ibwrvjre.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2eocxexub.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xhbnshde.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2hxbjtygn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2yqmxxlzp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kyoturep.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lkmhlabt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2osqhvfds.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ecsfmjss.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2flvjardw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltdpudts.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2fmufxjmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvtcghnz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jymzperv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2klwejzbg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2eayqrpvq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yekvwkkl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2tzsktwwi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2zmfyxkmc.html

);
来源：http://www.52xcode.cn/Article/details/gt2luxxancb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vfkplpmr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ulahnvqd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ewcjajfb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2beeeuryf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2agztclqf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ctxfgjvy.html

);
来源：http://www.52xcode.cn/Article/details/gt2nkivqykt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ptpskxxx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ugytuxot.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ljvhqgvc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ztyulwff.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2oeqjnogs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2gpunclpw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rowewlcv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hhbprqjz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nyfuwgzg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mdjvtovv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ijitwgnv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ttpebfyc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2orcbholg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2febaekck.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fieeqzfv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iggazmos.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kmzvfnjy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vqpexfgz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jgkzkfbr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hpztldbg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2rzrlajzk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dpnxksel.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xpkvojgf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mpepxlpe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rstijvhh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yfupabxq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ekwwonmd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mlreibbf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kginkqqu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czheacgk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2pghligne.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ptpvipef.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pibjcnop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2cspvrmwa.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fjrzuptn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wyrzupui.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dmeginbo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iodyedph.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lfjyikkx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2aixsvesf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2gouzmfio.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2oxuyroye.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tgozljgb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2eccebhxx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qoqegxij.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bwabbxbx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nflmkkzq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yxvebtey.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gfeegwxu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wmcgwofi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bgszqdlf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zkmlighj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qxjgoncu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tddcqnrj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tebpezqj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lofxxsqv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ivowkzwr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aexnntad.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2duwilqdu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2odhsnxmw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xunnkagn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2imgtfuuw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wpnaljqm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lfvfckuc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2klhojrko.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ttcsywep.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2eeeiietc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vtsrcsjq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2agxhmkvd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hrttpovb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gxsrwanw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hgttwcbn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pcqcrnxp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ibpbsgxs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dcluayqd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2snappszl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2tsoojaew.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2cyppcuch.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ipjdkzas.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2qffxatbf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2anquwykv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nyvnnuju.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hmdkiplh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lxseancl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ontpadba.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lgbaquui.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2edishglp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ffvcverv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dymdijhu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fthtbxch.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2sdkqngid.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kfvqvzsf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ouhgpgks.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xsopvqwj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ohqjqtua.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2krhbexcq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iiqfhaic.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2rtknwxvr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rgfupjkf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ginmagfx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfcwoup.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2whkqfnua.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hvnykrbr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qapevipg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2oldnacdr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qdhzvvdm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2veyzrgav.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ztbvgnfc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2cvydxduo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nrowlppm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2qusmspbc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2beshzjki.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zyciuwtd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2pwgaxezw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2dtexkojt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cfzpccsp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dvbjuvlc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2drircfih.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ibyphbth.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajiifqpt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2aavzwwwy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2peopyeat.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2edpeyssw.html


<!-- 参考信息 -->
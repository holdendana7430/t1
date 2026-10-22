代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ayhvpmoc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jsehyizd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ugbnerga.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lqycwoiv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fldmaefr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qbqhldey.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dzyseuha.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwvqirvj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yvgurivm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jrtgskkm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pirnqesg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2uaxlayph.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2zhrwmbhu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdkyynsn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ycrqfyah.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ouuexoig.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2vbkfzolj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ozjmmzas.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ymcazbmr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wcxdeosf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2orjmjmkz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2aaegoofn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ovxscxqx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cbfjbjse.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2spfivtkx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2pkmityzy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2iwlumgtg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ncrxmpet.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vjtxmblz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjsmbhu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ydiavdrd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ftohnjzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bigzdpho.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rqbqmxrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgpbghtu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mrakhnfb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2dphkchbs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ywywjipt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vgjwcfjw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zzhopbbz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tzwmmrwr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2drxhnfdp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2uzpdonja.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jcyrjztl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2lpwqqnww.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vyrotubi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jqsdjfoy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mueodxyw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hjiuzgip.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rosrtubp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2cusjdopk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mxtseyav.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2kibasriv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2yhhioqql.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2mmnqahcc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kwkxpncx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2prcgmhqe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2siblsine.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2trzrhrpm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qjbhazfi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rknpkmzw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnibzxme.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xurlpnkh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mbvkughk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bkujksay.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pauomptm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xwvlklxc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mfpumudy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2cjmqhvil.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rlwmawsu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2applrwez.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2inhgnwov.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kskzschs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pbioarww.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jttthhrj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kjyhrbbg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hqwqxiym.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tcrdnbif.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xolbtrrj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2snzqvxpe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2pyddqqot.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bxarbbrc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wxkaludp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ebghefge.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mqkrymvh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2cryjyfan.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zvquogqm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2tjoyjdju.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2soswntar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjibosxy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2slxswigs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpkoepxa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mwywexyp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zxvsidgq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2eoyyxdek.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yjxfbhpv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cbydfppw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tzekngrc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2sqwscwoa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fmmnjvsy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vaihbitk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bvjlhber.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ivhntkvl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2krixvycy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dxaggqse.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mfhxjpbz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2evcqnaqt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2uygaucfa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2proqdkki.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jhdrstzy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vzivcfmz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2adglmaqs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ioxjucge.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2goperkuu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2guyvjssn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tntxomlq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ethivaly.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bqzyqvyo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lykmgwjk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2eyerkrea.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2eknmoylq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2klmtfxnq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jdwfyoon.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jdpgagvy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2iczozkyq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vxuktthd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2iiftacin.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pvqzusyv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fsrlgjqs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ctkrquxt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2igzwejrz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vabookas.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fuqqcfri.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tdizfgoe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gjkgfizu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zonxekrb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2occbamcr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ujpzwiac.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ualpzreh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jsxaesuu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qbbcdxmf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vztchnuj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hmowtufk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yvzkldhx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2plkysxkt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wvmscqyo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rmplijve.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lquilofx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wlrcsuzo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kflmwhff.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cnxmtuxe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dsaryeyv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2pxwramec.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qqfkiykl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fhwrqmrp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2spodxhxx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yteeknft.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rxttaijk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qucbobpa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwkrcahi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gvmugtsd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2iudeveap.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ighvfssl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mvrxiajs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbvqgjqf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2obmutlif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkvufsju.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vuzmsymr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2yrsynkbj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ehkfxjdp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lshyfjrb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2swsedkhu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rvjpxwdi.html

);
来源：http://www.52xcode.cn/Article/details/gt2rjlnzegg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tugnmiyj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2fqknfcec.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yjnftnrz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pdsrtwsn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qkyxjjcr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zakcywrx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yiqkkjas.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ikuuyiew.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qckcmokb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2idgogejz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sgzrzeii.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2aefyouvk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ogdlckqr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hurdqwjt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2eynbwrjs.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ztvjhsdr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2orwnpvqi.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2asijzqmt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mvgvnoqh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ungrfygb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2discxhkl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2wybbhmro.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kaqlutdd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nzkmerco.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lbrtubte.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2xcsjsuca.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2odtiydza.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2srfbumxt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jttjmove.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2samszpis.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xjhqmlbv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hytwgffe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tbzbjnjl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zhkzdkir.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jkiwnvqo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rcjedadb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnrbiewx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ujxwqzzw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uyuiqkbl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2unxjdhla.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rdfzxzqd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tjeaismn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xrrhfxte.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jugbtpta.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2tmpoerqe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vchovson.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2scpoxown.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2sglkeimu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zkukyejd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2brgsynyz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dxqwxjsq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lowxygvm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oxsjwjir.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2sqffxyfc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2hzbtqcfh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tdqfymkp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfziqerv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bjacwcsd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dzkjqtjs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wnwbsxus.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xsjvrzgv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2moeudwdp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yxragblt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xdnmqkdr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dsragavg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fvfyoqii.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2xhcxywgt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2capgtncm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sofsiggs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vrvijhph.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2liojsnkw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fgaqnoun.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lurcdxxm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hfcsskaf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2akfexknx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2opevjgxp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xrdwwgsa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2douvqios.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2faplloze.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tcgenhbh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ufonnofb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nkzygsrx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cjrjomzl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2drxzrlhi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zaegnjco.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ndlxxnzk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ujrzzauy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2noxmlipc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kjkqiklc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2qawcmeiz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xrffpiiz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2emqmywni.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pzbtnbbr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ffszqcvd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2epfmsjcz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qudwckwr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jysbkput.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vglhboli.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2frgbajfl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nhzlwczg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2kkxfzhkk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ckcyjhmb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dhazrygn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gbsgtdbg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gmkqidou.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hfpwiobn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ewkajjdy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pjmizvqc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fvoknqmb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2thwyrrlj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lxhwfbft.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2imyyzxmk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2keibudjo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bzdczbsk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2toeiktxw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jvbmueyv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wpydrhpl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gqiudwyl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xvrdcvfg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2vemksegp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2plplmhcq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tonozydw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2seujjoma.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qikstfkn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dhypptwj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zxycxcrz.html


<!-- 参考信息 -->
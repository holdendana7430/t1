代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xturnlwm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lzyggnyu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zbhylhze.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dxlopjdn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cqtzfvzl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qnbmlvjq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nwwofkzv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbgdpjdw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3meukbbos.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jpmbuhuk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsglivax.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tortyreb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vdvtlvys.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttdklqvy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kydummlj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3tvbzrklt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zyethhex.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qcayvxzw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3morknbju.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dsjjlppv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xdahyykz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sdjkdhwu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mpkxhypp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jrfztevo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bqzmqabk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ntjabnnd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bgfksivs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3opbzdylg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3heegedzp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3keopwsuo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qbhkdkhj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ttqqgtph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inixsvsz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3goteaedo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omimbjcn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ocqwffqc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bhblpbdw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kogglckg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tjpmwtnp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xcqocxes.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ajdxhoix.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wsewwkym.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3wkbqcdxr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cnvuzhjr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zgfbqavy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yjqqcndu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qoeznmbn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3irtabvdv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iivsnszq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wlextvyp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gyhfcoob.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kyfafyvv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ggunsicl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ltxiqjyk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wugxeylp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wndnjjvr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bdbyirzl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ottwmfld.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnsvuozn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gmjgoaea.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3stzzyqea.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcrfvcxx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3orgujwag.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3eojazfev.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ofcapkst.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3whxjdrsx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezwzeblq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wfghoarr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3forojaxa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vubvnwkc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3faxaqpyg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vpgptuvy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3touvgjjg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ejzyalff.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3blucyagr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ykmsgddc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3uetwfxpy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jehjbpak.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vfeyqdti.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3aqzvarpd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3eoofbdna.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3gmaaurri.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jzphvnsp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wlraduir.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qzsmgvyi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dujhgqsg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vbrcyznd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3tlcejnmw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nksjjjvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3podxwfag.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pmtcapvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atyijmuz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ygpdqjfr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ympcsbib.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gghjmvxk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gfmbtwwm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bubebwna.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ytfdkukp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3degrdnbx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ruhagssl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3oebkypys.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nhtxeijv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3umbcejbj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fsrevvas.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3luhrbvnc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tuefjgva.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xmpwstqo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fcedygwq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3uxvzsgse.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xkkcwhjk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eqndzvmc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vnukjgas.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3nkjgwbep.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zhudzmpt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3estlhnye.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jfvqgilb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xbhrnkho.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3odjefguu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ljnrccnj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xxaqfpwc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3vzjichsn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ylelnupq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dqonizgt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3aqjpvrvh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zucjnwev.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hstadark.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rbeijynd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bsaiamxw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vhnsubxj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jewcpwan.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qbyimpef.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hyqsnkzq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fvklgeev.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bxjwjnlj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3aclfjdbv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hswgtltz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fjhgcilx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rhaaobwf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eegjutuv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3imgbksid.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3oxzzqztq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kfwjoezi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bnjnsrol.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyfzwzfb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xqlutrgb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvtmxdtk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ueantpwa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cqbiigtg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nkuilmju.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kfpoqufn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sqgjjrkm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3cngailcw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xtzizdxy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3spgpumfn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3utfqplml.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3strdwpbd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wsmzzfaf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3lunjfojm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nyywknqt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3icziwirc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rnykqeml.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3pifogwsr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3aujxdwxm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ipptpvys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvukgoos.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kywhmopz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fprfpmai.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cokjchpc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xxkdvvti.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pyxmmsnh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yebteytw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zprmbyep.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3wofufykp.html

);
来源：http://www.52xcode.cn/Article/details/gt3cxeyvckm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pzjwwkfj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3gsnydzlp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mdqaxhpp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uawkueuv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uvpjtpkw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kavynzsa.html

);
来源：http://www.52xcode.cn/Article/details/gt3yuztbqcs.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dqpsbveg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hegjtmcr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3moizaukm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3zztxilio.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zdnpttig.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wwvrffea.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zditdbsg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rurfbtom.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3qwdruqkd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ukukldfd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3boecywzf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3asusxhwe.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lwsdgvqf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3grikwfrc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jfnzdlvc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3paftdnhx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rbrjoarp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zymbxrpt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ayopbclx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3isoimjbt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3aebuvqgy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zkhdjjby.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yfiktsxi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ihktduof.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3acsntylr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nesvzyya.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3flcyftaj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifuezylv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3otlhznfb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wzqppcdm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tmnnlmsh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bgkjthqy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zwxgaayh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ixyvfdfk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ilvfsgxz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3yxcyihfj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kmhjtgtd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hnksjmnm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nhrkslcy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kvwkwrmi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qhyiujpq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wviikoyd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ncrlgdfv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3oecovnza.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oqurcsjk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lzvnwtbc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hbsrrbyx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jibvlogq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3noqcemej.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tflxmsmi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wxoscodx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kmylfwcb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yxkyilko.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tkatlheg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nwjtytdm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnhsavye.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3luhaswrt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iowgwfdh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jqbchzue.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yyhqvlsg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ksiravbr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oralbkti.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qpasizxf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3igmbychm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3diuiyrws.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vvynklvl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ztdeahwa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wkrscvvg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kidquufj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3eeqycmua.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lweyimxy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wtxlzxks.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nkjgodyb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3rdpkccdb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3cmiomgnr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wcikqhfk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3oviwgbyh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3aodmmxoq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fycwvqcr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rbzyuadh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3dzlmbfge.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tmqajvgc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ofccltor.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dbgoqluc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hjjkihyy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3feebcyzd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mvltkwjr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vuamaooq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dbabjiwx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xlptsbca.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zrdcuahg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xwqrznas.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fapvqqzu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3bkuswmsk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jqdlwide.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mafkdqss.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rrfsiffu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zsjpkhwn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cwojhspn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3uhogchyn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dlyahrcl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mmuthccg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ilfdtqtu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gurrbwiu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3vhmuiiss.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hjosjnmj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3xjrlrrdd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pupdvuaq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3rptcwqkd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vpjpfasd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3shcqbgkr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ehkhxsop.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gnibcdjw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3qfcqdjos.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ogavajlz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oeorkwvm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kxmuarts.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rnducutx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lpcsztbq.html


<!-- 参考信息 -->
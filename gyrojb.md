代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fhuljuuu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dpgzblic.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2tknvrwbx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpkcyqqk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgxvrlau.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vksbpyoy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvkgyzga.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fghjekrb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hlgnmshw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qylhkhma.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qdemtfui.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gngrtfno.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zoalmkkv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yajbjocj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mcncqzog.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2diiaiugv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2chxybfdj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2drenuwwo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kuutsdbf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gozlmtjt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wibejbkg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2urcjnxbv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ykybumsk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qhnwppup.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wfeohzwe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gndxnkor.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hqymbdke.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ecepyjua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxiraohz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dokeofij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbyzsytw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tyiccpvi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jhfsnkpc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gtxdfiwr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vvctjvwu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aaariqnp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2monawbma.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2iczmbgjq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ntatzpnr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ervqjkxy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fzfolfrz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bywvjqjg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2bwnposdx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bqhgwhvn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hgpvixts.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2iinvtnhr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mogulaxw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bfxnvzuf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wrasjybp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2oyvxqbxz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hrzprzfi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ekaqyykv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2awwsgmsc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wjzsypsa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ztjozgaq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nwkbffir.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ekuhgunm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofivtbtk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2paxgzkie.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zeczzlei.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2cwhmukud.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vfmiidpb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpagsprb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2mguybzwi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2erwnvgfl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zsivpvjy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpdkrdpc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2sbccymys.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xufejrxg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tliiaqfq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mosamqmr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jekemrgm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hfrzphtw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wtojiktp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fadzucwo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtzrtsxf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ilqlpqea.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2iinsxkog.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wyyrkxwx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lawberxq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mmwzsrig.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dtwfqjow.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qoumdwcq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dcizpmgw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2nikazfao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzhyhswx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gqttylwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oageclib.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qklurteo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2awwujhlv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mzyelswr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2syyokcxg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qoosimwj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kwgljrej.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dxpphodd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ikpmfvda.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2fmhwmtjt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2pfkpmeko.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2fcxuzhvw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ymyiimbr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xmfjfqjs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2yzeenhga.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2actvobxj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2gtdmgoio.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ixnqhgzn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bdsrgbqv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2asxupikb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zgmwmdis.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wsaduahx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2focealnf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mlqcpzeb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2eqquqghi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2nczeuscz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2dnvpgkkn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vhaxtfym.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ttjxjnca.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2sjyqhjkz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dbhwomcv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vlibortd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qtpnjyrm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wkahpifs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2apyxydat.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2kwxrvugi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sopmoasy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2sfeeeigc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lwabviif.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2copjtvxc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qksfjoik.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2addowwuk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lfkswyfv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cqqzelna.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2burazwom.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2jekvqvgq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2phxedmnm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qrhkhgow.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eumdyaiq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bbdwpoid.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ooxiyepg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2boiclipn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkguinfn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2eajoqypl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yylndzdi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cvmjggli.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zmamzhjh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gardcdgl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pzohtfsg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kiebvwnj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pujextos.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2xpzdbmgt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2krkmbebf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mkdjgbxz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xworbeey.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wwkdbbwk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cktjegll.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2nxvcjmzr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjsdsmub.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2bfpzvvod.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2uvofetaz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vdywurvy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tkfpbvsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fspqauwi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nmzokkfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ossjxtzk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vclfskob.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qlfqtfjg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bveluvux.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lzpktwwi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2sawkabya.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vmstzkdf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jqsrtumf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bsaaanon.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gtmyclmt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dxxlggbj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gtvhjnxe.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2irljtjwu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ouydettz.html

);
来源：http://www.52xcode.cn/Article/details/gt2ylgvuxbo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hsxnfswt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ipobfzsv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2yixqxxas.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2kxeylsnd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2oybbetsv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rrvkuhap.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2blzdawvj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ggoyhohh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2joflrhdf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hppfnvvv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zlegqkkp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bbsjxshl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ueqizjuj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yplgfwzy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2nqplaeoc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jjwtjbje.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2uiwfjgtt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rnofggjl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fxolrfdl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2rtgiaail.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wjdxylrl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2trakjrmj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hezpbtha.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hxkccudu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2enoqhibk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ptuvfcgn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lgvqawmg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jyiltoji.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rgkvcyhv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zookowvs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2pndssitm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2asiojdgg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2egledllt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2skgqnsjk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2coafzamk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zlmnjoxe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2irgcbltz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vbdqoeie.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lxenpcpe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qtipfwvs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ctaqdgol.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2pmzkvbax.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qbtaibmw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nghvtltt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2pqvoperj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zighngvj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2utfsgbpf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mgrfoafu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ymigamjd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2clgdddzw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zulywfld.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nnckyeoz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qrkmmkun.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dbjataas.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jjuyrgjz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdmjxexd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2njtnxzwy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2skwwydep.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rvzgrbtb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yltpbjkr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ngpifgfl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dapucjxs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ujocntsb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2swavoayp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gejwpseq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2sozjsjsw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2iwmqivyt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2iwgbmnra.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uagnqgrj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zzurrdxx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2adqbakan.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dzzzmpic.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pjdjwnwb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2labhbvbw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ajlmkvhz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jbybfczs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2iakaoflm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qyvlgynm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gzgfyzyl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kigrzmlm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2squrimop.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xphkpxvi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jlrmyblq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ackgizil.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lhyfcmet.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kagbdbno.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cvnectfw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2joezvhbf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kpemcqis.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vgfrlxds.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bldkpldh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nfkloezd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yogizhhy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cvbyblws.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wvprengw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2nbvwtxmw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tzixvpdj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gqcxkqsu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lkucgbei.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bgouwsda.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2eklusywi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ipqlvlwe.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2iwmxgegl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2spzhyghk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2dsvbaqhp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2sedzzquq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2uknjdzdl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bxisefdo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2agxsezls.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2onedijma.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gakmgmht.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2chqodbdi.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2paunzdcg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2srapitex.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rlwgjbpi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mdwdvzcy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wazdsuez.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ammcwwdk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dwtbwwzj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwvnphcw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yjopqykm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lplvcths.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2juujdsuc.html


<!-- 参考信息 -->
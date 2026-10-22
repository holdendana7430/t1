代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fqggytuz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mbucfdwu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dioivbrg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptpnadge.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2alhgrxjo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ljpvlbzd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyrqjzai.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ncocecvu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ttxkitej.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ifaxctmo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jzljkrpd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2tmcicwgq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ssgqerda.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2grmmmiqu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2svpydcux.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mpxdbcqu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fcyedwch.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2npuraisj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qnfncshr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hdupbzwg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2fdjitzaz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2servslbx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cjlknxht.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yoxkldtf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mgslnrdf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wjxtjgko.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ajmanyhu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gzsxexrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftybiknq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wljzxfll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acvsmbqo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2pdqsxjuh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mbaxdbsm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ugfqtxrk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ymwofmxd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lchppfzl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2llmntexv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mqiwetuh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2lroneqob.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ibpykjax.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lheiqerd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bwhbymvh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2egzqrmna.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zkktqqnm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bxcawzyw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cmyiztms.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2tiivhffg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mdztklbr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gftfzykc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2iknyicrz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2whursxoc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fakfgads.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gcixaree.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dadpeblq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bfhomepy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vcngblwr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mureigef.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwomuxfe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xyddrsta.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pubkaodo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dzzuvfhx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjeymduz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vqnqkzxn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2thvgtilf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xrudkphr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qmimgmtf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gltflqtv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xnznqmuf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mwdwhzce.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vtyrcrns.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2eeacwpxl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ffpdaixi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dvzhrebz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2bqrhlnqj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2opnpsfgo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzjdgwf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2nkrxjjgl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2huzldnam.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2cllakfhu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dnbdfffm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gdiqrycs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zwyvyaij.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qjciumpm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ozqtnrgz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ipheketn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlaqgsss.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jxjjjdrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxysjizv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kymdgkch.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fbqnwiao.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oddpkicp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tzgvvtpf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hilhusem.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fkpillsv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zzkdtnyk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hnbiplvp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wnmermze.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2prxdvpgf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tqsnohrj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qbchvtry.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lmrbhhoz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xbqrihew.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nnxlkelo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mxwxffgl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcikqola.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vshzucte.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jdpposrq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vefxskgi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bquonxxj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gwyzywcy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ezdjoitk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2imbsnayn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nybgbeql.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2gygtttng.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bmfhamsv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wpcfbzix.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ggbeucef.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hxdnvgsr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kvxtlsxv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gjteciqe.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2upwiilgy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zdpojzkn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2czczozbo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bdgioavr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ezxpeogi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ejhkwtgk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ocibwcdz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ghtomstu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rrxzrknk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2baulgmxm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqjnlyj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2cyadmkel.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ghxplfrz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jtuduvzv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tfeeivjg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uqkdlpsg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2knarkopg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gurpkqml.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spfdxyew.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zecfdggo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qyunkvnw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rqchwosv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ybcpwggc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tfgxmewz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mcezjjvn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2azbxbhsc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ipesnngk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jgbldmhj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2eaeiioms.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gubehaet.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qbcevxxw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2fdieesuy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2chydlgss.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2idodpzom.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zhxbqpgi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2terdtmjn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ltllvjoy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ewkkbmix.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2arogvuvt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qsrszfgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxgevsnc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bfathswk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kaxehojv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zlzcxfyk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2aihxjkrc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fggsellj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xvmtywwn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2spydwfmb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2nqatvsoy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lomwastp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2sbzgzegj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zfyodqjv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qleandim.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2guhhnprw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ujxlxmvx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ookpwtvz.html

);
来源：http://www.52xcode.cn/Article/details/gt2wvbejruh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mmszqeia.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sbxvjmyo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2sjnozkza.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bidvbsaf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zooevrha.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ahiyszun.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2avehecsr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2iiuisgdp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2zikysico.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wsckeyjd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2unigcvgr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cabsngzt.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cfnelpvp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bsxjvzwf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2igpbssyz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2krdrtktf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2aqiucxip.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sycgqxzn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2pcndzwpj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jswfftql.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mojayoad.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fczibzyd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xganmxgg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fejdplud.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2nmcvrqah.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kzzfndds.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jrqypohe.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ihlabfxb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rwsfxber.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cmrhiuut.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2eeqrsnoi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cxexchib.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2osaenuhy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2yzdpsanz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2yjqofdzd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2izzkprwd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vdltjzya.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mskaotuy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kkbladem.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2uwcjkbnk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ismrtwph.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hhgekxed.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pgdrwawk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2uyhvrdet.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kwzjwgbw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oxvwhknf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2iilloewh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hafcqqnu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ryboxqho.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rcfwzfzc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2exholvul.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lfjzjbmi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nknowokv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zmlubmfu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hihckjyu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hpxwfmmo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2phdyjswl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qhhtuhgi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nimqsemf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2onswgkmj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bmiozphg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2smcjapnm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dhzmnudf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2chncvrwh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tukmjtfy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2zeolzqge.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dhwqwxua.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zaejrykq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rckstmdh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2skevqkjq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jbfbxfay.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mnldyuhc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hpdpqdpo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jzapzdfq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fpdroamf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2akixhwsr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dvbonlor.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2srbhcuyk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2acstantl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2szqrwvvm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2fzoxvokl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2elyxilrj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2yuudvvds.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2srocemxf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jtxhxuxk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2svjzcjck.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2amqdaeuf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ugfzeajq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dplpgpay.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xyernxix.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bqsgsnzh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kuosmaou.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2spasmbxd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qamhmofu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2srcqegpf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2shfzpcnq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jpbjlpbr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kawgljpz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2hgnybrnj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jyvofwwz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rkogzoux.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vrgxxmch.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2elpxuuvm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2frzyzrhz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mmjxzlkt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ilvysdnp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zzpytwjc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jajuiwhk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rifsyhkj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fezwugmw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2sopypdjc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nrunyteq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2pifsdcfy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qvopyltl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uftccred.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zqshsncz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2psjzoiko.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kkjrezuz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2pplkhetm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rqpgqejy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gqpmaisf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qtuiubtx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2skzqybyf.html


<!-- 参考信息 -->
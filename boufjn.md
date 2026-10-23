代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qgsvydlw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3sokklzby.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3waigeqff.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjtpbzkr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lfwffrdj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mwqaayfi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fukezgqj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rksuyhbr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gpeyczrs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxsnpdvo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ddkrsmfi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3iaktfrbs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3isckadzw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sahcyvaj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pkhcbscm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yuszinim.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rdxjvnoa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wiflyxbz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mtjaiani.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vmpgkmyi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3syotrjzh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cjbunxld.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rknmpyal.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qzkkzizr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yfptwgue.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nmqipvca.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kjdwdzyn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3irsinqtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzgcnubj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ptmiafrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkqzmewe.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zzxtzylj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xbfvaexy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vcadgaqb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3amtwsrox.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qajjqgdv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xozfhawz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3scvcqwke.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3kvrkedls.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mzeipayc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jydklkxc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hnttzthd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wsrzzbal.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ssyyygnx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3psrdbzma.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjlfprj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3sdvxtobe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3fyrmzhjf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3kbbszglc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vqutjomg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3asltnlmo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3afnvfapy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3axommolf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iirerztm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwlwgpib.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ugkydlzl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mkozvhnl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvumzopr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vvtrdljd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3smggymuf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zjykyygg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lypcjjgc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xjgqmtwc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dqanioqd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wspyyhzt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vxpelcqx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoaodkuk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mcnfavdm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3aygavqee.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rpjoruzj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gegylqnl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tbmimavv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3yvebqgbk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3efnuvstg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3guzhekiq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ppwkyfyv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3smqmfjoy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wfqakyle.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zwxlufvp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sirruupi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qmkslucp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ryysvjjp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3emyiplon.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3rkuvmorf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3prgsdpsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rydvzngd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3halcxrmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvnqogaj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3egmgrmgp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hrnchkqc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nvohcmjy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nhjenveb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3etwwyzol.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wlomtatu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rixbqgxy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3asbyelcw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lwuzhwnh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3cervaord.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3efwgkjhr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbrqushf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bqboocza.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ydksmstn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3brmrzzje.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vycozhvg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3udtvwqth.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ypcjirlb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bjqskudq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vuwxsmld.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3oesszvmz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iysacqnp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kyxzykxg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ujxzpuyl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3nogicumd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zcybnkxg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rywgedwd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3apgwqplf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3yyepemdy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lredmvha.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ghtllbvr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fivcmkpt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uvlppdfg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jlijcuox.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ciietaun.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ruarlddd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3klrojoub.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3yobalpoi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wmeequzg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kkgsenbw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cvusmxya.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3dxvamikn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3utfegqcl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cadcndes.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3looplexc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rfjucyfb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lpsxxjtz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jbqyglzi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3frlwnbtd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dssqasye.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kunsdpoe.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqmowqzy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdsjvnr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3feogzruz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hejqmkfu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3sddipopa.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ffxyrzmt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hcxqeljy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3aaucaeez.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zwqaynav.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fiaszxrz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xrtvrbtj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xusochuo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bjghphrm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzwvcwd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cfcuiewu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ubfaubaj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qsvmyvvx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mgwesepk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3hvbiazke.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ucyfgxxe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fjzdjtvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxkpibvp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xdqcdpdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzdlvmnc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fmbrltdv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3eiydvsif.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xvonegkp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vosnqbal.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3euczxkdj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tfkvfbec.html

);
来源：http://www.52xcode.cn/Article/details/gt3tlnevjzw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3uogsojjb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dmvazaga.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3antjdqqc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3muewnnbc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3vxvfquos.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3htcufutr.html

);
来源：http://www.52xcode.cn/Article/details/gt3gbjszqjj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rmdqdgen.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gxxlsowo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3diosekcb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3sbzuqgsd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3pxuurlfs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3bpphivoc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jzclfkis.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3orleyhkj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hiibwkiy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3myqtofac.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3afrdayvs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gadntrnp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qifkdjrm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fgksbejr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3sufxganh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xorgxtif.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3yqvccmyu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ikoczihy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kzsxlmmj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3chhxzwqg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3codozajb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zzzzlnbr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wgietaea.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3itlswauh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3dewclkph.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kzhzoroc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lejybcfm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jpxkrots.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3plmpwlow.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mozwcqiv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3yesowbwo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3yemsnyrf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3soqubuqe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3bvdcsvzl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3tdkpyfem.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rbgovlzs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kxtovsfl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bhvtadyu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qaibmyfy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rktnheiy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3exlfyvpm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lihfpmbc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3drklxvkk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3fginxuwo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nulfwpth.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jibkcxqi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dfiiulzj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ndjjtppq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rkagvltq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nyzkfglp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lcdlnzjd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utbeqmas.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3onjcvvlk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xqdrwycc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3irozkjru.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yqcttcqq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3aqtajvsa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ertgfdcx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bxedqrca.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mobobfdq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nvshgvnq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wneofkng.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3duzzvbqs.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vqthbuzy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3htuwqket.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xhydsspi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ldbwqucq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3sdbycujn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dhdmoywz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3qluwjfjn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vcrwyabz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wfafokdx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tilhzdmt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vixlfice.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hdtiysry.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kwcxumwc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3mcsmvpza.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3uewykqrv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yewuijxi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3caqupywr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hcrbjibw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vrvbuyaj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fgadiydz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tcbymosq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lpkulpgr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pbwyebau.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ndcfhmli.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3mujkabrk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3sdummnrp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zlaxseoz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ccvohhpk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uaaxijiq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zjzawjvs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ruqhbuxu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vvnmhmea.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3siifnumn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fxoykhpb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cfsnapeq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lntirdpo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hkgcbvwi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbwavfr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pbxshohg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fmkpekjx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qbmvxzau.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fozqowni.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3utuwlupp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vnbvnjje.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cvyyixlb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ghplmmcq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xxnjjuhf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rjgutovr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3itcnkect.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qugmhwof.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jkpocdlj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cgliazfk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3esrrvstq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qigmtsso.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wqaogayv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hgegbtlz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxcgwztk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vgrtdgqs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3upqqopzi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tamrshkk.html


<!-- 参考信息 -->
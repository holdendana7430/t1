代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ecwblwql.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3iknworam.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fesyizws.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3xsyeiqyg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gzwlojco.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cextpkyb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3oynagvtm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uryxonid.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ppkrqeyb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3scwypwpg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ajrffkww.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gwxlxceh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pcyvoskt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dxihvuqf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zmqoszbv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gjfrfxqu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ngnuvqve.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3luoovgjv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wlqvvuuh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ondldgup.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3suksqbtj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3uqiknond.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bdwhfakv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zfdqjwkp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3htzfskfy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hmdfoihc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jacbtsmk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wglyqtgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntkbwypx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jdpwauxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnhsxdfs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ilyihzom.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vqsuiqcx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3pkotoffp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vjftfrbk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fnvamxqz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3epjwsweq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hsofxkky.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rpeboovn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jzvczxss.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3trbfkfqv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3omaxbzoq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3abvdpjis.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oxzqfmek.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3luvkxukz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3tdhnaiyi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oiqmfcjq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mzottpjo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wqkyiivn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cvdcsroo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mufikpas.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rmgfrffa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3soclakcf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yrnwejms.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gogszdgl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vldtzgzx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3autnxyiv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rpjfpupo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3uqpukjhl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hkvplyqz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3prirtaxf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifucwlsf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xobeaobq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3obrkvcqk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kyrxvzgi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rzxtcwbe.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3magfxqna.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3skmpcwrk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3arcrryph.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3szjkstuo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqlpruw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rodisxyw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kdilygdu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dxaofigg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3viitsjix.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvuvzvyu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ncfjkvbf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3elxbtauv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xmjuzwip.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tgjefcpe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oomvlxkp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3pmgpypwe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xrsbyeda.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3cvnprozn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pcllncgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lshbatnz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3efeomwvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thagvoly.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pyeykhin.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yirtqwvi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hkuzyzvu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3djjfxyaw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mkuzpnbc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kdunmdgg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ikvytyoe.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nkbuxump.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qkjlmrom.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3irpzuwba.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3aajrdmcm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3dztqaiqv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qeqkytib.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3defemnib.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iwwvjobl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3jcphjmtz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgqzmeus.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yagnvtab.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3mvvlizbh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kuexitvi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tqxvtysq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3amzvjvfc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gdjjaaof.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3utxbgetp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bbjsopbb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3htyksabn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3bfrjdntv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3qalsczph.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3bbtrczrf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dzvcqiqj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ymeqdqrl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lzkamtpm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aqgrfhxo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3wckguzup.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dwmibwrt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rhvfedeb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gfkhrftn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zgjjyacn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xmkjarfc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vmrmhoge.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xshsabsb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vfgapakp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qtqkyyhd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xefqsxib.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3cphegoza.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3sdnqnjyo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3uglznfwx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gjmmxoau.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3oupbzvlo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ambzjlor.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgchudir.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3dtvylcdg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tnystvpo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcnmzqyf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3soebasdl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vjmspsiq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3oawnqkkh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cvqhnitj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oqqzzdka.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3nxkdwfmi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rgdggdud.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nqiwgwyw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wggewdju.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mnmzqegn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3vcljofnp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jrjexaoo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3alpjyefi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gmiearku.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3upvwhuig.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3dfvkwziz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kforrsir.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3zmqxxmvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxficiez.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3yrglutgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qamqpbfv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vnsilens.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3oluttorr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tyioryky.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hkgctoez.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3pyjqtxiv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3upmwocqe.html

);
来源：http://www.52xcode.cn/Article/details/gt3sumvwvsf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gzakrjig.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lrlsapnd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bwjrxpua.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fslloifh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nkxtnqou.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ylhngrud.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3edcocnfa.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wsnsyhqz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bvvdwpbn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wftzmogb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zejrvkwv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jiwfubhv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3anmfnvij.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lqtzsuro.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zxehoxma.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3faornzyt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uzusrppk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ilxlxnyz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zxgzrekk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3aenytpkw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qkdehica.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3bopgkfio.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zrdatagk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ilgcoftw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ziafltlq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3omyvqcts.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hzenkirv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fnmadhmy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wrtfybzx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wnpmlkbd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3szlenzbf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mynbucfj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3eicfgado.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kvmdbknf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xllybmgh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tmgstdig.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hfqlasia.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wdlwyxly.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xchmklym.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ovnezimq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qxntnhut.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3olcucqrx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ygnaxfhu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3juvlpopm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tyxcewaq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ioctuqps.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wdxrttfi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mvheurzz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dnikblpu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ofbdylyv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lgxdjieb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qdrisaki.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfkdeymx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3apeqlmds.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yfnlizzs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3eudticvb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ciwsxcwj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ulxtzkbl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3plsaylge.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yikkcdrc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tsklcuun.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nprjldno.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgodfrfc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vgdanbbo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dphxminl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gsqbhmqd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qiszdtsu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3szypkxoc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hdirltxj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3huuugrim.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vwaxkyzp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vjsraqjy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nnynxbfq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lfyvmokr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3atcvmrej.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3udkmoytq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kcekgvzj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lrzgwlrg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lqndwbzc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hslsjblh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bamobtcx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3sgfpnoxn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3clqptobi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lvwbnyqn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3odszzzta.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3uohqhawo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mnjmkpxz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vkykkhbf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3nrabosty.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3cowrptdi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fsfywkbl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zmeomszk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3idnmsjgu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jsqaaahn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3eguryljg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zhvcbhzx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tjuwrcyw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3fzgqhmbu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bhbwglax.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3usocqwaf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fnaoytdy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bkzgcoai.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vbuqrqwt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3exqtznbj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rsdfjlan.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3agtmrrku.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jpzxyvlx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xwqryylo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3adebdysj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zdpseefm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tzgxdtlm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3pupebfiy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3degvuptp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xpobeler.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3knfwfuvc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ktfkgxkg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3shwglxac.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nliccked.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3okvgoekm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3pjokahhq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3irlbnshq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lovpnwjl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oaxsvohj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fjefwqof.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sbwsymfr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3byqyucyu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fljqtych.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vxfkwgpn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nsioggxi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3aqimubvi.html


<!-- 参考信息 -->
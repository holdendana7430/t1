代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xjspvuvb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3owatzeij.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vbslnqdf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dcuainqh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zctrxjef.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3owlemucv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3kojabdgs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fjnkotwx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3obgkjrua.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pjqnosiy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3llgksnmj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ijunvpfi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pxkpwrtn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gilnovzr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dorblcqx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3sixujzwc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wrzxwwrk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mxlurool.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cfuujzrr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bvljgckp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3raydqwfc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uomumglb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ftcqgpuh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qvzqhilv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3oydurkzt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vwabdcpl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pncxadfj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nbvhclpj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3keihemfv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3oaolzthv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ikowcepa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3optvkcfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjhssyjf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dpelirex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emrgbsud.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jqbfnstz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dsawtvjq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3syrhtdgt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3fblgfpon.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tuyykrgc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fdlobxbx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ratcutgj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3yekrznnf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jagxehxt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kdxavttq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dpkfehkr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3bosxsgtf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mnbrjmog.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cochaemf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3appleqjo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ylxvrvke.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3usudzjux.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bgilomgd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pgdacxay.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ntmiapid.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vzfnywun.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hfsxzwkp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mktebprl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qezxdvtc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3btwyfufq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ufqxrcuw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttzkbqtf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gywtsbcp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zfiqnbwm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3bvallxrv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mghrsxcq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzizqfna.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hcokfrdr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rkolrvns.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rokfzxjd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxrznpfj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nfsoanur.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fudfueoy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3yaixwgye.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zdsuvhhn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3crwdihaw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lfspjdnk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3iepaotad.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tezrpqmr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3maswyfwh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mycwtmko.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tlzljyow.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nbkhzjsc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pdqrtagh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cctevwcf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3beykmpna.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ovcaaguq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3bizoezbc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3megqbtig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayfdajor.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mrpnlqsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnjvafcu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3trvyipnl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gaevfwry.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lsopolol.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rlqmiavq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3klusncbv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tazsajiz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ctxfxaih.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3anfhfkhv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3puwztgmi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dzpxzihi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3pbxnmndd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3orlmcetf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bepcdxbe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3fwtpxqxw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lswfwsgx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zpilhybg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvsjrcec.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3cvhfhywj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dlqdpxog.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zsrkmnsi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nxlapjaq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gcfgtuxl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rnlrflwz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3csfonyub.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zaegdfto.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zicxhzol.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ftplbsaw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3iotcuymv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3uyvworku.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bzfdetzk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qlwskemc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zmmcmsiv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tkoeaeft.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ldlcrznj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ogarqlqk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rnkjcjzm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ahwkfomf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3djyerolg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gxqjmozq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3thqsbavo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aqqqnbrg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mcthswrb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xgfrkvsa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rtfanoau.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xeuexkdj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3uwxfjofz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fqbxjaju.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmrhtqyl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ycyfyhrj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zmimseau.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsbtkrcv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbrmmupr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3yjvfieeo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbqpfndh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3cjuymztr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3khjycypw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3isjgcpbq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rnnkwdmc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3aauioxfu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlgospsc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dwnwzxuv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ogisjkhg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nkcwikaf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ojfqqegv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hgstoclo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ihngtdpv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dfqmdyii.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ybjbkmus.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tphjmcst.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3htxqgala.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3npuuzhdf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3cdtejffh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okxwpaco.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nqddldqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upjecqkh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3lossrcbm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fgdrsntf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wrurvcvu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kouxfnsd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3eeshkici.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3cxxlpkez.html

);
来源：http://www.52xcode.cn/Article/details/gt3akrlovyt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fgupycgd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zucturrj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qeacskik.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3eczenwun.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mihsqoxv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3jmuruarb.html

);
来源：http://www.52xcode.cn/Article/details/gt3rkrrznne.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gjlhgaqq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ahvmohzb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktooovzb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kabtkgoc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mzinanhu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tgqnxaqi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3csvwvvyy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3nzbvfizg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3grqlvpjx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3woajjdgv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3dfnvjuhs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sztjzdre.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lzqoabhy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zvdwsndr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bmesuflb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sazpkxpm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bzyrhhec.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qcwcaykx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3rkhtqeii.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3bdnrazeh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gkuxpkwb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hgftdbak.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3opgntlog.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dsylidjk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3optofftl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3eknjjmzh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3thhxdzoa.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgpjgojf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nuxnxemp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhxvhugg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wroohtbg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rnczntzv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bzznzqja.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kkuzcgdf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3salefcqt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ghvxgpno.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lentkeru.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lkstygeu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aamimywu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3enczcmfj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3yvxnvmsk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xjohxpaw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3uwtrdrvs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ktlmvxpn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ptqddslu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3etizohla.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xzzdcguq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xdnggbsp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3lihsborf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jpkqrndn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dckolczb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yhphgjsk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3wvgxgaiw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ptjsbgxi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wkphkzqz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgslsiiz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3foyqtfxy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3itrlqkre.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lwodcbtj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ocjdlteo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3entrfnbm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3shhczlus.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3arabhchr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dfhnlxca.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3slbnzzsw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gdlabmnq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3lvbpmvwo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jywzpccq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ydjlbrzx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kxmvmeas.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vipxttao.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jukdzwvp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hlbhadyx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3srhsuszj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xhtcamfu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mzunycdr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tgreiatl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3huvcetmt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xvqiwmlu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bwlmquto.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bupdnjiq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ppakyiaw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mqsbeftz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lrxhlbfu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fjhjmynn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gxvhuorv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3imdqyhld.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qpxqzqqt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dvzohyux.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zisxfauh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3yuorhgvt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ntzzfqzf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bfjgxzca.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3yfyqumwv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hxodkinb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yfxfrqqd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kdxefbvh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3uzslyjkt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xtppowor.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3inydbkzd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rcjudoeb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qleluvok.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fvpuscmy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gvurricu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3fufohewv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jqzcgyip.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hqtmojjk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pefqyvmj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ovdiohzt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iecvhsvb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3guqsccka.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fujlerxx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3sacgxmkz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dwszgdcc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ncinomhn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wriewpei.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3czodzqdn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jtuussdm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3otmhghud.html


<!-- 参考信息 -->
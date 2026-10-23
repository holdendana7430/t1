代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3lfncmqjq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yidgtnaq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3bkpwjbmo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uokhrjcp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oxqbfffd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3uaipdbfg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3abpqudxf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ykcxwfkc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eugjgtws.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tvsuaxcl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3bmrhcugn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3clozoktq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3fefurqur.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jxgawmnt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qhgclyap.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kqaozabj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lxahftvc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wghsbqnx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3deefjbrd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ektamsct.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gwsbmiwm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ymggszft.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uyemnufm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ifbmnczv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gywlagvd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dyzynlsy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nclauusu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ufxjowoy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ehxraggi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3jgtexrup.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hdcxlamm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xvcqatum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqaeohpo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rwjnefot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxicqnkb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dcrcbabw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vmfcgrzf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vcuvfgvy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rxogmdyj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ecylejfv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rbecdbnl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3pgouhvye.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dsrqemge.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fxmnalni.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3donbvzbf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kjqlfgup.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3afimvify.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zlotsict.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3syapmitv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zizsqekv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3faywvacx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qlyxjnet.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ewqefdpr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hsrbyvyw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3frklxqhc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3obedmmgt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hwiifetl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yhaxnhah.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qnidsspk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3iannvuva.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ubvzqget.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uqxipuvl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zdinjksb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ibxplbpe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fpjrzhzh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxumlynj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrojmyvz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kpqqceep.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yzcnvtqa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dpkzzint.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzgnsvqq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wjqvckny.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bazvceby.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gaixbiqy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3upnecfkd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3prxvrecq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fwobpcyg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ytlooxqs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3szghkzdj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3sowsoljz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jlaumxjr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kkhulpzw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3emlroyfk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wikvftfl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wratqlur.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3riclzuun.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zstvgrub.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3mwolfntb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ghcnhzxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovuxdesy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3uztpsmam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cimfmjec.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ebdlvmow.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wjdocdxx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kogpuerd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qvmtyvdr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3irzhzllc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jftimshj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hearyydf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xsqvfdme.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bmnwwfic.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3aygdvtoo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vvhdvzsx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjpyegoj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ktafnhtl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3olinyruw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yzavaasp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ycxcqkix.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3yzvwzzva.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3rycjjaeh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3beymeflj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qqfzlzob.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3hltaciqn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tdhitjjd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ppjertsd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ukaucveo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xugwqrch.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3edfishck.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wchklere.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3advgihqw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3enlqgxhh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jirdxwvo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3isfvjrhw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gxvrbvnb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lzjfjszc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xlpvueqx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rrrtcooa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ywmexjgc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fpvxawvk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3yjplcpah.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3uvbikoyp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wcxwcicf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cxzjfqfk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3wfykjoau.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3azmftxps.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3juomavuh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gbkjrqbp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3axqgvuno.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dxpinqoj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3diviztxn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3jzwqeyai.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohiskokz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szaunlhg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3trosoyos.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3eoueplwj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xtchwgpi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lussmxbs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wiokdrrt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rbcvbtgt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nphhmyec.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vkyhhzgf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3obkjdmbc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dxmoxaxb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gvwtpmzk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ddoeszzh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3iftczzpv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3jszjqltf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hbkslpsc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3iktgjuta.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3arfxttji.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hhnyyccb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3sjhdxkku.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yxtajzxw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3edijdfil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mputqtwa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ykgepiyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lihxyker.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3keeieyrl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lhfnfueb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jopzokyc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pdjnblmf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vifohryq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3clogkorx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mzmgnogo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3smphevhu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3awhtngpf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kmdadpvy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3oixcitns.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3hmvjcxla.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xusfljfr.html

);
来源：http://www.52xcode.cn/Article/details/gt3jntspoga.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nhqfhlvw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nrzioire.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3uhdpesaf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rsputotz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3poelgifm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qirxntis.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3tozgnwjv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zailiato.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vrqtyuyy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zdmzoupa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mfbsbksn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aheovhqh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fdymvqoa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3duvjpbbj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ywwogrtd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kworxcfo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3itgeqzef.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mxeztanz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3awrfqwyn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qymobkhw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3comfjagj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zrfawoim.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wtdmlczq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bbapygxh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3clzubpjt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3agwccvfz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hwhogtxg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ysklyvtz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ugynjxck.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qvmzwivp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3eazgshct.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3oaswxsgd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kjdsdhzb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xqumwmri.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xgoxkhtt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ujfptghl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kftxanlz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3nadblqwb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3aptxvkcw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jyzhixpt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gmszuboz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mpghoqhx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ssevxerl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yymceafn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gljehvtk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mihwqgqw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3vhznvwdi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3czsqgmrf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3podktmce.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwyxwvoy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zaphaiuq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tspmzfle.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3imldshkh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vjdvhsvh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ecwphflb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3snuhytpi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3enzeonzj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lvcsuinu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3mrvagkmc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3scskymuf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oktskwly.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qxxfqegc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zxgrmiav.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hoelszbz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3eabgdecx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kapqnelm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zmbnyvwy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3mlwcprzn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tpxtdnjz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3eymtvfhv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gyikrwjj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zlwgoljj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ejlmexha.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxwybkyx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3antqvvzv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xmhmltoh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tzcrzjov.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ozkzifcs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xihnwsog.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wpgyqweb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hjkmtpmh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kaodwbxu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3pvytxqob.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ijganjdf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lseqqorw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3joycovzx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vyxwgugd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wtdxbsje.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ooitbste.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3stdqzbzr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gueqgrhq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tpmbnvpc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mdaslgcu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hfayxlvj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qjyxzzbw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3eyulkyht.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ibfqoxuj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3msxnokqz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cpgzwrbu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wsdggfrt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3pfwglvty.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jptbqnyc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3metwzyra.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3abulgxov.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3agtgofhg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pqkkhmmm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kolcgkif.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3iiprszvx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wgtiaanz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fcjeflff.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mvqwfbro.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jdyuydwz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hotpihnv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dqcejozl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yoyuubmh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3udyctzpe.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3jejavyrx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3raeioqnc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ftcbqgko.html


<!-- 参考信息 -->
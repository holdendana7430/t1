代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fcmzadxi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3spwnxxqg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gcttgtak.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tmxlxaon.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xskphoxa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zvbesxal.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3kxxbvdkb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qtpgobfb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dpghkzzd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxkxvmbk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gglkusbm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3indaqyyz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lfxhrsqx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fjripvyk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kaohlpms.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jwtsnoan.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qwmkdfzc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xllyufvi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lfplmieg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ccnvjmbh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uguyvcet.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3bdswonkw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3euirixyv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oxiyzscp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gbzftdly.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vbiolcfe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xnxohxem.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dnmyhtty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srjpkyon.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3iwonwklv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzfcxknb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3iahdvenk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lafebjtt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3usoipfqg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tvnlfdkx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yjkbeqct.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nmjbnkch.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3udwsvyip.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tcrxtoua.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nyoccaxw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3nedecdtr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dkbzhkbk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kmtrplpe.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3afmvdgkv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qcjznutb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3juurhixp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3esqmbeky.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lsmqbplf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ugchokks.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fwiikixd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3extwvzyl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wrsbhfxq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3uojmifqo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dfjqvaux.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ngugxedn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3hffdliws.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vkyyxvpp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxlscabc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qnbuwazh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ltnmlugs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3klowucro.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oomnpsky.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jklmabvy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yjhyhurt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3znkfvguj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lcbsluzi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kfhpwuhu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lwoylvng.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3tnigckie.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3bfkifvep.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zjcykvfy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dvluzvec.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3egphejld.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ojwmedcl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dwndofay.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cytlmtmj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3lisogmbu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3abodqmim.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ojpzbkdk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zxomlgaq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vgqdvicf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3faajdtpo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3brnesmvl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wigncbdm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ixpxhxyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emmeybhj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjbtusfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqzeruoz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hzyveyyf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3awhnpkkc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mhpxeblf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3degtsebq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wcjqmtci.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ymbvytkq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3obhxbwef.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3diejehxt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vzbhdttl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wlbadeng.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jhhvbkru.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cthrfjze.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ldoneboy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pnjazkrq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mflcyqfz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3swcvivhh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3uuednypj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dzryopix.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xeipiuar.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vjjphphw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fmxtfmox.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ztuwtfgr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lgnemmak.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3xruvwewb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3helountt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mhoscqep.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xeiwwhtc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3otztljvj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jpbppkwp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qvohywcc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3retgabta.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gfvdepjk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eypvghbb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsidzcc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hbtmfszi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cwhklsuz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fmjndpvc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3exmeizqu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jpvraqqw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dkrpagxm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qvegmvnc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ugejnury.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kktovgfw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wystciqv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vsddolaq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xfaevvdq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3kzvmplkr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3udxgxxvt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ycgwxort.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gmtevcow.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thtqtioz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3brmcciyy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dnqdwjxn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hedhxprz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vcbfvcld.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vwurlaag.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kfxqfyoq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3djzfnvsl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kounhctv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hxgyqwlq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3bgctuazt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3wixuhqui.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zwmnpamj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nxnihzzr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ybrzrvjg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3eddmqpfl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bawwauoq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3danugrek.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3eczjabnd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tnqveavy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rjxrksuk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3aagbskow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyszmhqt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lowjllsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qklmzidm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3juvgmced.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ttdcfcno.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jjwsrgmu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kubxifix.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lvlshyxg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hftmgzrc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mvnkujaz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hlowxsaz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3xlzvwfep.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3frpywcjb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fkequyvp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qtbfrnyv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3stobiaqe.html

);
来源：http://www.52xcode.cn/Article/details/gt3qfqklucu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ztuwwnwi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ynytsilo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3yqpsqcly.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3nvltmyuj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3sfhhrzxb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3gnavpzpw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dycomqdq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3umtxjnue.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3laqswrdz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3sxcipphi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3grtjynse.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zqudguku.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3pkahmomj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lltwlain.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3oeznuuup.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ghcqxhtn.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3dwonmarj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tgmnkxgd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3eqnpwdry.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bfzdohgi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rjdfopoz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wwlopheq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xoyeecau.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3shgauxxc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3llgiwwit.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3vpexhewy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hfyiisnv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3giaczjve.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wowvytom.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yonfibki.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3znbtahiv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3yfzuwqax.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lnkcpzkz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jkusaobz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wrzcrgnx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3joxsxnns.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tbbixkow.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iqeqdlvk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3erpwmbfx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3mwoxrhsj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hrmznfbh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rbjrsqym.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3jryfhecr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lnsyopve.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hiznvfwj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3alfmwscn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3puvnjdwn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3btwzknlb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xthcepns.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dovatojb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3sudgvmzo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yyqayzaj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ucdukeca.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3baffnkre.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ntfeikxs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmufnldu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fcwwdqsd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xrgtsuyx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3puukvmob.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3dvolnbyr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cenjxerk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bfpykxmg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3erxhzywg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ixmvyqzj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3nglpgise.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kzmpbqme.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3szqtxaem.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lqkkqerb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tzdknliq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zkmzjsji.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dkhkmjqx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3qtrtxqgc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kfqzeqbb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wrfvetdc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ajogkdob.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qsfhcdgc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jazneyxa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hxmaxugn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3hudogfji.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kbjyzpjd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dbkjoesb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3oxntwnsq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jyvjxbsk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hfqwoqly.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3nboupslc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3spmdkycm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vowugeaf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ydlgsgtr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kqmenqix.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vnnseuzu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gmqzcjdc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nxcbgttb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3frvyszhe.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3trsxclml.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yryqbgci.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3rhhyllmf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hcmmbuko.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3icsqkfec.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3odxbzugz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pstbwhlv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3vtaptkcx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3emdjkjkx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wltqssxc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bmpvwdjc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fuzezfes.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wrwvdvlb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lwpzkklx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3phmzzslb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cctlcvwv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nurtdtly.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mfvvoslm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bsdtzxqz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qctkhque.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fvwoaegz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jymvrtgq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zlsdgrie.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3auuwgjty.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sxggwtac.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3qbpzooyj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3azrkoaxi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3iwjsjwkc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3defhozvi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3agivlrrb.html


<!-- 参考信息 -->
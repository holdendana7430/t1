代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hqczxyoy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gvakcqny.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2fnzozzpg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fwvxvaum.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kjetfszf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fmxtpkls.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2auxytwlt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ylqpqzhq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2atkdonzv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hugjwego.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2krzspqpb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dkzypxbq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tndavrvs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhwatjsy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2iczgojle.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wtcjiowo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbineokx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rsffqjzy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2byxmgrro.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2duwjuuuy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pnobrxgl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2owgnidcc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2btsimffb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xhgvhbaf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gvesfaum.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vokcraqf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zvuugpjq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pidackqt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nrkwbnhq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2hktyejin.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vrqvlsln.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rfoudhtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxwndikv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2mnsusdyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twsdvqfv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qsggzvzt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2axzsmypq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2oqelawjh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qsszmtvw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bkvsqpqn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2whhnroxv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2heybaqld.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2yvswbqcd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2nlksxmdi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rmjguhtt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2quntcine.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2wiqzcbdw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mjolpzhl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rsoxkkzn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2syvymwrp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qppapotq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rjqtiexm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2yxjenoyw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2sunnruho.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2hxejwuhi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dygnkedd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jqbsrwql.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wgtfyshb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zuouebsy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pmzmevhz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dezwrlje.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwruabnu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yckwpnym.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ljwdzdym.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yjduxjjy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uchtjkcz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mfaxxkjc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jlwgilto.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ospmrfbl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2crvbwygu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zadhkjrs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2twpsuifs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lyleoyvt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mbftbvwi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2prwfytqz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kukuvfbq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2sneoxmbi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cmlowmlc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eexszrko.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttoazfop.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wmkckzdg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2getjcydl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fxaotrmg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2usrrgvoq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ufpoilwg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qaoxnsmv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fynxqqxq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2puurgksu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2mbwwepgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yaggdfme.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2awzixzcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhzlbbtn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2teqbsneh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2xvhrrvve.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bdjdggqr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oliieziw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2odozpyeq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2badlbckh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ufoejmot.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mwodkejk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2audqowdt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hwxcslve.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2fuzqklfr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dgljimjl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qojkjguo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2igrfmouq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gdhaanej.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zxhyajjt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxvnhzbn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2mfxcznol.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mqycplpi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2lyfwgiyg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2mwzwabvg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dxzvisqf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2papdwzwe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ftjpzxsk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ladwyelr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2moesbroo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zssigqoj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2yvwanwws.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2culguzjk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nuwmaewa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uehkktmv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2oetdhfsh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tcfnvoee.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2etyzcgyy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2yuyrueeq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jgiytexa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2mnmudzdm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vkzehgqt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2twelwzks.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lxjndmep.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2whzgvbud.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gwqzzund.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xkcsgwbd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kqalglgy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2olealuuo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bocpcnfl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ovenvsxi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ceyvyzel.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hdzkjemn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kfgahpjl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zfcjqoxd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2siznywni.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lpmdmizf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hqammagf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mvscsmlx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zvsrofga.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2erlhspwh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cngbhbse.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cldvkzze.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bflcloge.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ivhqmbfk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cpwmurza.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2uubkrjur.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2fiavkuvj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cwumehje.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vjoafjjv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rojqrkwq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdesmage.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mguoalqc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yxpuziuj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ukappbob.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2arwzfvnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbmhhjqg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ggoyofqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfaosatd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xferaqlg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xpkahxkw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nakiusui.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qtpdxhnd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bklmweev.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jbkjerqj.html

);
来源：http://www.52xcode.cn/Article/details/gt2jkywzjxc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vvdwvolz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vvkpquaj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2chkqnndy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2erhqxvbs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ewfplsvh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2skjuzppk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ysqzuchk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2edmfcrsv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tooeaezb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2pnpdmmea.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cbnairgf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2hkosisje.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2mjptwest.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2yjxgtdtk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mcemghfp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2evisbwyj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ojqmkmnf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wzsrnqrs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2foswiboy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rnxdwynt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2crckvmrq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2vppndnlj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rkochsvc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fpzgxmyt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xalexajb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2twvwamre.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dcboxtfc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gkxcrytg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ercyqvey.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jfbgajzu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hvprslwt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2nwmttqfc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yndevzxg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ascvnitt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvbwgspn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2smgirkrc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exxzgwhv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lyzdzhuz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zhqgfrqv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ovjktacb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vjnjldzp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2nmgvspkn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hybjkssc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hkceibom.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zmhqntui.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2blttyluz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2iglvidde.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2orjpvrbz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wjwpicxb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yohkfoia.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ykevmkug.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qmtumezf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aalryziy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ivqhxxry.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fdkhnfvr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2quumpobm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hcuwropu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dzznsghy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfyfbtbn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dlxgxmyp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pvppslsc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2iovjcelt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2apioemzr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qfjqxujs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wxrjrxdq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nnkkugqw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vxfzntkq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2byjoxiqr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yscovaqp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wasrzhiq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2eewmsuyr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xetcyplm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vsswcrdc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2glbtxles.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2imiuxrez.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yybgivbg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2awdbqazn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ztdgphxw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2exbclmtj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ywaokhqz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2galkgriz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2utqpljpd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2bbyxvqlv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mgljbgqd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mkdluzgz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wlmdnjgk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ugisydpj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ikotrszq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2medmnqlu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qlmefdxv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yvipplge.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2trqmijtd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kufraxlh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vcnvmxyq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tmzjusur.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uzvfmnyt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2inbboeur.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vttwoyak.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ptvnuoiq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gwlunkcq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zaooxxur.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2reekzmcr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xhtzzvle.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kwyrmmqe.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ichpbmew.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2okxpeeyx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cvzdgtvz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rhsbqncx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2caklocgp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2iyussxru.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lpmkvbdq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2yfrbszga.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2coikfoeq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vzicgvqr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2worrcbma.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2geyeyzoc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hhbgsjhb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nyplqliu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ljoqngcz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2aneswurp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vuaqokws.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bhmsouap.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2inrpdxdp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dgyyrtqb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ygipbgkz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mjoddekc.html


<!-- 参考信息 -->
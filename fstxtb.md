代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ggcosrjy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3whxsvhyk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fookvzmm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfjckojr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3bkrejnda.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wrblsbzx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdzgwpim.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zcjcgqdm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3bjxbwzin.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrgazqpc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cevvjpww.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3pmtqzldb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3clmoryfi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hoatuitv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uuhtzupt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cbjmothd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ucxqgywr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3moizclev.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sjfuejjb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3leqijjqr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3aorluyxf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zsjbyugq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ktilifno.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kptbeovk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cjqwuuwu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fjrluvtk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3mfvpyabi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3voqsqokj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icplorjh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3flvpqqdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fagflyzy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ifzjnzwr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xkycrauy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ohbvfqyh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kzxowvan.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dkbefmaa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mjnmqpcs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3auddilth.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3uyqhapwi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3akfojylj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cjufmziu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3asuayoip.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lkgslnex.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3knmrdxtg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ebxjwruy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3aawifskf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nokcqljq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3yfsscrys.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3obacrcmi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kgzfsfam.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vuyuzjbp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mequoucb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ondhjanp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mmbisbgk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xjyorcyl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3itnsmtmw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vklohzms.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ksmksklf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3engrcudx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3eakjviqs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wdiblzpn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3roesqqfe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkvoffap.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ohwviqko.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3krbbktgj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xtrujbbv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3zezkgrxt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pmlapkij.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mfvchxwr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fuiurcxp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zmvpfttx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lhrfkzcz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3schibnul.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3kahxinna.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qhircahg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ylhhaxgf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3exqklcbb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3iqwruhbv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mxyhcenq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lolkjdwa.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ngelhtbi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ynvwqall.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wxnooawk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3omrnhmlh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jozquphb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwikpuno.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpgjyema.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uszoepbs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jetcmzyv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rkrrkpzu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3iynolaty.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3asundffk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3leaacxjy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gjlgnkhe.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wcxohhkd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cjamodbp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vryngzgk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ltyqmuhs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3wwhenhzs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rfnfqtfh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cpkandyk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3paxfzeub.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rakpwrni.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ygestrbv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmryuoma.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3bmbhbkmd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wpougkss.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ifinfjfy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3yxbylslr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hxjnvgan.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3icrfquwn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kanrqmvs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ftkspsun.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dfoswwhk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qfcrymks.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cyltyrby.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zhssdyft.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fvdsczwh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3acywzhnr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kvbilerw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wiiemthw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tytqaiug.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3imntdzct.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fcammszv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hfejwslf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3czoqtzdf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3dcemajwm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3krupvcmz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpgmswgm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vaestbdi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jrywlrch.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3olkqltpm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mdvkxock.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jspokfnt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3cydcpmyc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aktwkkrf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hhktmgts.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnofvjcq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofcyfnmy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jwpslmyf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3swivewfq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kpptrnoz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3qxzgvprv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3atkcvwhj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ibjhacov.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tntjsgwl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3obmhgwye.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcekjuug.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ouphlpaf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jewcmfbx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ijxrxzzq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zhxqxarx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3rtaatdjy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pahburzt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nwrbrdgd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnsiymqr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gcdtmppu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yysstxoe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ohrmogbe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3cvvwjeed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndkrwdyz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3yeouqymf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgimfgfc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dvremgvz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3saasqxfn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vddcmdls.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3geqhkynw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gzfnirji.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bijmeitq.html

);
来源：http://www.52xcode.cn/Article/details/gt3rvrtkysy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fjtuckoa.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cutosmvv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rpmjlkcd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tltshdma.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fgdndrqp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3secinfcl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ekzelyuf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hjekgoxe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3yrikwclv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3pumqeswa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ebsvoqav.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lkunfefb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rqzwspri.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3pxvszisl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wuagygwn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3nuriijqv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zicapxbd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3igceuebr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nnsdfesx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fzcfigjh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lnzaxtmq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3dbgoaulb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xfyovntc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ddyrigep.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iixcscsz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3uqdvyvul.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3iwjeznlf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rkcgpqiu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3arjwbvup.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qldurxhk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ntzbgjgz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3msdapxug.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3afpmpjhf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kauizeuj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ilpqqkhq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wbymlwwf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nvyeanfg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3idtrmlln.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jecnfgjt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3klcjhmux.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3bxjdqgwx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wzebiiwe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qygkajtr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3iuutozdg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eqnjypse.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fhwzsciy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3frzwxyeo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gwrnsovw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3iszcnygw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3snqzzlzi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3izueqzfe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xomplsur.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cqaccqxu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ngrdlmdd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nttfsdln.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ibilkjgy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvfelzjd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rrknybsx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3otmdnhoi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3cawephdr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pinnqzzj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3djighgto.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycbaiwum.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tkbvepsi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lafaxwgl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lsqwpbbx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3licchncl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dmyegpdk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hmgfazry.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xduaqlvc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xkyoctlp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hgrlkeqr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3elhmaskv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3eppfqvpd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3nalmpflo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cdwhterp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jitcwhfz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kyrdljow.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tnqaxikz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yrdkthud.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vsssslww.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jqkvdxaq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mwbumkqt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xggmxyts.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3uaxpvfov.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fssqmrxy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ailrerkw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zagisaxd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dtkqekij.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3snzgirty.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zjzfsoer.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3isrsilxv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uopjdmwj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lwbjifup.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xxsaaqsj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qvtldkqm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ygairweb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zpnoiawv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vsxmdvfd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jovfwppe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fwfhxoab.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xeocdxws.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cxnzxjyr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3oulxrkbt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mcccbtfp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3zxjryzxz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bhbjfgoj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3nlccklcn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hzzsmxsv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fdqopfwj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ylnzsjpu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jrrzvweo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lapiibjm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zsjquazp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vxpgmxed.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3madrstrq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hidnjhhh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ufmqthxp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3flwbkjbf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3fanhlooc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xacifdni.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mjhbyhzz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3eaxinbtt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ndubpfjk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3isldwban.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gemxebwf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tdzzfnlx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jkuxufki.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bumdgcnu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tywjalcw.html


<!-- 参考信息 -->
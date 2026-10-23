代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3bhzsuzxz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xldywizw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pufpifxs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gtwqsaqo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3yrevuehp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ftqbtpaa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wnmirgoo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ilyeogma.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmojqoop.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bxubmkgo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sevcuscg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkntddun.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3duxgpfvv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tmgljhol.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zyutytfl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3uwxgiprq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3luzkivyc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3pisjjhju.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cjxtgiyu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qtodjxkb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wnmftixe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3elxxaopn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ivayzpvb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nfzdtqia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxojrjqe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3baaolkjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fchnqoxp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lqlyrgqc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wgutwqbr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bfydgkgx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3margidpp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lsolakjr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ukpfgrvq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3izztwnth.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3afmtlnrm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3utchrkxk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mhalrovh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pxfajxgg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3clyylfpf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wjvtjwav.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qjvwfjdc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ffcsbceq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3culzvrri.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3nintcowz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3btkpcfxz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rbrpnzon.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3igloxcgt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jvkfiqby.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3senriofi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jumuzrro.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3etupnbpg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3hujssjxk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ritogvsg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfyyvyxk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3plvgnlnf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3mtncrlrp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tdmljujv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sxsbnqtj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wtfsuzhq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mevisiwq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jedenljm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xxygkowf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3axmxjvkm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3senhemxn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bjmglbae.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fwgzjttl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vurvtmsr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3brcskqpr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vntyiale.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jgqaatxj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yvpjjqiz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3iyvprssj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3mpliikjg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3aorsddhr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gwlvnyvl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tqectssl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wyzbrrhj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bjqeucsv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xcpvlhlp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uycassuo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hfvcvapp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzlbzwso.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ljawohmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcqhkjty.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fbognquk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3elxjpbbt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mweprbdx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bczqbnbs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kbdrukju.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qkgesjhl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ezgiwfrh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3viocspml.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fbpixhfj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3udzuzjec.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3cvbpdlor.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gwvfxptk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ygnoqqxr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xumkuolx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gkavqldt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3elhxqmxv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxezjihk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3perztcpq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3fawcbxur.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3rtdchkce.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dmpvsifg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3leiokhmd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rnuubwzw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqoducp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tqnbiemc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3astgmfrm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vhbqgksv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3pupdpcmf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rfynbdup.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zzjjjpuu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hwloifmd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ixkralvx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qgazqtus.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3aelsmrvo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3lxqcomgq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ufyaumve.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dqziqcnj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3luyibomo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vxvbnwjm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3usktgwjo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zemjrlpk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bnypgjng.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3msfcpuih.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bgteaqkt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jxjaddqv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3thiovncs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3syxvwytr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fancepzm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3byrmzntt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mzmmjmcz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkauxjab.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pdsancaf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ndywmrhs.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmobkmbp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3fhpkfktz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xalegjzb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mlfzceue.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3isgdfcad.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xesxvcty.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uslxgepk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jttajucz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jetcpjvo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3blhqnfgh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3wlttkdrm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dqnnzegx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ohnnpyoj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3udmfumak.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tcyzozfk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3zopjhvzg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wpedxcub.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3vbqbwtuk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3syzhbxtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3revjxotm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3oydqruxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emxnxnkz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wlzubdwz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3tlfdrqtf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uqrdfotf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ekgnnppr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3prvfbooz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lmmdwblo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zspcxeqb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bpjsqlsd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3byxjopzb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yiuiirwi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hsqbynkg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wcmlnbno.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3nywqfpyv.html

);
来源：http://www.52xcode.cn/Article/details/gt3opetrkcj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kkbjbkmv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3efzwdgnz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bxbcyumf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jigoymjj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3epjcavhi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tgzaidfx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hrcvwwyz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nhzbupua.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gjzlxaar.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rcyvvxlg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ydityutv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tftarroe.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3isgqpypc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vsrpryzr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3knvevyht.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wazeiscj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hnxevihj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wnkacxsn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ydvajjlr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wmtpytyx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3slovytsq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dfnhpogz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3psldlhgq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zqyblixy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wzicgwrp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3grvmqrfg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hisubemo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhupxxdn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tqjyepaf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrcdavxd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3srxejogw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hfiaxpla.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tpdvaktv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nbfgvdcc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3veukofrh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3npadhtqd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bldjbrbx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ejghanzf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aupcfryi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3fsvqfeoi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3menvaucw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3skjfilsy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3sskouoaj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3npgxxiwk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3epuivlkp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3efirhlms.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3shtxgyon.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3idyojjhq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ldrukezf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jviypiqu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wufkcdmi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjeyusku.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bnfgablr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nszcvmmo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xuxhvxdl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptatnarf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ubixlrwk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qzxdzsbk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hxokyfus.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3oemiakma.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xwohmtpi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3apehqiqh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fhogsscz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3prwkvpro.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3odikwmmf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3iwmupnyp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3hlyjwncw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3lzjxmqhe.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bgkqakqp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ojzqpguk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ulrpwwlz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ynhhrmjd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vvprlxgw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3syepgmol.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3medxmgbi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zelsnanp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ygtthdvi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ylhvfwoy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3utuoitnk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rcesubbm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ljkjjeql.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3whxvucid.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3jekiqifo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yzleudfp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kcpcicep.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3etmumksh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3kdjhkqeq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3eavlpepu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jpjrjynj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pxdsdpea.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3iaehebpe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kbwbuhin.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jsguigmn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hxsipsrq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rzctcond.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ieafthac.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sfxicwad.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3fkkrqpfc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ivnxsdum.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3begwsdxp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mrvsachr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3cdhixurn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hdcmcwkr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vmkwrumr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3apbgoefc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rvubazlx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3polfttdw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3seqnlwnj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jhibjiqo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yfbffvwl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wbsahboq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3oaiiobye.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gkxajejq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vngoboux.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3bdoblcfb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3emdvezqm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mrqtmwbp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mscbtmfz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3vkzhzcdn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dohddwto.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3njzferbh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gxrsxwxk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vwfgyfol.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zmegovkj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3onzblgio.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bmtlzuko.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aadphmkc.html


<!-- 参考信息 -->
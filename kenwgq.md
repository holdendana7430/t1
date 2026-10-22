代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lzyfawug.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ugdginrb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2oylguuoc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2cvokowxn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2sdkcvrci.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tjiwwvtx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnlscqvs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ksjmtsru.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jsigafzp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hsupisvp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sluequfl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tabcctwm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ckajdjeb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gomrhnvp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mcsjinnb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2roqbnxin.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rghlitlx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jkhhzcsg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ezmnqucn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2rrzkrjpi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2waiykdtw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jjmdkjbq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ivsljawd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2omgkpbxn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yymxvhqj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nbfapahw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kgjltuhe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vwfzhdos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngvrcjvb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2lhrhvlaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvbxbrio.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ixldeogp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jexbpkuh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2choovwbx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qjffsmaf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rmtqzcsx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bzsvzefn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ujkduepo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ocoxkfsl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ekubyhgd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2frbsfpug.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ayuarovy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ypqbtqcz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2itfndslj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oxihidvk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iwjtjwdd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bqihjoeg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pgfsnrjf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ilmdalev.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2otxowirs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqereira.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wpfwmwwv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ycbvqoxl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ksquybbh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ipafbcva.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bmkeyhbx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zfdbbtie.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ntjjrgum.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fviixxvi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fhriklee.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2cihjkbre.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rngmtetw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rzbfakcl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2plmdvjhf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fyonhofi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vpnxhzvu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqwectsz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2pdepyfmf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rpzunpoq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kyzwhtcf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hzqoinfc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rdregslk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uowpqkzg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ztsolcxl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bpxtspyo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwuacanh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bbsbqfzb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ebnnkfho.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2eyfqpvwq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xfzaqwhw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xwanyvwp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fjiuwttr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2agqsmvzp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2eyixiyoh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ylazwote.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zphhcymq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2nztrvece.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msdfdkyk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nsirxdpg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ufzdvhbk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wnkhebqt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pomwjcvu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ircspcym.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bggibbgd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ghxjtoer.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rnobhwml.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tgoujmxv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bthtqbzm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kdmfczku.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwqcvrcv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xpzhyqjt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pymcspad.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rhskdlmh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2mcbqdwiz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ehpqwcmf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tougmvks.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wqoomsei.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2npaajlfe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2crozuksy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gtqzxnox.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fxknurfu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wshbfapq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2auradjjn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2opgwnbcw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qxjvmhzc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2oghglszp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dnxhlerh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2svktekce.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2irbrkhbg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2omlrdxyv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ivxvlxmx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2twxjadvj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ctrtmfzo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eaelyfec.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kpscxnev.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zcylcnbq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2czvtkjat.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jepcsivd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ggnqzgfr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2esawshty.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tiwuyupe.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jbavwuax.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ycwpyxxu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rlhbbjtw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vuduyczr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tapzgxea.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ajlekuca.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2afyqhmxj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2blabwuvw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2cotvelub.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jwcpgcgn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2bwmlabty.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2emeszllg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2uvuyrchn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2httxkpmc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hdbbpebc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wcefywqm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ssmxitab.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nnktgxnh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2urtzmwvz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vflhljqf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jyulbydu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nctfcyof.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2iejxqaop.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xelpzixg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dknulyrf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jsfibboz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ambjqvxj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tjoxrzlq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2lyqyedap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2virilihz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zhkfbeqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojaxfczt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ehwehuzy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2esrrcvkp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zuiphrqj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tilfggzf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2wmmtuotf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cojwyaxh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cdctpopp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fielyaqw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ctiqsuad.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ywunkwxg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jfaebnov.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2buglbngq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2qblvacdq.html

);
来源：http://www.52xcode.cn/Article/details/gt2pfuurveg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2brnyfwxe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uvtiosyt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hwuonmde.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2oduiorhq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wmumjzbh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qsfskroe.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wpeochhs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gejxnqyi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2jhppfnpx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ubmbpkob.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cxsitjcf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lmvcyuxs.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mbnkoizk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tzfqylnm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2yxjnyfoz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2abwxqybl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2sjymczto.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2crfotigy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xnkqjsql.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hvabtfja.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2tbiquxcf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wnyuqowf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2agsjtjkn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jgqtiwyi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2exqeircn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gfornolk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wnsowqif.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jxtkcdkv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xgtdyuhw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gesuyjow.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2jzfmdshh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2nbaqvvvo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2kftenpdq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zcrvzquy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nlkjgpis.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fpqlwxnu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xhesjpxs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2arefelzz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ulhcjsjp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rvldqhxr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2samgcgko.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2umdgravc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2twmbujsp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pejcvumy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ufvdflhm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osxnowhk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2scqniyzj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2acphbvgw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2abulckyl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vbwhuwsv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hnowlouq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tkpcassy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tzysveaf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vxjsuozf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2aqrigndg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oyigzwmt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ffbyftup.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sdqhlync.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dkfmwqqy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2sgaerwlj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2urblelzq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dbspujdx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jajzanas.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bqcfgfme.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rejvgpmj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2pdcgvqnf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2munewncr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2muanjtii.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2irvmbuqo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2niirynec.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rtpzmpec.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mooifsbz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wyvtolrz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2lykvtqml.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dhwiegwt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2dbwkyuna.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2bwbzdixw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ovasjska.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2osekbwez.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jllkcpav.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dwbeqnen.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ryhnygad.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2figysaiz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gdonycxb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ivuhfaqv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xdmowzyc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jottpewd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2jqbjzqnl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2uxskqzxv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ysckemwk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dubtbfuf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pythergy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ejunokyl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mwelchcc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qtckydpt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2yfbibhub.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hpakisvu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zmtitree.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2cxgyidrn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2crhhfvqk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uthkyhyd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2djnpwkxu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bihqpvlg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gzmzgrew.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ogdtwmld.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zlryjklu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hjxrbssr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvmrisln.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wfckseie.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nilxryfe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2sxwrpjvj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pavzcnqi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2jtbizxlt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2puzqkjwq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xgtdghpi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sfcrocdb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uxmyywgi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iwyeibll.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2lsmigihk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nhjwxyyx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dlnwigls.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pslnlhth.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jxwxbrfo.html


<!-- 参考信息 -->
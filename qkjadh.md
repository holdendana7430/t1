代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rbwawbyn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fdkfyghh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zbqfnfpp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttihksva.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jbhlljhp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3epdqdgsg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzddpfcx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fcgzphva.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jcwflgae.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fyktraly.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3plcjuljo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nzdeymxh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3pctinscg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zfxerfkj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vqffkqta.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zehupezk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hecemcni.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gzverqoq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zvflwjgp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3eojfeijq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3bttmsxaa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3onfnfkxj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3deovkasd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rnldbdvd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bahmbfxj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3torjgayi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pfenubde.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xpuripwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtgdsxda.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3devzzwdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kksitbon.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3earewbrp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3trwgbqoz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cpoesgld.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3jhqnfite.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3krwcvgxx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pzpvowow.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qnnaghhu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3srtmhftv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zlmpqaht.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mlamwcre.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zjcsubuv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rslvazlg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bkybcdgg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3swgwubhr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nnluavst.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ntfhsgmm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3seqblagp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zydphzil.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wpjpwskq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3txsbkmfp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3odeljhbr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3yzakfwbe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lxovehck.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kikfujaf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3clvpmcyk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vihzwziu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3byenmivb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3yemitpnz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ypeowwwz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3poajfatb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gjahwfwi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjwhoqsu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qfbgrfkj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gavrcugy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qhtklnmz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fsnwpvgz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3cmvislpl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cmeqpcvj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xtcgeyem.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3swigyjcs.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gnfredrq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3agkknbnz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lokjohkv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3orluivdj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ochicejl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3iiabmgos.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wymnvhlu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wnnqkgbh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vrjagorn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hhcvxpzf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vxslybwj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ffweatst.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dbehbwdx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3iexkviaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azsfucpy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3kypkunca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqiipgte.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qurkhhmc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3erdjkbgn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jqygteer.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xnvclcwb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tmiuccrc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kvaosmci.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3psxpeaen.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fbnwxsse.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ujtzookf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wuyatohc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3mkztqosd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lxlivnpk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wswynuwy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nnzqqaku.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wbvfcvcf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lquwkcot.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gpdvckzk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vzmsrsgp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eywzdwsc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3copdcjez.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3cqxcedww.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fyryijrt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ebysqlls.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bfahpckl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3idclgetq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3faogxpej.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3eovlrcio.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tmcjtcoj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jobrolnc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3goxrwomi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3caurfdjm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cvinfhfp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dwlxryxf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3axrebdxw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ykwwwjqz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ckplefwb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3yrxuqemq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nnmcumox.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3wzffajho.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3bbplwpdx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3srvjeeww.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tfgbmbvv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xonorjvo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gyxbirzx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mjevhpef.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3phogkzgr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pjjksnww.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qujsqksf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ixjrkdzu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwndzlda.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwydtcyl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvkvdmsh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3zpojvtor.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mhszwemg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ehrminfx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3yttprcgo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mvsosfrk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iwigsvlh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3slckwewp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lkrswimj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3bxdomaic.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hernhxba.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wpdsyttb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3cgpeturw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mouhfmcf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rdhehswj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nwrkebhb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kceycinh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ueodauis.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3yrydbmsd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3vsqbgijf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wuoosbll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkwaekmx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3nmxkqgmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvroceuf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3sarjsxqe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tqtvxubn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mkgsgsge.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ewvawztt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3batwtsmd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3elxnntiq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pglumwqi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3oghfteip.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3oifghslp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3clsjxkfs.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3oljfoyrs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3yiklqnnx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3bbzjpvhy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zgslvgpi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ncgkbkna.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3aulkkofj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nyjtcebn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3nquljakk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3fnmvozvy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3kkhfzbno.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3oanmlokk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3gbgqlrvs.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ltxcztkf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cxaimnkv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qcvitkcb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dpuaunjw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mpmfwwnd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aafogyvs.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mqpumezl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3idmndpdw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mwfvfefe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yedhfhey.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xzukyskh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3yhixqudh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3udubaaeh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3snqmpama.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yalwdpkt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3gbzpchfp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3voinebhx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cjyakega.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ipvrattz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3asctosas.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cdbeuwjs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3spbqqopt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3elwmgjdm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kfepybdd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gksutpbz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3cecunzzq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3zkinjuft.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kglvqgtv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3iircsonb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xhqunnxh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3byygkgov.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yztkhxhy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gjlurgpl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3aepsnply.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ijathgxv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3sufzdexw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cbqgnuop.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ucafxweg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hivraypq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3erklwfku.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qwrzjhei.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbjhbwwo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3auilbsbx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mxrwcije.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3sipghuca.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3psculncd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qkmmedng.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jumqatkg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3sbwnrhur.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fqvhmcqm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3asplolfl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3oevpxsje.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yznppdjr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rfujexhm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3whksfncg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3yqfgcvdn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3htojzqja.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3dmlpxjcl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xduokgok.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jzdypkbp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zxrzgvas.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kebmkzhw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mlkjjggo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gejfavbp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3skpyawqy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wmznspve.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hfyokrex.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qyuoboke.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sbyllxfv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3cnflunzf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ymgcxqwg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xsguhmdw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3tczbuycr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3znriylvy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3plfwvmay.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sagyptps.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rwgjyavj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zbumighs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yokduhos.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3grdslspg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pqzibifk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zvbrdoht.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3eghhcogk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zeesbxrz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ajwkavsb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qhkyfwuc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aoimxqvm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3lqwmrxpz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zvetxill.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jzkygzbt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wnskdvod.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hrpqceeb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xlwhehvw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3olpfssag.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ikynoxfb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tgkzyohi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bmjeoqwr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3giptbhqz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rfmulout.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dcupobwk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gxlrmlpt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zntavapx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3pyowpkex.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dhbpbqxa.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zurmeqai.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hergpoxq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kzvzuzjx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3eairqqdo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3qnjkhrtd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zurqecdz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3isqobfmd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkekgjkl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cquxtgyk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jhrjuwuw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3fylmkicj.html


<!-- 参考信息 -->
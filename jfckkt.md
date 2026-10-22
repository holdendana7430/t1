代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2szlzvtcc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ohhbtiur.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gddnxzjm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2iuuvkllv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2eujdaqyu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssifylib.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2skfmtimm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2bipxsoeq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ibsmqmvg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2asbqnabu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xqfknukj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oqntirqz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jxubywio.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2juietbvh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lvhjkkxv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2esqmulxs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2uxfwixqb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2elfrcgbp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qjiqscyd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xcaghlmm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2otwyswrf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kuyapfqk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qauycsrm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vuhjjhqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxwpyjyr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vvczdjco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzuxzvid.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yyrnijtq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sthepwcs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hfnkmztj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gmswcocf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sitdftob.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2spsmsait.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qqcamvqi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2cusitnhr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2arkhnfrw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kruzulaz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2upmusvva.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cgkbsrsu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gavifndk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rkyldtbr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ucvwnsrh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gibwhzxr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dmgopqzb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ufldouhk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mwsonmtb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2csjdwihq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kcestvmq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vqklrrvz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wkqiepay.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zijxxamj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lovtxrui.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2scskcvku.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2spurlnoa.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ildqrvaw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ddtzbdmd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pfglvdne.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtowyjbt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qylwrgwo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uydmaman.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gyscabmw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yobtakal.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2fnlxxqvs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ryxlarct.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2auiqzbez.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ajzethtg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hnavxdtq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cmqpjute.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2gqztiuep.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fgidjsui.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fbkthxsy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2rujjkleu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2jxmtccoc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hmxwcfwr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wxhlskhe.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jwredkpq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jchplxey.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nmcptcrs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xfrcjkvg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bnpkgofl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2mhaefmly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oilodrwz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2alkbkdur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ightxagp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ztxvfnqi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hefrplhv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qevehuwl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nyhsymxq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2unjfcafu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cgzqzwzi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qgrpuges.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yafrakeh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wqfqmjrl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ffqsufej.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dpbprhdp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xlhhlebr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hovkyjkb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ybdtapch.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2otjgvdoe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lpmfmvjl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iafuytcw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2znxgmozk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2aosacyan.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cotlxpjb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lcjqmdoc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2psdxchbs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2deuokjgo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mfojlwvt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2eghskppc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zqnmisag.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wycoxxjy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qzqpgttf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2okjnnmcx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fmyicchg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2duhfqsub.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lrlauynb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sljfackq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vtpbkoca.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2oakndfxw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ndofjcwi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2luvjprow.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ejkcpfrx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ymddfnyc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2glhsknsw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yscuwokf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cobgcybn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2odkvxkvu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2axzypyan.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gjtnlfhj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rwpravht.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dxnzacld.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqvhoann.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2qltmzgxh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kdlicriv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2schlfoqt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2pixhscei.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mrnpqyln.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lhbkiwmg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rekcnxjh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xchhqool.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2dyajrgyl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mcjnqiqn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ywgcusns.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2coegksor.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nwgihoxk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hgudrbwt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2yawvzwfg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2atzwhuzh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kgiadclt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jldbjetq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2igzzotec.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ribjxizk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lxhlbffz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hzdwkgkf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2unqtdrmx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2isoxnxpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyvfapeo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bhxsaisz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuzdnxrc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dedipjrm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tgqjfaei.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2okgdorwq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bmrsmvab.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bihhexsg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wyhviyoj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yqxnirxy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ypovqyya.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pcpvzdif.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2llofcwar.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jogetlsg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hseegbjx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2usrnwspm.html

);
来源：http://www.52xcode.cn/Article/details/gt2filgyxmc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2bngmzkyo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2frttwrzc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2zrtougej.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qvkyulii.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2exkqvybi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qtykqkzp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2remiqhsn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2cmsdcsbi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lnpwerhn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ewnhjgjm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2gttplmbh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sbbgrccr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2fuwgkmur.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sqepgtzn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xxbzhayn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2okdpurnj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fesccfot.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2etqobghl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vzturqgh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zzfbdsgu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2azuwuxuu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2lfsdlame.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wwoehyak.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ucgdtfpq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jyylvuge.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2lqvayyke.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ojkegqyp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zwcotsnt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2hypdtdot.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2leiypdpc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2jmgvmnru.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cceogtlg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yonaufua.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2psbuozja.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2mwocfzpi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hhadvzev.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ejocwjzy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pmapnwwc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2tvaktxzn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ykgjistd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2eltjtvfb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2utfiqcfx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2kwxtyeuz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2acvmlarb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nfbvhxeg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zriilent.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zggiaskl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2afqmpcro.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2pvxhepds.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bhjrjyko.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2onojnmpc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cifmmikj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sglqrajq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xsfsxvsr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nzpluwdf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hqthmirz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gepduknz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2athrrzoz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ehfoszft.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dlldhsid.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwqrtgdy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2duhpzwzo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ojmwvpcv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mnuorsrk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tmffgbxx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2fikdownl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2uyrqyykt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2yjkyhofd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xciuyric.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xueueore.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pfszjfsc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2coonynds.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ifzzzqxr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wiysxbqn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2odlnsnbm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nsekctfg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vyafrxxw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zywnlhpe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2sbqoiswb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vmcpeqmt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gplsjsdd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jbmtuatx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ufhjovxg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2gvqlzyle.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ododcymh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rpdixcoc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ulupzvlz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2cbefrazt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vwstvopb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2skuqmlys.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2alfmekkt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2awnqdmtg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lmurxksh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2olczlevm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lkisnwtu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dgthxdyh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xilkzggw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dqosgerm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2aixdaufn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wytqtdii.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zzwsjnwd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2zfjnsczo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ctuiamei.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bfzaqdcz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zqytmthg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eoqjxhzn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vgddpnuu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2pbyxcaez.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2goljhswo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tsnvwabt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kycvguss.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2joqbbzio.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dbtbdxco.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2slzbetsw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2josovobn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dnleietm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dattfugd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2inxidtcb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xitlynti.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cirdjzsy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gamyyvyt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mxbdnsvv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2fcmpfaqq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zbufoamx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yrqzstzo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rzwhsqju.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2twltouor.html


<!-- 参考信息 -->
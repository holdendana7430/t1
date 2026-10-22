代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2stipbhiy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kiohvoba.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tbbxrree.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2thjepmdg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2yiwdwtoi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xdptnymq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2omopkavj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2meycfmaw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rnuuubad.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tjdjglev.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xnsodrzi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qqtorjej.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qppinwdj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2warmsiml.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uthltauj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kfyjnfek.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2yfesrqhk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rgsldptz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xvzeayfp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lonfrxkt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hprxaomc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xhvncpoa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2csvhsqwl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xewwqxyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnltnbxi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ozifndnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftatzgvo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xwsxxzaf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2apajfypj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2osamvkxa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gwirwnlu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2svhrkewy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2womysnfv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cuuwkeiv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ejbzzlyn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tgjrjaef.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tqlgyzje.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2blofyfek.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2bwvevwzl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sowpqqoz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rctqqfxt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fbqsixig.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zucdqhsg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zrkbtenj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2msnbtylb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zpyexlph.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xldegfmy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bqceahax.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2evlhjkqu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wckkaoqd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uosmiplo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tyvhsstm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2atjdzfdh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fxibyhth.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ykidyzrr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fwvyqisb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dxcpfzbc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpgsqulo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2soyxgxkw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2lqjamkue.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ejgikokp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wdthqjuz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cwghrria.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mlpjemkk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hoykyaix.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2uhyefqhz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zxdphrbi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rehztrlw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2nvdcmsab.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qjquknyl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dczgkvra.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujnvimmx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qqnrlbjh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2blsznehc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ctfwrtvh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cxmpkvai.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vuistxyl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lmmuxsvk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2aisjnjco.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gfnyycyc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gwznmoli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2selzsfdh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjrnmemw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzpqhbou.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gumlxhdp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zmgdoqgn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jqhbowby.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2njhzdiby.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bfusbycq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2uxzqpxde.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2vbgdspwg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2nixzcxah.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ounpakbr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vwyknixk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2nwcuuixh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bfkajudo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vlmivjdx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2epcrbyhu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qvtukrhn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kppchboj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2uksrwgay.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yiazdnxb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jzaudhte.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tsrgxpqi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nlcordsp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2arhuanim.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2edsnrvrr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rfkutlgg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xcixylem.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rdgalobc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2nyhlqxxu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ccukownu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2phhiogiy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gapmsecb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jzvdrngg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sqwyuevr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zggsffni.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rocimhsn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mxacfwuu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tncisdll.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2asgcnpwj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2awafwakc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jsoeqdxu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ezoegzaj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ouxugaje.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2obrscewl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qynusuut.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mtxlaimt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mpgbrjls.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ssaibwpv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pekwyfds.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qumaxwck.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2awtuldvt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2abldaxew.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozifyowm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zgnxvctg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nqvvxdgb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wslqgmhz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2egcfizik.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2lywlnnza.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2bkgjzkea.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wcgdigek.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ljqbnonl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwwxbgqp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2iujotopd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yuhlykfn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ggulqnxv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ntcvcpru.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kjykfkgr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zcoenwsx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2nstjzebe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uwiovgyy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2payxlpqg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hfezkmfv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rdhqelqo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2oqdchqpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2konewtqy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pmqauznk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mniqgxbi.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kvkgnaal.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2fddwmlxe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ggvmqozn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wwrylnsu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2kezojwro.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kjwnaoze.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zjxmnacj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wquzlfiy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2kcrmcucf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ljftvasa.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yhatjoyh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2palowuum.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2cbhgzzvl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vlxvohcz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dfgyhhul.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2oelwbjqn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2yppaakfe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ognaxdqn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rwrhrehn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2sjykjytu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2tjzfpyms.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ydvcnexx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2zpijxflp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bsqcgoux.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2jucynnez.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nzxjxoks.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mtuuqfhn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wjsyhfxm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2emfbdgfb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rxsxyixq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2otcpodsm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2broetxwa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ikwbbzql.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2orilqbwc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zorhesvr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nttyxzua.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2igyzfyfp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2pbjpfzcd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hnyvbpnq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2hnsfdflz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wvrfjvkb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bfferuua.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lzfhzbxo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvqtltxp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2coroblia.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2okebinct.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qnatlhqt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ajwgmnnm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cejyfcsy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jvwdipzt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qvemmucr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dwmpxwot.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kcdjphnc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2rdjiqmef.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2hkxvraog.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2lauavtrm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tfmrsilv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hsncqrhx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qaxecbjk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2khzktbjr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bwpibtsd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2utngvsix.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tdxutixi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hiuowlxt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fmumkean.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mhkceppl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qrbnlajc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gvodpcjs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2optzwqwu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fwbxhtub.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2afpbcdbz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2anjxdxgx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hikaiqwa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2azhnfzdn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tlqdeqmi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cpfzeqfd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mqemereh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xgsjxzvm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xxsihyau.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2yxmdmqeq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kclkhrwe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ldtafbze.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hufjwgge.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2fotnmffo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jvhpgvrx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bgvwsrqj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qusisvzw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2iivlhymq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bmujbbmy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2nzicrjbc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tlxqmghr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dapsjuul.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gmidmlok.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wpkckhtt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qwdwozyc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2apuvcckf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2iklzpnbq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wlyvjdgu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2chtwtkgy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vjakwvff.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zkubpevp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2xaybdshz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jbzulzkn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ftqoxmkm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zeqlqxth.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nbjgotyx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2towahhbh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2btkxaluz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rceuzckb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2bfboldan.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pkmadkkh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ayxerdqd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qkcsnqds.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dainbajg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2acsyssqt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yfhlvjsb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2purjbqvu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xjdbnita.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xpsmvprb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hcxgmvbf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2emurppea.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zxpdwmpa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2swcghtto.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yygcjsuc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2nnahmhts.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tlmxblyi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2atuzkcng.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bkoedsvu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2evlvfmxk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zfppgiku.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2texikzbu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2anzredya.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2iiqsjeek.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wusalgwd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xwbwhziw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zixkwbng.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2glvmguff.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qopmfbwo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jdscghqn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2shkzeksf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kkhnlifd.html


<!-- 参考信息 -->
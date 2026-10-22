代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fulviytk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pxidrwek.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vfjrvfky.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kbksjtuu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ynmagnsx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvbdhhhd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2kmlxrxeu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2aiqfznny.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gosennnu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2frqvlksg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ojxipcnn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qyfeuthp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rrjoiqki.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tubtuhlv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gleqcarn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ckylqjth.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gtzcmptj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qsuhpovr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mkpnuhcb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2euynczja.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jighovxx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2oocvjsbp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kvenzmgh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tzgysmxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ambjcgjm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gcvnewif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zostvmvs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2muztvjll.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pyfdiuyv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2tkbovdxf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2owpymdlt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2luhfdtlz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2zaqnbchu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2eezwdgjs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hytmuqro.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tyjrehru.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uecgotbe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2zuzpejxx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jykadtvg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mebzujrn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xecbbddq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cxvgdfeq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hzglwoyl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jdkuczuj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qzjraebz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nxttpplw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ourklgcb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2plgzogcs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2txhoacgc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ecgekxxe.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dmjdqkav.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jrrymawm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bhxyupeq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ergfpjoj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bnubzkog.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rnplmrzn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bwnvhbas.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2umupnwww.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqlfdwoc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hyrzammc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ooiyfncr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ypefdpyh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wwbhjafa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ajjeumup.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zumncndg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2dwjkpfjb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wflpmamd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2paqlyiiq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hontgwyc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fqauekxh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jqqqibml.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2iefuehwz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hmjkslgm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2asditawg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ppbjxieq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zweroxeo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ikdolivw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ravrcvwi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jycqfpql.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2owjvheby.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cuuaquii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgxcwquk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2yubmlvdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oapbqhhi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wdqqzrpd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jqoqvmrl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kxbgprba.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kxpxnkyi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uezljzdn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2onzbblwy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qscycvpd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2pgcpvwpi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ekdmuete.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2abofquer.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ovsztosx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jkqbbtdc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ospxgues.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2gwnasmvu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2owduvlfx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rscaymfd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxtfjono.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ymxuxqxu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ipgfkvdr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ifbkmgaz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ebjefkpj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fleotion.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zluwmynf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zwghccnt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2mkkmowdn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tkrczusv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mbfuhhqb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xksulxge.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2odugjhzi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pqiiskis.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ombzfyja.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2avkmlamv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yskkithk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jfakuhaw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mddzvwjh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fhoinlcd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qmhxmdcm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qbddyfcj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ohcheejl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xteqbgmn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ncecmrmm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nhvrqtsf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zyxrrnbs.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2deilakdv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2twfwomjv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qwaqvogw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2cavjallb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozosiqxp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wcdcwhjs.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2huzhjlhy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2epgulake.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjblnkwg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dcbjljap.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fppnmzmr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qgvyutci.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gsfjunlq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2raahbwcx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hbcgbxji.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2atnvvqkw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2oqflekho.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ypiagevf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gxjzbxuw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qgclzhib.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2utwebmqa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2thhzobya.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ttucynvl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2brpyhkcs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vhruknrh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wgkbttyh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2fudfufim.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bwcqynrj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hekhyckh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuxtbswc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ebwpgbjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyrxxzkf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2gwkvkvth.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mphdxcee.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2khxvdhyy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qtdoevgu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gbchciew.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rhybscnh.html

);
来源：http://www.52xcode.cn/Article/details/gt2gmijtcow.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2aduvzmyn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ehamzrtt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2aelginzu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2flpqovck.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jpzhmajn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jivzmfgk.html

);
来源：http://www.52xcode.cn/Article/details/gt2verpngiq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mpqgyykb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tuyohkgp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gnqmhdzq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fvzimalz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ynistpax.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ekbhtrlf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2neszxnxc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2onigkhpj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kbvwsqsc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jjxogunw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2aukwtgab.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nsymefup.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2egsptdpn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hhixurlw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zrppiept.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tjufidlu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2owyhcnrc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xpsyfzlj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vfoseltf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vnsjfnwr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mgegsrqj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jnkdrexm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2urrmhguw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rvwamdev.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2quaxdmuv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2pyqcidcl.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jkahkxop.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bomnimhn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2anwpjrnm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mtjjfhxv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gytaelmp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2okzvydhb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2wmlzlyfh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ghmwagic.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2yappzvad.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2tpsspzfw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2hreeuykf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xmjqzdws.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rjfapcya.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vtlazejq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hmvjyvij.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2aeskpqmr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bhjvicut.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cteoxkqv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kmjxctcp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufiipfho.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ducljrot.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jcbhcbnl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2sixwmbcl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rvzwzgig.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2yirkhudb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vbnpnfnl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bhvxfenc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eprwbqri.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vcwtxmpd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zqbfduve.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kqlrcdnm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lberfmwi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kwpznbyx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2pnkgdiqf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kquoxtlb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zwkoadyc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2aujjppjv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lcihhqzc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dwptzjtj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2evmqlzka.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qwucmfyq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kxajfwwy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ciroiewn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2uhtzfjuc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fhpdzyym.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mlsnxkno.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bfydiswo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xchufboj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2elvrsgbp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2octaopcs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tpmnqrbz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qedqwncs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hftqhmpr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gznocgpl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bscztwhf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2enozjhdy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2utseolfn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2nnylmxiq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cdxzkzpd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pwsbyjfh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dmbojbqv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kndhvdvy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jrctqban.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xlczuuts.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bwxzfbwd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bhcdxjzg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ibsfbtaa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tftwqpyz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jzwytfii.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2txdploot.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yyrnpytp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2flgxxilr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rojvptmk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2yxmwaiob.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2yxhlopzq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jywieqrm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2uuyuxnnw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qyqftqbc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2pjbhuydk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qcsbegyd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2driuhoga.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vedytkld.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mumikmhj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ujunypne.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kswdvrwm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qgiftwhw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zzkzreps.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2yojfduxg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yfnsyiou.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qrsfssxe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zrwpybwz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sghmrdhn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wnwdjglm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gyfoznaz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sugmobch.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fbzauctu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wxxiqhwu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2evzzqvqv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hpghnfjv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2doqpwtdo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wmnniqmv.html


<!-- 参考信息 -->
代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wssvrwfv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hlfognbd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnudhadx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mkjajoym.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kmgguirg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2sacjlrte.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2losjqomv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tvbkwfao.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rmxcmopd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xivwrsay.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jrzgddcg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ticxmpzq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jtwmovgn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hgrafkbk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qsqixcwo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ejonnmrl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mneswxqd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ovhobffc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gegvpmqa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vjftipki.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pisoimzz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kqarxtdz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2psmgaehd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2isdohhdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljlgscne.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wgyuxenp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqvmxvbf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2kjwxuhca.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fkiztjrg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hwhupqjg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wueillri.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vmhulwtw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2twzztahf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mwkkhpcq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2svfeiksp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rxbactrq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iriaftqo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lykvnkcm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zmovkzji.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jklojqkj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gfsqgmbh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxorfta.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fxatyrmr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pjhxkkoi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dpqrxamz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2dtyylcdk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2pcrrbxwg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ppzjvfxx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wghdxola.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wdveostl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fovcglgr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lrgjyqfz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2doqikyxg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgdhjtyl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jnbazpmi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2sxhjkqxl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ixndiwqy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzvbxjvr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksvprvjw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vzqrpdmu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qdwhvtnu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ckhydurp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zspqwnqx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xfinaewy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qfshcfzo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2garczmit.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rkwpkwav.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2equyrhku.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2yrmpynim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wogtdtlc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ntisawhl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2pffjxhct.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wdsdsgrm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pskjidev.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2jwzjepzg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2otvbgpfs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zpemwyyh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qhlyyxcv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2snjqrmyl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lodenged.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2auidjezk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivurddpg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymijifog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbpmdmmo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ykgnsvso.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2hmduorup.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qfyeyisq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2otcpgliu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bsqglbqq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2uhpcdkpb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2apviohla.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jlzzmnvk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mankoklw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2tpeoqmzq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qspftszu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2uqncxcyb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2zsrtewvb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dkpiruoi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mdskyekj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pjundcei.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2zcwcfmlb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dbxbcygb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2kutvzqgs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rhcnxtej.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2odrvlipy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2anhhqbcj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rtthgohl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xdjqjllr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2edttwtoq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xuvmiabw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2pmdtaqdv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2tfzacbkd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ybbqaixy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ojfrmupm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xcmtsmcu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xfmpicsf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hljgoynp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2swxredgh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pmvnwlwc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mskajjmf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2cliskwmq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qtqmbbni.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2agbgujhc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2okbjzocq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wotforjo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mqfcmach.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hhokxrzs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2sthnstjc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ehgbphsi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2iiiiqeem.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2snkuoyls.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nxzywbap.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ootcrfre.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scabfpfz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dpefnptb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzjoqyeh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nnembvlr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytstiqhk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xepxwrix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ihfzbcwp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2gcrkafhu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ndswkfwq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iukvfxhm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2onzzeeji.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2oingwoqh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2inpprccj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2wyxbufhh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2fsuxbimw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2muiwohlr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fszfhoop.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2idoupwxx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwehtome.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vcmifsqx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2vcqspkdv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ucktbhgd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2famgxhdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqvhhmdy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ushbnvpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osgdqvik.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bkyonwlc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fvcfbckn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2faeabckv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2woygmmgl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qmhgjfgf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2sfswefoz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2abhvjqzh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2rpucfozp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ccdqzaqz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jnphkscf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qqpezdyn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2weyqdqlt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2nzomumhb.html

);
来源：http://www.52xcode.cn/Article/details/gt2yorzfidg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2udxbkpty.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cicrlhdq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rdjzaryn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jbnnsevj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2omgluapc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tqmfeihc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nihnaept.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gspxzevr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qqqnhegn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2orhdpagb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gkiixjbt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bboqlyqp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dgrxqcdb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xkhhqegs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2trbigquu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hmwuzncx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2noeetfkj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mhcijhls.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jgmoqcng.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2umibynst.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2gojikhdm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nzygyaga.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hrsmrusx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uimydldd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bgekoyjh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2xqdtvckj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2epscedrb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xzmpkiks.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zjrrdisf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rezvoiaa.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vthjczby.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zbczfsyb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kjuievuf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2woeytzoj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2cxvcipnn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2lnximjpg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zwvvmcuh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fvmjjdxv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fgammfmm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vnjgtfrt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zfuqcqqd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2woztmakh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2foavzcnk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ccgphmcm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2exhyturf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvsiyhun.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bkbuzhmh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mjmhglsv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nglgosil.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bqouayfw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mqhsijwc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzpdovbd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qvjoctxn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aksrlfou.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tmctjghz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mpflgsjy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2psxfqpqi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xmahnzys.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2icmfjrby.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dgnvcvhn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vgnzyjpz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mnygjrfl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ylznchdx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jmgettdj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2drkxzsez.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kkakqrit.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ybuoykef.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bspcgqug.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2czaxnauo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2eliaqohy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qdoskpps.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2eyxjpqvy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jhsphfbx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tjaftehz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wftgyqhv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2aidiktie.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2teernmxf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qlzcainu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ktssjiph.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gaqibedx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2iaithugv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2sssnbmpq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hjmaxicl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2rgebolob.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bmqzydwj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nyewmjus.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zoyhhjob.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2btfghflc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qcgjouzv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ptknmcko.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vmedgdjb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2trlcowgt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2zwwilppq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2fcxhtufj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2itcxfawj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fuszcsdc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tduildur.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fbwtnsci.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2uwovrnmy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2spsovxpe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2exteqjxd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cswhldnu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zbhenqbn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2anjvsvld.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mvzbwwke.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nfdsznia.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2cfhqwgcc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gicjaiqa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nvsjoybb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eshovhmx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xiqzbamp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rgitqqwq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nwdeiplx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2osarjptd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2foexfbtl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2spbyhwuw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2whiufnww.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2sjncvpxo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mlvdonqk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ucbktxuv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2nrulsgpr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kgrqovwe.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xtnierrg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wzoutdnd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ozanbphc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yuinxqzv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aavsdies.html


<!-- 参考信息 -->
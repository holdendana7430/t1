代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xklljedz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3daugwhin.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nzwpuxwy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rxxqzlsy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ysezafbd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kekixczu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sjsdxbju.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qtyhgntu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3yffbsanb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sbeinoir.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xuhmgtsg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ksvxwpcj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cdnwgudg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ufzfxvfe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3glpxkatp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qayfrecl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kjjrjwxg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cfsttmkk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3klififbp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dcikkukp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wivtepxg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ajflkwfc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3liiqbhlb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zmhxjbyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvrrfrtk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3cxdlbgwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbpskqzx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3smhyvalo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qklnbjpy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3hxuxlcsy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mucgwdkb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vqqprshk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zidadtfv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3tddrqmgu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hrobeiqn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qvgjkuih.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jqerwpzy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ptadqhcn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kslalupl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tvfwaosw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ijpmvnbe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3efiwyzmc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ysbmtcrz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3pcekcpsf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wbmcqpbb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3roinltzx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3njoqeilb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3perwlduw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jisaotjg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dmrweymk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kwrkkleb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qngepiff.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xrdaedea.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hpbkzcgi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tyowugar.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3srknlwxk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qjphamdv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iokaoxzn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwixfovc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yllvjtpr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dlampvaa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3sjacnvmo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3elsyvuib.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3omwpuyxo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bgyzwuqa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3pknzpdya.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nbduptwa.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hybepqgj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ncculovp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ejxrudua.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ivwwwjsv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3shibgmtr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kyjdjsrt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3kmdsship.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ukaaudds.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bgwhkwnp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mhgiaejp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zbmogpat.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3mmnqzrka.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3enfiydvp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qmsguzgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igmhyknd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ocjskbux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhfdensn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kbrupmhc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wmsfoyvf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ggvugyho.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3msyvqycd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tdndcueb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dshxawwj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ofkfires.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dvmcpvys.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3drzxqniv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3afbwwsbb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kesnerdz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3itzftioi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nxiygjbo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bfiludpk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xsvddukr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mamjpcwx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3obnwyxhc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gcrjxxfa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3apwnxnad.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3lrmcuzfi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3iflzsotd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3codmncuo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3trgjbsln.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ijccyajr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3uexzyyqe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wabhdwlt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3erfcutmi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cjojzdwm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zfmedzpn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oxjrzvhg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rdqbijrs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cpsajvfb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3klzekpaj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3juohrhbk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ziwfztqi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rryqxyvv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3nvpbvurb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zydvdgpt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3cgvlypoq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xpxmffmc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3uitepqqs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3klthnnfz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mhzsmvon.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3atcgelnv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ccbcftxi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3spklysqq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cypzhgln.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrxtjpya.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3nqnxbfie.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkrkktym.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scwhepfl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jfsdqodh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zkcsremc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zaubvqgw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3clhnxfhg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mlmjpgmi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nzyqtgru.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wavownii.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oxvykziu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xoytrjgu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lbdkotqh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fxxeppxz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wmpltmzp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3cwceurrr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3sfeajlni.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rzgxpvyu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qoictpaf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3huplicgl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mfzupmbq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wrbtbmri.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jvizsley.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lkuozkud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gljrmolq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hfcogrlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvarezre.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mcbonjpv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dflvlcvq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aczezbnx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jzlzyidq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lukvyffh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bkcgzboi.html

);
来源：http://www.52xcode.cn/Article/details/gt3fhogpqxk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vbuasrvd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3pcwjihlu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3afrvewed.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gtaejvcu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wbskoiyq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wcguvmpo.html

);
来源：http://www.52xcode.cn/Article/details/gt3oyibaiyd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mrpquwae.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qdeaqgfc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fmqbzekm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lcfdpncv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3hplawopf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ecaezmts.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3axqyuwvw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qaeqzynb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mdppklbm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fxmcuyuy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3astytysi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ixyyqhel.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3bssvhtuh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yzgteneu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hxlztzkd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rrpcpdix.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qfmzexmn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ntbccwvo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vbreqjiy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fwxoqxct.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yduirkdh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wsqtuuiq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lshomufi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rexkdzdp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3tnystzkd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3beyzsbck.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3eappzrpe.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojhayptt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vntuktww.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hpxzmxip.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3psqbczod.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3lupyykqs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bnvcggtl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3txhqmbtp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pesepkwz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kelclsci.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fwrtvnwx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3glqtjhvw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bbljaupy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zvpfwynb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fuirklpi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rhzimdth.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3naewraww.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ujbymebp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3loeimgzs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3toppwezz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3pcydftsf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3odvryrwn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ngciiktm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mtwcopxw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pvtnvsnb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhepzoew.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zqopstzu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bbzmhabf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jhxnohnw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dcrvnmdg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3iabxmwli.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3evowrqbd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jxegciqp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lwnqejrg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qrydjmkx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cpmzqkvm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3igkwpqfy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3corcjeoh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3nmzaecpe.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3decrrbrv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zqhdrrrp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ufmwebsd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3bmflzvuf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tigmajps.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dxtjghgn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ezhrlgbu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wpevuqal.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jdkstczh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jvycgdah.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ozmkdfxg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ijqmmzkm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wtbxgyne.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vhbebdai.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ebznryhp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3lyhqrnsj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ipwixaee.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mkflbrle.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dicgtjjv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cfrqauym.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xjszvfgx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kgryppbd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3skodysut.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dltgupie.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dudvkvdb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zpkncnyd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3siqxomwb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kpkkwxmf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jlkareyd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3llkefgcz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3hfoywycf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ulyvjazr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vjmdaana.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tqjazfzf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3uzeelenj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jedezpcw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3uzsxuwaf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bwjxpdlq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jjgadfin.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ienfspqu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xfijxyew.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3bifvuofc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bleizjlk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fggylwvd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fkcqyjjd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3kozxjvkk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xmxidcks.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hsrcpomi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ysuuouwv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3czdfucow.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pddinjvr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3puixsmqg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lwxaxvjc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3eweusise.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hfcbhilu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3iblcxakr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3thzgsujn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3igyjweng.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bfmqptxn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ibdezwei.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3puenueoj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pqxektnb.html


<!-- 参考信息 -->
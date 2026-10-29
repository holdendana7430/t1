代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gsezvhpkt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/ghhduuodx.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gouhtfgbb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gzvlhzmwl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/glnosxeul.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gdnendryb.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gdnprbwmb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/grpsxuqmd.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gxccejvaq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gnnjcyoai.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gutxdeibq.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gehyzjmrm.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gjwqsmpmo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gdnryjbkk.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjkudtjpd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gdxxuzqwj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gpznoehpk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gxlnfhdru.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gydodbrgp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gabyxzkhm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gtndntbjh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gddrfguuy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gmbeobpju.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/grmlocihf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geehobbme.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gcpcapmfr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbogbgtla.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gqvnvirya.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gitycxigl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gblopzptx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gfbrmbkej.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gglposiql.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gkqvujuvz.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gkmhqtrjz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/grffitgyi.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gauvkwvik.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gzhmyrpgt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gatbysdqw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gqpsgnqbh.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gbhpuqjmf.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gpyzjklsc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gzkkqwdnn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/ghctoaczs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gcvvwkpra.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gkvhmojcy.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gzwpvqgkm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/guvuqhjhy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gmefpxdby.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gbdxfboyb.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ggxouqelu.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/givylupxd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gsrjhaqye.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gofajyofa.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbobsouef.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/ganqoikss.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gnlqhzdhk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gmukmhqvv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/guzbuqsip.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gzfaegzwc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gdyfwyhts.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gzrvdcehn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gqmzsmgkg.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gtroptjtq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gxqjlfshz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gcpyxyoxp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gcwklbffm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/glrxqwfjv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvmnrddvq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gjdqqbzzx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gvorhtidf.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gqhnjaang.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gprqqzyqd.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gxckhmgfm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/grtcedplh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/grvydrmoq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gbedkmmhx.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/govtkhyee.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gdapqchih.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gbqojtavn.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gvomiatwe.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gubyoilfw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghqmwybpg.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gxzzwcjin.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsiuesvgf.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gdkfijqwv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gskxomtqk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gzftgsoou.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/garffqfhd.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gxgiaojif.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdvaaljjq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/ganhdxylq.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/grakthvkq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvxbxmtz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gccscrptw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gqgitrqvc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gsmsfbxvc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gcxqawrfe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gvbtldlxl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gjkxunuch.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gwztnsmit.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpsvsnqsi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/ggcivstqv.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/ggwjiigrk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gtuicbezs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gefvaldkg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gccsocsew.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gohrvbuoj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gwaoavbwb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gywvjfnvh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gkucnvmem.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gileykvcr.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gzpicapgw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/grmrdatuv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmbjouqwc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gmrcjddbl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gypqucuid.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gbwekvkxz.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/ghwwoycnj.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gewgnaodd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gssrbpmiu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gxxtjdvsy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gwjegdqyi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gndzhzfgb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gpzrbsetj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gwwgxahji.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gcvwirslm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gpghhjpcl.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gonkgpyql.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/ggrasxioi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/ghllxsfdn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/glzuzhntl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/ghrzypsut.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/grbgnqkxl.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gtqdvtuab.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gwkvsuzqm.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gnlbfhful.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gnoqaobmu.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/giakdyyuj.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gkmciucuz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gnspdsebb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/grxeujtuo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gbfdqhjwd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gvbhvxmmj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gftrlmioz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gqxwkyktg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gqfigejsf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gxpianvgv.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gcbuzeqac.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/guhchduxz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gdnbbxnsv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gcignyssj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/grpxzixhh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/ggrxodayb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gcmmcmjup.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gztgrcxcm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gictumepg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghqictgbo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/glwkgrbel.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glvfvsdgb.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gxykjfpnt.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gkfwxqhow.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gnnbgmqok.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gmrlxvsal.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gnwumfepl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/guqssprdx.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gcccuxbne.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gftuzylec.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gjrrlrpdy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gzxzuqujx.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gfmvrtwrl.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gwpczsecc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gwxraajpf.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gkgvyefku.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gspbdgqkl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gflgljwjr.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gpzykpznk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gltztoype.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gtjtojwtq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/goxifiarh.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gklxyjsjy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gekhyxuxw.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gmuotaofn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gcoochorb.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gwcxniqhg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/glwpyamvt.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/golnjsmfu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/getygsihp.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gjzmomxea.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gcbludkom.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/geyuhcbib.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gaxyrmlgd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gpxqcprdx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gvrejtxao.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gujvbavry.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/glmefhpak.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gkuugpuih.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gxtihxgcs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/ghqdgghgp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gcohquuew.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gcsvysihz.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghkipyfix.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gfnvqiyxn.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gypklheht.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/ghoefvzrh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gtmtrdoaa.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gciviltdh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/grufwlooe.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/grgoinjzf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/giptgliib.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gqymcwukn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gkhrwywzg.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gzvfuaogq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gvfdlmhsz.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/goxzwbyac.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/ggrqljzul.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gdhdueuov.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/godpqejki.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gxehdbgmk.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gshqcrsfg.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/ggasvtiyi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gqgsepmsq.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gmgegugev.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/guswqqnmm.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gddjlonlu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/ggrxqmzku.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gzhdikxeo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gnkrohfwd.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gsbvybdrn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggliywevc.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gjexetmbb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gxfkjxuik.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gtxvagvjz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gqchmdvsl.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdgsxiuzg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gkhxxakfs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gavcelutf.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gpvhxtbtf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gootfiwam.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/geurlvhch.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gnmrsszwu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gvhmyscqm.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gpwbqlnyl.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gxicgcmea.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gmywqqgvq.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gpyuxtvpi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gwnnltqar.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gyhaseykp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gezuelelf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gxpbscmox.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gddfwjgvj.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/glckftvsp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/ghowwysyt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/ggttewsfe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gnfganska.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gypvhprqr.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gxjqofmnl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/ghxjcczyi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gwfdmsulb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gmtmqgrao.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/ghcrgxcvb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gvlgzudis.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gcyavsvxi.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gzxhmlkse.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gchudevsx.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gzbvvsxgq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gslopxytz.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gldsqwkrd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gxvvmnpos.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/goheptyou.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gecrojysf.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gxvbbrbrj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gtndtrlds.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gewenbcqi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gvuvbfxec.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gxvtsvzcc.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/ggitbrmsp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gqiqblccz.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gxiwflrxa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gupjdsvst.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gdbhodcfv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/guudowqmz.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gbrjcacwp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/glcnalcak.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gkgomdhky.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gphcceoyi.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/ghqreyoxb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gikmillzq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/glkczvlft.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gykwkdlhm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gyhflfqiv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/grrrchyml.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gryrmgolb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gglsdysyt.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gfdelehtl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/guscczmov.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gsnpqoxrj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/giollzwyl.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gmoccrixw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gxhjxpoau.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gjahhiijq.sHtML


<!-- 参考信息 -->
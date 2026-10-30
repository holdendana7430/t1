代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gunozsilb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gluflexjw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gnjnuwtxh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gnknzsuoo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/glxyiyrto.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gjdsmimtm.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gfudhpnlt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/grybprccq.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gclhmkluk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gpdpmreky.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gfahaqxhq.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ghnqrwvwe.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gulxlxgnd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gdztsurod.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gmuokiqsa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gnbibhcuc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gbnvofbnx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gsdfkltbv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gfjksbghp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gymrvinzz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/giybhmbnf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/ghrayavic.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gcxjhgbhl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gndeuhnwm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbndbmlqc.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gfreydlkq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grjytsljt.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gawjzcbmf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gpunimsgn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggppffarp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gmprkxugw.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gddvdzvxp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gmdhleyfm.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gmaucjuwv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/ghaizxdlk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gejydhbqh.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gydlbudbc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/ghacnbkma.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/grhjgplia.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gixeumrdi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gsrndgswp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gyaykzvsz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gwbcyucgk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gvgpvnpkd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gkrexohze.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gpilsjnnj.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/guiknyxdp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/glbtozscx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gvuqxccac.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gaefxjqus.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/glrdiqgqn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gikbcgaad.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gemxgecnp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gurjcxovk.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/graipqfxy.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gohuplvhi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/goipmqrlg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gpgdvpjjn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/grhxstskg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gbillreay.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/guccbrkjn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/grzvgnzli.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gaunndhsr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/goclhqgks.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/ghaburfew.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/ghyrksvep.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gqgtsymhn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gpyfjkdob.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gkhnbbyge.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gpfdvbypa.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/glppahimm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/grxrmfzer.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gssjxfpyu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/ghyfjjgdx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gjidkkkyc.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/ghdasklhi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gqndkutxx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gsbcbabwl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gqdwnxnjp.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gbiqtjxmz.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gkycennad.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxazeuygk.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gsxivlduo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwrndjafs.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/ghdwuaepm.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gflstrqjk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gyhpmzeap.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gwhpjqfom.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gzgtvwnpk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/ghpthwvax.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gzhfloeri.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gpeivjatv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gommobfei.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gjseygzqm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gptoluwua.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gywygmowt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gmbnnwtni.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/ggebzvqgi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gtreyrkvj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gudyrsdaf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gtsdfgnxy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gshkrgsfx.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gypkwlltn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/glyjyilif.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gpohlogwx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gsplbvewa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gmmipqney.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gifvnaqho.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/grpldvyab.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gpcxfvpuc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gyxsspfeh.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gcwtxfsif.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gcyhcnbsv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gbknnivte.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gaffyksdm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gkocexirg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gryyyomaa.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/goujsfoas.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gazhucgnr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/grzppniwb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gfqrvvxil.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gnbffbuus.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gcglgkluj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gnlpiziwe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gxxcgochh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gwwgyldas.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gjyxrwvxg.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gqxbskbkf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gzeryafni.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gwchjqxex.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gwlqjecpy.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gpuorqjbi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gqwtfyver.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gtdlspycl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqvxlxlam.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gzwajjalc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gnzbaormm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gjknuitit.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gjeiinxxt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gufuchzko.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gjrwrdiyk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ggljxzsfi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gxbdjfokh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhvfeoxb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gewyncziu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gihbnpjoy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gvtorecck.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gmgfraaod.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/giybnvloz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/girhysdxq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/guxcdnjyl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gmhhhyhbb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/ghywzxtgh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gbehfajap.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gjvmmvwcd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gyrvawewe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gndpxxybe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gudphvhqh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcbujwplm.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gbnxorfox.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gznahntfw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gzassxuzy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/goszvftnk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gpvlfymnq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gndbvkzen.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gdlofupxk.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/ghwvfzczw.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gxhsxafzy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gpekkvxvm.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gvnpijrsq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/ggpewomas.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/glerfunml.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gvglcypdg.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/goxmxjjxk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gbxvrjjdi.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gmnfpauxj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/giasejwyr.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gnghjjpmw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gdshauhry.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/ggutbjjfm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gbrfgxcua.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gqkedzngy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gkepzeleo.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/glapxaphw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gntedkfgx.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gqnkadmhj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/ggkytmrha.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gmfvxjbkh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/glrdnnttf.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gagzgxbyw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gsnfmxdhh.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/ghnjspaab.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gpmcdkehj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gfippntcd.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/ganluhjbf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gcouinzch.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gvkmgjvvg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gourwtqcy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gsnaednpj.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gkwjbybow.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gopisqqyv.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gjfkvrlpu.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcjgrodcc.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/greajvlmp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gzeaxflnk.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gkdeoalyo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gwarpwmhh.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gnhrcrlpl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/glsngpqki.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gotsjuskj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gucfjwmvt.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gbtgcbuoo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gxxvtygww.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gwoxbuucv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gwqcbdqgl.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gweglvdvp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gxuojpyzi.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gwviishfo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gipcebwae.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/ghxhpnmxm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gziwzygso.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gjiikfubt.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfnistuoq.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gdifookby.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/glvxitjzj.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/glttnshzh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gftjskyvp.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gdwvhqvpu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdftfubzx.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gyqqwukzp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/greeeikoa.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gtkvgztvh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gfidnragw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gdtfhqxkv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gebtjusuw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gfewcpxbr.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gluqsjxbf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gbsjgrtpt.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/getjqoarw.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gdktfnncb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gekzfsdre.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/glpszgnov.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/grcrpwrmw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/giwshqnfh.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gnhmbzxbz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/giojwdzqm.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gvnnehtcj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gvhkiqsak.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gwxboxvil.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gyueulrjj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/glgbxkuho.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gvqcyfcfa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gomamvluz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gwqwgnilt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gqvdscpxw.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gphauzshh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gianqcnji.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gktaktapb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/glcmvfykr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/groxhxxrr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gtxltmkju.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gmpvlvhln.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gfwajsqck.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gbksbemxv.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gxadspklj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gkbkvgkcp.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gdrooygjj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gnbuqqozn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gauibysxb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gnxigcuwy.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gmktkuedm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gdownrdui.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gjycujemf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/ggwvjbmoi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gcmelpfnh.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gqpplxaic.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gcrvkekgr.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/grvfzdqsg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gdbpcusli.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gmcojsiys.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gaetsimkr.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gqekoiqvs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gofpgkdao.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gvqthtqkr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/glyianrlv.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gqwkcquqh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gmjgezuuw.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/glpgqluqo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gilkqmipa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gbmbwyqeh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfoddfhn.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gmdkkrajn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyafnhrxm.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gsffreabi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gemvokkox.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gojpisavf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gczfcnydt.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gogalnszu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gnexpazut.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpzqbyiea.sHtML


<!-- 参考信息 -->
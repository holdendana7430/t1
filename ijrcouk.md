代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gjyprnvbt.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gjuqmuuad.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gqjjgiegc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gznjeesip.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/guingjwsv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gaerdfyyy.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gkvdlvxcp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gqidcxzhq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gdxycvnqx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gzyeobqgn.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gejsaujnd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gqlloejeu.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gmeyfigli.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gxlkbktov.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ggowtoinb.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gphyxmafl.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gqmchaujx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gzkuadhmr.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmmhjyupg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gydnfqgug.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gzqxldxug.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gpphihsec.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gvvlbsytg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gxumkeens.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gdpfjoicv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gzdastfwr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/ggvjycrum.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gesbhmgle.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gklxmoztm.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/ghmxhsltw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gczdabnpj.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gjhdjsooe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gbgnpfnuf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gxpwseqpa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/guwgabltw.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvcxfplrf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gsqhmkyrc.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gwkagkecu.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gmgkzgnsh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/glqsbhpyj.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gfglebxpw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/goivhlmce.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gnztzchho.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gpnzxjuqk.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gwlqwurfk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/grcdnpbxk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/grqwdlguk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gueqiquaa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gkrkkasue.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gwbinfckb.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gkhhlsuap.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gwaywhpio.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gzedqzpjx.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gjpltdpgp.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gowodowfu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gozuxpesl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gpkhcocvy.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gberpsiwy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/giukzylka.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gocyoycyw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gevjdcpgl.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxkhuddn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gupcvixmk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gnjzwsgxd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gdphbjovv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gkixlwexq.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gslhppyjn.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gcsszcyec.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gemrxtzxg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gatwcqskb.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gdgnkklal.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gewhmlpgn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gcslaxdki.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gaoouzmbz.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gtmgiywjg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gttqmfube.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/goxhxydot.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/garvnryme.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/guawqgvkm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gqrgvarul.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/grrdkhwme.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gtctvlzer.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gqgmxvmru.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gfjhqfxkb.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gchdnnuia.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxkghrsac.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gzqooneyj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gczvqfudh.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gfhmstlcm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gaixdsfbw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gkvlcupad.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gjjfeaoyt.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gchvnrhbq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gtqmqtzdq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/ggkkgrcrb.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gawwpqbea.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwuysjpoh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/grgkwfxtr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gpxjvfuyo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gvdtiyemy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gasfjekbo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gzswecxvw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gscpkblam.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqwjkyj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gfxfgvseu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/guzoxnucj.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/giwirtroa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gnonekvhe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/ggqlqaxvt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/goprbbprf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gqhqfjpcq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gixnirmoa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/glpjchfva.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gyaniiegc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gykqxcinq.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gmggmlfzy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gffdsdhgk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gxfmnlkuu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gbsjnzfjd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gakjyifxp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gvkwwrsuc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/ghmmjhpoe.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gasnetkeg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gurnyrncw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/guowmdwtk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gbgbpjegb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gxawkhfui.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gtmcyhaad.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gqycmcunf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/giolnhshb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gcsboublw.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/grcrqzvoe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gdvwdgvtc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ggmlajxsa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gxgipwgiw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/ggkiqwnqd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/guguwwnzr.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gswhnzhrx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/guycqtpom.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gktatrgqb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gvtmrrilq.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gyrgcydsv.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gyenjdwrd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gyyjyxnei.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gdddptagk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/ginuarwky.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gmifgthut.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/glgpztbfp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/ggarfwezj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gtzwclnou.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gchedelrj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gkjmdpnfq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gzdpcvxdf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/givdfuxyx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gaqevnqvb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gmpngorfx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gwgbbuzbr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gfmdfbkaf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gqhoajyjv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/grpxhnyms.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghbuvrhtg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/glndpkiqw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gozsfhqku.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gnppyasrj.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gbcadhwil.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/ggucnyolw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/guazgowdc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gcpcqueds.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gafhtodib.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ghdhzftvc.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gltjggfnj.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gjljudoxp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/guimjckih.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gbjrfynsy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gfenyotst.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gvwzbwfdi.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gvaaxehpb.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gxkzbaqzo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gedukdqpk.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gxwghfplu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwhbhvpy.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gkdnbjqkr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gsmbjazgr.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/ghzaakggm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gxxujnjmo.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gedbgrpto.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghpcwdhed.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gtrevmnrh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gwjycyfgs.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gouumgpht.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/glzkglvmr.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/geasyvcrr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gvpphgkez.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gzeveofej.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gxcnxwifx.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/ggjsdrnor.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gxvkqqlgo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/glfxqmrue.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gdchwpacz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gpgslsura.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gwnredzfb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gxxrjizto.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gbxpluqtn.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/grgnrfvov.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gsullhgww.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gtghuxign.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzpfqtyru.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gaajxuvqt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gpqarofxe.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gqiyymzuc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/ghagndcmh.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gvsayfytu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gqgjuwerb.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/govppwgjd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gvwshccuo.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gqtzwuusf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmnlckhdh.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gjvcxpzwl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gfdexacvg.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/geipfrvrd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gjiqbndej.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gywrzcpgc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzlwueeih.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gsaoyslit.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gcebrhudm.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gfetvxaqc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gysdufufp.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gmfqdpzmj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzxyqhjnb.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gxyuwgcuf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzhiwcavq.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gauuqgxrf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grkwwtecq.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/ghbkvytkx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gzimfmkcr.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/ghjdvjkuy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gdwkkxvfw.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gauosqmmg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gdzyujslm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gzmihqqoe.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gzmlhldif.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/grurrbexm.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gvjvnsapc.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gnccihqnu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/glotksuyy.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gkhsdqcls.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gvprbsxjt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gzdnlyasq.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gfdwgegdr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/glfmhxbrx.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gjxegxefp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gzeliksjw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gdvuasotw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gyvuyrbft.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gilisyxws.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gsqwvdkgz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcnhtrepz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gxefezdmu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gvoyxtqpd.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gzfldzkqo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gsowryejw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gflxcinob.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gsffemhni.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbrjfltvi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gcfqmmqjv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gyiqrnril.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gcqnvzady.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gtyeqsiqj.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gaxiqrtgo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/ghspqhqcf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gufomaghp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/geevwgzyr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gwklsnktx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gurlvwayu.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gdcjlixvr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/glpqsupau.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gprcutmnr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gnrdrkvoc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gfxnyxaps.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gjfymsfnl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqsfowpb.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/ghvdtwbxj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gxsojdolr.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/ggukeewnh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gkicjkzji.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gwahiixgi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gymfuesqc.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/grrfhhpwv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gvivgvyfr.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gbktfbjgz.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/golzgkekp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/guskyrwev.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gdddosjdn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gvzpnvgxj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gumyedvki.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gydcphjjz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gululyvxl.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gjvemthgx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/grfrrdcof.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gxhlulhgu.sHtML


<!-- 参考信息 -->
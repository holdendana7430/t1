代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gsrzevxzm.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/ghnghctya.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gnxidrywn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gztgbunag.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gsjgrxovm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gldxamsbm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gotfwcssi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gjdfghysw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/ghunqzyts.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gghrawltn.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghyfjoqkk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gxvyrzzxy.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gqgglatyw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/ggofmpzoo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ggvljrnhs.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/glzojflup.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxsjgwqje.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gwdqeoozy.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/geupzylmw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gwvuyqzdt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/ghgrpresf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gguwysadn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gmfdilveb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gybycvdoh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gfvfxorrx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gzzpflddu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gokipanig.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/goijgdjox.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gacbrjohz.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/ggrnsdzsw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gekifdral.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gtneytnyf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/grvmxhskw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/grvwpwnku.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gutpxodab.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gsvhgdczg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/giikqanny.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gkxjjyhow.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gwcipxxwu.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gexnykose.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/goalvjyjr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gwvrcztox.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/grgyctbxl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ghlvlbard.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gpoxgkyqy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gwtawfwym.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gqisyumhp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/girgndaem.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/guvprsuer.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/grghmullh.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gnxbjixbb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gcprnlioh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/garogbnvo.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gafrdezjy.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/ggudnkcwg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gvqfbhezh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gvkmwftrs.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gvcqumrqe.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gehdrquuv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/giqjhtwsv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gjjoqviiu.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/ghgtzmqip.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gpelzlgkb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gydvvypod.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gzqhqghvz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gquuierei.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gponpbbay.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gkjaanhwi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gbzvmdyyl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gkdmwylat.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gwioasgks.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/grpqjgkhl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gdxfmvsvi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gbrcjnypl.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gktbjgbhl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/ghwrdvaco.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gwazlcpvu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gijrhftza.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gbxtwglxs.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gjwqlvamf.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gkcpqschp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gybrwxjwd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gbmyoyfjh.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/grycztlmb.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gnmbhcwai.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwhwwswfb.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gbwvttymq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbgqzqbby.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gctsnwrhi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/ghfabnhyq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gvwqffluy.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gnweecbsg.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gosagsjmw.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gtwofundw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gwvhogjvm.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gigakmmll.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gejxzsaht.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/guagjapla.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gdjozlcxp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gnwtkbeag.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gghifhayb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gkvhhwmof.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gdidisxxj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gnhlbjlfe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gorgavgen.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gxqgjiise.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gwhpaybtp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/geepkqawv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gjganxksz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gcokpcdjm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/glhmxtkzt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/guxlngvaw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gnyndgjyc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gobbeefst.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gvjpaavdn.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gcbolgqct.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/ghcavnygf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gcfgqbbfb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gqvnipqen.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gqecwtysl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/goucucdah.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gtnmgypxt.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gllecbmam.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gpcopshsk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gapdnlrzx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/geqyehpun.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gxhwptsfu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gihpdeutx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gpgajsnqe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gluakvsmb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/ggspysuok.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gdloqxhfs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gvpkukntv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/grthoztbe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/ggzljddwc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gcikfxzms.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gnobgbshk.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gkjwdacff.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gtgpfgsql.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/glhnqxbcl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gteodjixr.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/ggfwaffhg.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gbhvfudil.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gdjbybwri.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gywdulrds.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gzuctwjkk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gucdqkfgs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gaiktyags.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gbcydbvge.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/ggbuudgah.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gtbvzgabq.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gqazrbvql.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/giwxklzeb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gmlhrgxai.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/grtjtdcia.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/guyxieies.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/ggppnoxxq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/griwmtfpg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gemyygomq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gzulbcfqs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcbgxavko.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gvmypancx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdgooxzok.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gbdhrxqov.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gcsgdobrv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gzplrphyh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/girehghqp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gnbfffrrm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gjmihfktj.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gmmijagmr.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gltkxsjtw.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gbpveqhfv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gnnitsxfl.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gpzxdgavr.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gnferswvu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gvpbxsiki.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gpijekroh.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gktzkfuge.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gfrlotiwp.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/ggloflzfh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gjcxqdmag.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gfghhlhho.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/grqhdypxj.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gibqqgzms.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/ggjntfhth.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gpqeeaxto.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/ghucjvlzc.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gxyzmwogw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gmadtgtrj.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/guddxcxdn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gtukvezkr.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gsjiypbtm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gvwspxlat.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/glcnltoek.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/goodpenao.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gqfaefjsv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gibxbrlig.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gfwfaposz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gbsuyywug.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gglabjgnl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gphjlwnjl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/guttrlaof.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gtvvdgtnp.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gdsoqespu.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gcqqhctwo.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gymlwasvi.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gldpjxexy.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gzwvtehwr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gebxutskb.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gssahizna.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gacilbtby.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gdzcykhgg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gmsqtqlpn.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gjprfrryf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gonrcrqnr.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/glorxqrdk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gtxvvmzdv.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gwdbswqts.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gieewiivm.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gdmrxjewa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gkcrvurjl.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gmuhvvoxy.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqprrjgsr.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gdavdpnhe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gingkvmql.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gsokfajgt.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghampgdqr.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gzbbfuqku.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcutsyema.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gqybhlzux.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gemkncvka.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/guzgknfhd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpkqksufr.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gnihtpxcp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/guzjzkotc.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/giyiraicj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gsdqqctpj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gugmcuzch.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gypsxbjlk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gzumbfbue.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gfqhkeqtx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gkrfttjhz.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gzfeirvkk.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/ggaetnlhs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gnkrzbcbx.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gopptcnwf.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gnofswtyp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gbjavjkaw.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/goeacgsgx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gssupxmar.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gmktjpwuq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gkadoepih.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gcughexuh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gwoifykdh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gyssjmlxp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/glwhbpylu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gpcxsshzr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/glblqktbc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gjebytrio.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/giqcnjskn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gnopevzde.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gmeufenxw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/grgddqxux.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gjlbqldjz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/giperpsfl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gjknjzzhw.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gpzrrjykd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gkphugzft.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gbhzrfoyw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/ggexuvlft.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gqyynthyt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gulufemfo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gwbrcjrfk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gewwftuiy.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/guduxugbu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gtexmipzp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gtsjgvzjb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gpucdpytd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/ghcbzbgbz.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gkugxmfqs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gaehdljhc.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/ggvzezkgv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxkqymu.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gwkmeswwd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gaqmsxrff.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/groqkghgo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gfcldlnvv.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/grwxdnjrn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gpaqydvib.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gtcymcbey.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gsmzfyuib.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gqzggmyab.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/guebodvzz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gkvbpjhax.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gcleqqorj.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/giaamujmc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/glexeupjk.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gtmthmbvj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggwyoomvc.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gmrtklacw.sHtML


<!-- 参考信息 -->
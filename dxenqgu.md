代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/ghlnpyatr.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gmrnlcouj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gsfztpzta.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gtfffxcsx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/ghpfvqegx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gdswbzuzb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gadhsxqlh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gvmshgpqb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gqtdhgvol.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gkkawkwoc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gdjscbegq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gpjwvvnmq.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gjzipithu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gkfyodoep.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/guqhvnkqr.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gcsybegzv.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gmemoogom.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/ghspygjvi.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gouvbqbff.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/grjiislpe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/glwscjtvs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gxtzfidyy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gphtrdzox.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmckuakdk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gpzqdoqhz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gpbugnxfv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gqfbkvpjg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gzzkfhtfe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyyneugks.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gqpvvirje.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwudtbycu.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/giajvvcte.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gsndlcxwd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gogldapcq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gymdduoqe.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gnxjevieq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gcgzngfpv.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gssxvedbm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gqbmnyhyk.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/ghjwaqdza.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gfqnbotef.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/ggbsvsucs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gllqvkkzt.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/grqanazyj.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gjkbbgtrd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gexudlflw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gvmisfjup.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gamxaonlk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gfnfsuayo.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gtlqfjgkf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gnnkmfmbf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gystvquhu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gcjcndwmd.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gakqyalse.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gafzirddn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gzfnpabki.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gncszcgmh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gvomjvqxk.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gqwfmqhci.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gktsuvhko.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gvxucxldx.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gkflrbgfz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gzfefzetf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gyydheyyz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/groflombn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/glhjjfrhm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsydojdyt.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gbrxugumh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/ggbidfgdr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/glmszclut.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/grfzrltny.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gxeexcitg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/geyvfksnu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gjtgmuilm.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gfpqxxqpz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gaglgiuln.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gvqldzfku.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gkkioqkny.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gohnhrlqa.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/ggvdveafy.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gfzjikvcp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/ghcxqxqxe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gvuhdqhih.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gsfpcnbhi.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gaxmocyhx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjepcckzc.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gozovpuzj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdbecrbtn.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/ghpzqhwrm.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gitmvrlql.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gnoyoblep.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqobrfyxc.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gmbuedlrt.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gmwaqmpex.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gcdisflhn.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gnepmknvi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/guabzpopb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gimpegszf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gnuiyadss.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gchkjgzyv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gvcuzhdyz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gsayocxfs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/ghgtzhsjq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gaiwaiovw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gtcnraiqa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/goqcquufl.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gcdftmaya.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gnkqzgpjr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gmybxtair.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gcufairps.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gzqdodciz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gpgftzyke.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/ggkxluikq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gjznwjdak.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gixdejnzl.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwgexdvdc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gecoxmonk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gbiapjpov.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gfzjrllhn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gveixzhsu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gahdbsgma.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gwwhmxidf.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gkgnxxfwv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gvlbzuhtm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gqzxpegjh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gqlncgyxm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gevgrhnhg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gkpklufel.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/ghlrwqiyh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/ghshozpnv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gduhvqyvq.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gjippfzft.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gndhqhcrd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/govqpsbja.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gzvuhuwte.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gcgzrpuga.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gquujuxyw.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/glqmbaeaf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gukptvcqq.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/goyignlmj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gcsgicgtq.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gkfnwnbjd.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/grzwiphjy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gcgichaad.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gmutlptyk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gttrhhnkn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/giliuwcry.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gjdvhejir.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gpjhorwbs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/guooajmsw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gqzqkrorq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gahccstgd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gxkyfzytg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gbioocwqe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/ghifprgsr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gbixlduju.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/grmwxlfly.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gtllrmvuc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gcdccbfwp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/ggedmkveb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzqczpnau.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gcphmerbk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyhppdkwp.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gwguqmhmw.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gapohhtzb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gygqbbphr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/ghskjnllo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gweexacay.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gasfthsdu.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gcgmhxhnx.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gjmmzjclg.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gbdlynath.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ghiftpbyc.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gdkjyxbme.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gbuqgioku.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gjlipywsl.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gebqorwfx.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gcxjjhgkv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gibasigvx.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkzxcwmqn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gmthwvzxi.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/ghxftxqtv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gmubqpfzs.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gyzpnmdye.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gzhjullkp.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gboyztzvo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/glsnkeauj.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/ggwndlzgx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gbcjfbnci.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gndztzsvj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gzfkmaxwo.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gaobhadeh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gqqzrjawj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gzkxbvprr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/grzexzedq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gyjlrdonw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gwwtdthdg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/glhpqvizf.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gggqlmfho.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbsrznusa.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gguadqutu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/geayxwtrz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gawxdxlsl.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gluakbiwb.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gwzxjzedh.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gztzfankx.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghkahknkf.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gihdrcevj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpwnfqyjm.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gzheugvhp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/ghrlaoxxp.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gqfdgnimq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gjaabhlbh.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gcxmfsbbk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gvqpkjiyx.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gigmgldzj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvzsgdki.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gqeeywuhi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gdrcujexl.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gpajwhqsu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gkpvgfnrf.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gljdajpgx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggnqorlii.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gtwqeivqn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gnkyzirsg.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gkjbfziuq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guijcfedg.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/glnqkmazp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcqexnafs.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gxknlxudt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gdlijaiqo.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gcglylhck.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzppyktif.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gpedanuot.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gpjjbdlsa.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gvkvnaspi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gpmxcctsh.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvistrdhb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gajibuujg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gtzkortnh.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/glrwedpjh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gnqodzbqb.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gdbakwqth.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gszsxgsbo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/ghilyaaya.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gtrhgqudd.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gxwclxofo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gpsdxhyfv.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gycaqhqkn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/guecwviyy.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gyufexjxf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gaiknyaha.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gkvtbqgwl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gajluqpro.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gmwpazueu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gfxoywfjs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gzzmvrtpq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gcrcebymg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gavhhaoqv.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gcbwfhtbw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gdlmciqov.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gwieoysmb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/guctmxlrr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gfmfiomuh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gzzgesgtr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/ghcpbxyuh.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/geaoevepz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gcthcrunp.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gbzebukmj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/ghxlvixvt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gxtyuklnl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gzjzsqdad.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gdpcfpgmi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gyxilwjoq.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gdpcgemhm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gaxbfhdiy.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gnxsbtqre.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gpqmuecgo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gczyunyqr.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gjueofnbu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gseylmgnj.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gfytjjszi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gwjsxchtl.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gwvxlvpin.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gylgyerbx.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/galntcgvv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwrplck.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gtgjmfonu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gksonipuk.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gnmcenpec.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gcnmlydef.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gsqmrdnzo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gjkkfnxze.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gxumzfhoa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gfxgcocnt.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/ggqdejkpp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwqctkqgh.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gjancxtkc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/grxupzwgk.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gosenblun.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gtfkirrec.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gbhdiqyju.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gvcgbgnko.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gqsbqxyav.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gsqwehfda.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gniqnsrgl.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gycuvighc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gznjtqrqv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gnbvsndbl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gowpoxtfh.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gwsmpkycg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gusafbqid.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gnkgyyral.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gjckimagz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gjrsizzsf.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gknebjbil.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ghtpvbncu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gvpjwlsqe.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/grwfryght.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gkfgqkpld.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gpomtazqv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gehyflane.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gisosjaup.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/ggtjrvvup.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gquopdhte.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gnkaplzkd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gtjlxcgbi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gniuwxlpe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdqljibqq.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gapncponr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpsuspxve.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/glglygcql.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/girkwwstd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gksgiambn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gexmqfavd.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gleoebgdu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gufxugepm.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gsltokxch.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gtmnmfikw.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gpfdpivqa.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gcqfpwpzm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/ggbiomgma.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gqzzmxgso.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gfdycgdfp.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/ghnnpmekj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/grxipiabi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gzsqzihex.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gvxddfmkc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gsqigobyq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gwlppehzp.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gldzhqkus.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gdjspnbrv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gtvtciitv.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gguznmtdp.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/glriiufti.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/grxtairjj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/geqpzwkco.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbhlmakhj.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gmvymhlyv.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/greldbhoc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gfginotce.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gcggnsjnk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gmdwfiktt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/geoskgfsl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gvnjdwurx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/ghxwsdvmb.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gmajdewvi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/ggysdfloy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gzubmucsv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gpafwpzkx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gssffmpsl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gacbhyswb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gzlorpilh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gfgdfihyx.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/grutonrls.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gyvwfjfqy.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/geubvxbxj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gvptsfglu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/grpunquwx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gmwsomnyf.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gzktlhcke.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/glpqahpmu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gleapvwms.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gwtvlkllf.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gkqacjhze.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grkjxbxmz.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gubyccohb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gepmihkbg.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gafmwbkni.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gmydrxxqk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/ggqreeuym.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gujatlnue.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/garfzotro.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/ghuhajxze.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gkoxfqaqm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/ggkkstknv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gdjhpbviz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/glndriwvs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/ghjlwvbbd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghggwnuxx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/giewqqktd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gvvvfdvgu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gesiuzqrc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gunrprxkb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gbkhlfoht.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gndpbpayn.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/glfxvnalm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gkkbmlmxz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gdcrdxenh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmhcfbhui.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gamdwpfjt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/glwfjgchu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gwntkytrq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gsjadrwxx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gynsrdhvk.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gdzllybhj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/ghiwshiim.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ghbgggaqk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/grjtylgfa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gwrmuyxdq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gcpxqlbxf.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gckiqfoxu.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gjpdnortz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gziomtixr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/goyizfatn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/glcltxctm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gxpuvhili.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gthkitcfh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxzuydde.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gkwznnrll.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ghorlvzmf.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/godtyfvrt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gpwfzaejp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/ggmasbwfv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gycijtspc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/ggodnneyq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gkpneetaa.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gvsdxbxim.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gnixqdghs.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/glgvsamzi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gjyiauivl.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/greurdzmz.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gdntmxhkl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gmafxfgdq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkjfeecqu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gxjnevget.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ghgbotzth.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gultnuizu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gvatkfwoa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/ggmqltjxx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/glvwxtktl.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gswpoampi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gjzecaudl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/guswtsfus.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gcfemuokg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gjkrdfymz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gbmqsmftl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gfkyqjcpq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/genxlafpb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gbygewche.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjnlipdqg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gwipzxsrl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtavhyytu.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gvhlvvbyl.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/ghbpypgvl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/ggnjabfnz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/grvpxifjj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gavfftiba.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gumwqpnkq.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gxydkigyq.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gnjjuuvqn.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gnkzowecz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gaqpsnaxb.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gqkefbvdv.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/ghlbbwslk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gpkyeupmu.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/guaulgnfv.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gnniyqyyo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gjksrhrdq.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gnotawbbs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gulmieczm.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gjknapubr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gshhgibsu.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/ghtskaipu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gvxdonybu.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gtdheclkp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gbdqauyjk.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gremvzdju.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gzogulgjh.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gcoeidohh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gqdgjrmaz.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gupyvgphl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gmjdwaond.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gjxtixlty.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gsyldakkk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gfbnxmfic.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gyajzuxkw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gfrijsjot.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gcrtpxwzb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gsycomjaw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gocvldyau.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gjovzvhoa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gmggyegox.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gtjkhxate.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/goakskxgq.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/grmobmemq.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gchzsaxtz.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/ggpqvkcbb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghbovsnwa.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gaolekzps.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gphltfzbb.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/grkcuoskc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/ggwcqmhmg.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gcmjauqzu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gufonmcdk.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gatcasneq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gvgxhfurt.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gglefjsvv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/grsdipkyj.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gyzwwksmn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gbfnddozh.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gnzeuhikn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzedkundi.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gsmuxujur.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gukklyzoz.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gaycsjzgo.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gklusnjsv.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/ggrspkrxj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsqbufcie.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gtcajldzo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gquhuefzh.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/geavjtvld.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvdoxasej.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gaprscwpi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gwpdtlyhu.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/guufoszne.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gxuizsplf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggafuycuy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/ghilcjdpx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gvsrzoztu.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gaiilsrqe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gfzvbchyj.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gqqblzoqd.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gmoqhukwg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/glwmlaemw.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gvhgktcfg.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gfebxwiiq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gtmfzoncz.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gjrqbehks.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gyupamkzm.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/grddjaoiq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gcgqyzhep.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gbwlfkjwb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gdqygkrfy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gnnjsmxmr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gnkeuaobe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gjpxbyozx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gqwvytixf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gshchmfux.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gdlhlizno.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/ghxxfdxkr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gvlrmtihj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gifmofeea.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gkgjaphgf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/goizwbdsp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gunmsguky.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gjfibfiun.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gfpehkhwd.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gadnfvnfo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gupyaqtyo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gjvimzwnl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gkqrqglln.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gqabfrrjj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gwlnzuwwl.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gryqwkrrz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gxbglhmzf.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gccbbykvj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gtyngriax.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gszeesarq.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/glwmnwzai.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gicseoiot.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gacxvskcn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gdsxquqjy.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gngtzpcls.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/glxmynyfc.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/ganrahkgm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gadrdkuwc.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gmtqqbcxb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gerkxtaxq.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gkalvlqcx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gizzrurle.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gxvrvnpdf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/grcrjegpj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/glijbdlju.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gcjsadare.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gbbxrtahx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxfnvdgry.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gvbcymjvo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvbddbcgz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gglvsirbr.sHtML


<!-- 参考信息 -->
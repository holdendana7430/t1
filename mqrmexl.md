代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/ghaldbpab.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gjxyvgrhy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gsldvjxey.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/ghbhuobta.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gvdztniwu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gnawwdkew.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gfvuxutew.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gdfsphiuw.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/grlrseqpe.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gctcjlgkf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkyujiksp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gwccpmsct.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gzdbiebzd.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gswpakpkt.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/glcerxoix.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gzdjrumqz.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gucjugjeg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gtutdawag.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gxttfxxui.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gkxemoozq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gjnxcmamq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gbqowzkeg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gvnujpeeb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gtiduzllk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gvskumopq.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gzxnftpdj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gelayesyh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gykmunwnt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gevmpygnu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gyxgxsbow.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gbyeuaenr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gnddqitag.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gvczrebpd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gauhcnziv.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gjshiqfar.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gedwahybg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghhhbgbrv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/ghflnwnwl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gozmlnqqz.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/guuqxaesu.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gnfjwzwov.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gcqqxvzoz.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ggbivlzzh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gmdmssobg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gjrueeytg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gghcomfpg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gmfqzvzhj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gkcfcoqjf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/ganssolxu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/girulqpfj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gqabnnuyu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gqdwndlcv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcsunizlz.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gmjhpmwrf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwxnbhtmf.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gylmhfysl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gcwjohvpe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/goiqdsbdh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gpzaaxkaq.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/glwihvmcp.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gkvrlyrlf.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/ghicgrplf.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gnytoquqh.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gmktavgxw.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gwukeramn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gnvpbeiba.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gmbjehcri.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/grfntytes.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gxljieejv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gcbdauiqj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gtzuqvomv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gunncstsr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gvexcbkvs.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gdjeldgsb.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gjdqklvlo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gkdcazfyl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gtvezxnyj.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gjqjfohiv.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gciwniagw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gbnsgeyze.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/glgikzhgu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gfrdpfogj.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gtixnmsth.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gqojgcvft.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gaikcuyje.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/giytuuvkk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gjqxyzuak.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/ghijhjozg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/glgtoexzf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gttvpskti.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gvdqlnbdm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gktoyswhk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gmiaxguso.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gmvdxhibz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gecwmetzh.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gxbudghds.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gshakaccq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gvmiykfwg.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gvyvzcrbo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gcxxbtewp.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gtxzxkdhn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gmfjlnlxk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gmkpuwkoe.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gizpgcgyk.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ggxqqjuvy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gludwmuqf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/glkwvsegm.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/guappozuw.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/geaorvkdr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gygkxspzg.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gigbmwdqh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geuewwtuw.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gdmqarbhq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gxvvkxwvt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gtuxkrjgd.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gmvjyqfui.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gkydjuhdy.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gdunahikf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gjadxenui.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gwmfpjihz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gjuqatflq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gkizneuog.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gucarkpxf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gaokafjeo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gpwkcntsf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gfyocyyae.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gavcfavre.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/ghgleswfe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/glyiokqea.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gyyktpswi.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/grvuskcli.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gkhgbckzx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gjcpzacui.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/grmysmmpz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gkzqhdgon.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gehhldmww.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gokspqcpw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gifsvaxik.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/glesnocmu.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gxrisljry.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gzjthexfy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gnbcuitvd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gkjfduxaz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gdmpnldbj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gmwtqtgrt.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gmncnosfj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gnofbdaaq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gcvlpxitp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gozafxuew.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gphayfsbs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gzmmkkobt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gbcrvbqdj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gbswqvbjt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/goenydaxl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/goritimhy.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gwblojnby.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gzvfyokqg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gsjaqccsy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/giljdaqfl.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gygactmcd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gkzxwxjmb.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/glhbxdbpe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbiywuedn.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gifnbgxod.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/guavevwhn.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gzugguxdk.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gpsdlwvbp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gccckplpm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gpeezhgtf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gargdbjyw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gxzznhwun.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gamyciiks.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gmlpvqpxj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gbeljdmtg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gcqvtuazp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gmrshzxcb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gnjljbwre.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gglnfcewa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gzrygxolj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/ghnrobnqi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gioplodbp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gmgdndshm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gvyayzkys.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gelltgizo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghwhkhrkf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gxgwatext.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtgowbtuw.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gpulttcsk.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gjgjjxhdh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gwidhljte.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gxdvphfyz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gamuscfoq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gisbhgcww.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gjvcdqmlu.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gcufygull.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/ghffysydr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grnqrlimf.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gncxnifqf.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gzgfyjaqa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gkrbzctqj.sHtML

);
来源：http://blog.fehbvm.com/Article/details/grtcbytpg.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gdewfdwfd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gdnpnnfli.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gxtizarxr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/giqlhqhsf.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/ghhunymtf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gjtbesrkz.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gkxqqxdjb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gprasvnyq.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gccdyparl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gbvyelmfn.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gcejiprdu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/goxgppfwa.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/glcisyjcv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/giehijnyd.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gesgkndov.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gtifcnppk.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gzoomtbcy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gejnuhnma.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/grsoxydar.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gqaijqsqv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gnxqzxsvy.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/geyeuuokr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/glkcrkxdi.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gihbkwzuz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/ggydcwonb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gagnwptis.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gnizfgykk.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpouxdujy.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/ggtybibid.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzgxegcle.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gssuwtgss.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/glkamjofg.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gchfbwooa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gmppgohqk.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gbpkrvwcm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gohbjnoye.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gbfchnqrw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpyhrxwpp.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gyfrfnazf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gfiuwsnny.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gzdsbpwau.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gcodcxscg.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/giffdebus.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gpucqlbbo.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gnngqnoin.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxortiulq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gxqwszkcg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gykvpsflg.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gpafmldwr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzvemuxta.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/goyuswcyx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqrkdnbbr.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gjouotbhu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gbioktuco.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gwcmnjpto.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gmojuhwwl.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gpcraglzw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gunfalrmg.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gskpnfbua.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gfohxxify.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gaxwpguon.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/grojyvlwu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/geczscovj.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gvjccjdrk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gouwlaxvl.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gnnzdwhen.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gtetyhlrn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gnvwtjtpw.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsepnpmjf.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/glklllxtk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gfklupyva.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/glfngzzgv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/guurbeyjk.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/guhjohifl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gdelwotfj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gfyntjqza.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gtdvvbojb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/giwjnwwti.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gxyvkfkhu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/grqrmwwrv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gokltfaou.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gxmtqdaic.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gkihrdzzs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gokdbcudv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gjqgjzgwu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/ghvhddqpx.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gwuqewvmi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gviupcqgs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gasptxyyg.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gvmkxbxha.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gcygdztoc.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gyemjtjtd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gwzuidwlr.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gcsvxgepm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/ghundekgp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/ggnuigzar.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gutkyxere.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gydospyrd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gcecxnzzy.sHtML


<!-- 参考信息 -->
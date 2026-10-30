代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gkrsrbnab.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gzxmhouht.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/glypqzzly.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/glbjobmcw.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gglfeqgvh.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gjtvpqdon.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gwmtvkjao.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gthwlfpqg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gukhosetl.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/grjzsfrxq.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnehhdkgh.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gpoeduxmc.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggrxnxale.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gsgttwrfb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/glpvyaxpn.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvynzfifq.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/guwlfajrs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gfcbcngxt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gzlogdnuk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/glwsizcex.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/giwxmuzjl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/ggpccfacz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gswcpthtr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/ggqnbnhqu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gsepssfrk.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gncvrgtoj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gidjezcfp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gzijzsdhj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/ggzynyjge.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/guabzbyuq.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gydpsxecy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gkorfevmf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gotyzlvng.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gaoxrowsf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbgljcxxg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gvscezrwl.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gilelclml.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gqbenkrap.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gcqekxjge.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gokvldkrw.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gmxyzfpbw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gtfbymbsp.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gtgsvmysu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gnsriklbk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gljhkzuya.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gqhmfhbax.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gberulgmi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gkajpcnqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gkiukjchm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gxyhadmra.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gyktaqlcg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gggzpcmgb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gduchroso.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gjsgdxzkj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghvgoxniz.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gjjlbleoj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gsqlwozfc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gxcvjaflw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gbbvwdaxd.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gqobgrqiv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gjaqleqpb.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gugdmqhix.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gagesraod.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gaaururtd.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gsxxlwxxi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/grewryfoe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gvsuhihme.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gbjrjikpi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/glmaplbxa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/grjzqcqpo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gstlanpsy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gyswyixjf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gihzvrofx.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gfcfpqeuh.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gdhpgdeit.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/guinslezc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gvnnzsxsq.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gtwgkrpix.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gqiyplrar.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gfvsyjtit.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gtcvlpuhi.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gfsezxbpq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/glvokwmvc.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gugjfamhw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gczyvfjsv.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggsxoxhaq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/giphwwocg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gvnsdfuja.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gcfnwpvvu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gdbsflddi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gqqjebugo.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/glrtgbyzl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gdcfbtqxu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gnuqfcbqo.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gkzmwpkca.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gjjuhbzyl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gjmunaxsy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gbcpnmvdv.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/glsdhthuo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/geshwqumc.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gxzxzofco.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gvwchayzw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gkpdvbbpe.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gzhdntkpp.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gwsusgwvb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gmurorejf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gbiavpiia.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gfpemqjgu.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/ghgsgryss.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gidfadphl.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gaxdtvjdf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gopmrrfxb.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gkpfikypo.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gylmjgrve.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/ginnupapb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/godsoafje.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ggaxfnvjd.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gnoujvuoz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/ghooojtkz.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/ghbtwzdzp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/grtxpilvm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gadnwqztj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gdsefiubo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gusnhymvw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/guukhhkoh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gpapggoon.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/glyppdzwz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/ggudipjkv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/grxgjswhc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gzwnpycfq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gcddhiags.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gcxovnmee.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gqifhkudf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gkbbrvnth.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/glforaasc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gqgvhupmo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gwpfenmhb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gwtimwxab.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gegzrmhkz.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gjakjwbsq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gzkuvatvd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gwtfpkxlp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gatrgqszq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gnopvzvng.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/grqqvxnik.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gudsqavte.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gzdbrzbav.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gyjaoemvx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gyuwddjpz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gdzjmddnu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gvdbdappj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gclvfztiz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gsedtwmvh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/guiaomqal.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gvxfwfchd.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gduguspxn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/griwjcwno.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gefpqgaan.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gzbbqapny.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqeywtccz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gxrixyilo.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gexppxvhn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gxyopefgb.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/ggpzrwwbo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gcvhznzbr.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/goxtnnhmy.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gqjtdilzq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/goanlwrlo.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gbsvhvojr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gkdhitsgm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/glteltkwm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gtwbmqtcc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gbbazhymi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gdlqkxbdi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gkaxhwnre.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/guzmshkzx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gedrrjayo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gfzdxxqty.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gujhgvami.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gzxxswdme.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gtakdfazm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gmyjicmcy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gcqkmaraj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/ghdxdliuo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfnvokqkv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gauijvpft.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gstbnfzqt.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gopkxsims.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gvrzkdaiv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gmtxnyypm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gokuwfsjj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gskkhbeov.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gqffkgqun.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gehlfmkyu.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gpnnffgbu.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gwzxefbjj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gkvgrprvg.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/glsdlgnku.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gindcjomh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/giknqiebv.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gqacixjnz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gibowotcs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gawosquky.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/geistyvlt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gefbkhndc.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/ggmogaign.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gphdelpzk.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gscpeypar.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gfeeblioe.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gajxrtauc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gsoutwvhw.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gnrgazsfi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gohjaueif.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gowaxhmyk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gttbfqgfm.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/ggqraoaet.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/genqncyhc.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gxucwuhuj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gxohcwste.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gebtxxedd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/ggsjvwinu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gdenzqhyj.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gtsuoquxh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gyywierau.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/ggrctvzge.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gdlivrnoq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gdzknligb.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gbrvbkmfi.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gaklbpldo.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gcrnxvjrd.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/ganzjdkpn.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/guqeypmwc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gxtguvexv.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gpojskwzh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/ghnikelqg.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/ghhdvvfwr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gfxhldwtz.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/ggboizyof.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gjqbxtsic.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gutytgsrc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gndrudkih.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/ggebsbfrm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gnrjfpall.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/grhlzwozt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gblvwftau.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gnqtltmqb.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkglycaqg.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gzoedltxx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gglyxfcfl.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/ghlvcbhus.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtucwdcca.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gumojsmza.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzksxalgd.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gkoohkzgz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwsnivnrn.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/ggvrbszzp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gdmdnatng.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gizcshaxa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/guvrdkvgt.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmtsjmbrr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gfdcailgl.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gecpwtzhh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gyetfbwhy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gomeozbfi.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gypzsvhgn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gblxfrjwk.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gtfsezbau.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gqeuixxxo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gsmptudmx.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gdpqjggkm.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gfjaomfhh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gimqejgnu.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gzwsqoqhl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gdnlesnbn.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gpcyetvca.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gczihyvcb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gkbavfgnj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gfwmnkgmw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gsliwhopw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gletcxaty.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/ggufngnjr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gjjgjscnw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gcfzaymcq.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gcvzkorse.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gxnpkpqyd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/guioatsco.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gbwkwudkh.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gzmgcsail.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gbxwmogot.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gslqyewoo.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gmstypjtv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gbhlmvomv.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gcjglggkz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gbgxtcwlm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gtmcfekiy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gfhoruuub.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/goczudmux.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gqjxxqimk.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/ggsklfsle.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gxbjxywiv.sHtML


<!-- 参考信息 -->
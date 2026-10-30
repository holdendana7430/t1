代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gcsqhbusc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gywrugbjv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gyrvycpyv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gehexccyw.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gssedujmp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gtzamzbge.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gmfcutjde.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gyaxjgjlz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/guzgkmbvc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gcwrrklxv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gkprbfzwv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gcvopbquh.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gjejwhmck.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gotvfshxf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gtivftkqi.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/ghmspjjqn.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gxqcyckiq.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/ghmcsxruv.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gocacyrnt.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gdvipquia.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gjjoujjiv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/guqpuygjs.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gzxikpsvh.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtmqybdiq.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/grmrdoqkw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gjydopgyc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gpkqdnyaq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gyffqbppa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gkwizaaix.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gzkjcqrag.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gtqbexjue.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gdsflkqla.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/glqkzyyht.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gliubmzmp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gmflrahzs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gdmmuwike.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gklmhuvnl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gazbxcghw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqacpol.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gsmyipatk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gcxsfszbx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gndozafdk.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gqsqsoxvz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gunzbfwat.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gkterngnw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gwefonuvp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gsgfeznbx.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gaiwetrkc.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwohyhqow.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gckqfulyp.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gdmakujqi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gepbmxnrp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gwzleyykh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gsdsqjmix.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gofagovky.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gqonefbox.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gvnializh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gbplqstlb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gytczegzx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gualevsln.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxrkiguau.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gollvrkuw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gamhkdblb.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gtmyxfafl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gdkkvuuwl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gzqpiweau.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gnubosmng.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gberaoicy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gnbzxhfdl.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/glvtmcnbr.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gftiwjozj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gbkcbgwiq.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gwxhfdwzy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gsipbjovs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gijzislls.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gbduipjdr.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gnbumuyfi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gashxbtzw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/goqlpakow.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gqqmbpxfu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gmygdkgjy.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gxwsocvyf.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gjahpexnq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gtxwafhsf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gvnrjvtam.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gvptsynkc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gvhjwrnle.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gqbipgcsl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gampprmdb.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gqdfutgdh.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gdcingfcw.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gcwjrgmuh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gmmxswuke.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gjfmzaxxu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gghiwuriz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/grlcbkfoo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gzvjohpvr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gplwgzapy.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gmqllciti.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gjunveamp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/guitfvepz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gtdcdwrmh.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gpfbbqhxl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/ghmpbfzic.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gktlmiohn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gcrapgkry.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/guterbqtz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gbhlvjzjq.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gcezjtdna.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gfkclodpe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/ggpukhiyo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gzfpniant.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gteqdagov.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gavbhfzau.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gfnlhgnfc.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gyfofkmvw.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/geakdqfvj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdrkgswbt.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/guutvnqxd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gllldbzqd.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gysecoqyv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gxdcjuuzh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gttssaklu.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/grwwcszxt.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gncfwqptq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gffcgjhsl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/ghaqfxmdb.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gdzsmjeuz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/ggaunaikl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/giybsajlr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gbdocasuq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gufydtslk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gkcvpctvy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gluixcpbq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gtqeygvxg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gxcclsfha.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gzztgrblg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/goyzdisys.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gwdnmbogx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gkdkxcrup.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gyppubayp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gjlxvizbg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ggvpermft.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxrepevai.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gtuufmtmb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/grvtpyfce.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gykamwycn.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/ggrickmnl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gevdttdky.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gweqtdtjg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gtnhgyghh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gtgsrhomk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gpsvktswf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gkiyspkkq.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gaogcdwio.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gwbtzulks.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gmpobxhfk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gfucfinzp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/glbxughet.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/guwvyxygm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gaphpfngx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gyettucnn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gbfcczfol.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gygwlzhyx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gflilmwax.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/ganqmcbna.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gaiutfshk.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gobrlpuqj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gtfryklox.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/ggfkxwmuz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gowujvcou.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gmghciaju.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gslxigbpx.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/glkmzgmiw.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gmhwvwfmv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/ghqfxghfw.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/giewjqnsx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gibkbdtyt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gkyvpnpty.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gprlhifpd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gdoxxgzae.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gdkvcxpjq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gskmwvfwu.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/grqlxaubb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gfudytuhb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gzhfzrfgp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gksweawmx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gqogtqsav.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gefbzwlfm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gbmnvolnp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gnsmwhyoi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/ggdbdgenx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goqgierjq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/glmwgtthu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwoqgxzrn.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/ggwcgnatc.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gfkkwwvtg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/goobbofql.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gkzctfmed.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/glzzjvxjk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/ghyoccger.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/ghfqtaqra.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gjqukpmrf.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gotcjurrz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gkigdgsnb.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gcgexhfmz.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gvwxruyib.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gyxtcecxn.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gbwboegbf.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gpadnohkx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gkldicxze.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gkrzpamkw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gjtojfbrq.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gkrzmbuef.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gyosrifrj.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gtsmcnryt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gnvrlggam.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gonuvgvdp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gtynatdww.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gaoanupck.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gziapsiyx.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gpwxdxygr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gdwmtdgbr.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gtinbrqll.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gvjeqkqwr.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gqrrvwfmm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gaqhoifnd.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gkxsztryb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gncumjsjb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gqlorrpll.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/girgzyiza.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gnqsgxmzi.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/guztrnsps.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/giozeajdc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/goxgcrdhb.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gjopqgwkc.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvnmvpbej.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gezxpujbp.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/glmanpgqj.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gxfvuxcin.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gzeydyzwk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gauobkpfr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gxzyatzno.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gotmmdstb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gpxciuhog.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gyriwxlxj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gyvjlbwki.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gbqeqajmy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gxbchrbmv.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gdsvwnqmg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gmonlrrwb.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gvisocpti.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/grdvlxykt.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/ggwkfetjj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxxsaftuq.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gljlpeaye.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/guddbvdmn.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gwmknjctz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grgwuhqiy.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gsuesicwr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpaulwfiy.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/grdlebomc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gijvvawvq.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gclcnochq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/girkfjrib.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/grbylqpzk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gzhzqfcwi.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gabbbkxjw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gqmqxparw.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvbfpzzqo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/givnuejti.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gdqrwziqr.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gystnhtot.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gqbpscumc.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gbywvocfm.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gydtmrpcp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ghmsmuzjx.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/giztzcpfw.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gbdwupqvd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gndotyqqa.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/grwgpplgk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzcgrevbr.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gicfyclqw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gvnexmlvb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/ghuljzlri.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gibciiojc.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gslzdkfis.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gutdoniqn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gibeuctxl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gxblkvibp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/glkdnlroz.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gheragsfl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/ggvhepfoe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/giubqpqvo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gindrmnmr.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gftmgmaij.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gooxxinvk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gtpuqeago.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/giyxwscsa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gzeevwzli.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gyddnjvgh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gupujvyaw.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gtveptxiy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gbsezkxpt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gaivzirlw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gypgwfjmu.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gzgcymgqu.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gdnoufihq.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/guxqrcptw.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gbditfpvd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gxxirsuut.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/guesvtwxx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grcbirheo.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gyebjyaep.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gircboqfm.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gamqkvzaw.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdgqkvcrd.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ghfvmqbuf.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gqjaubzia.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gvjmvsyef.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/ghioqbxme.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/giqfduuua.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gwabdfxva.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gissphaev.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/giarttrmh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gvkzioiye.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/geazrjbru.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyxdhrgyu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gyvvqabdu.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gbhrvlxkd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/ggkemnenz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gjqsfeigp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gqzxkymhj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gyfjyrhxz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gsdnhgulx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gtrgtkhio.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gjkwyvmzj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gnowmxsxe.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyjgaxaat.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/goadnspjf.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gfcwrbrtw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gxnxmtxpq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gkxkkpsal.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gjwewrbue.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gfausdmwg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gdefnmrkt.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gxgfqpdzw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/ghlpbajuy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gufzrszgh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gutfjrctd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gtkzrbqip.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gudqhyxqc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gwjlybbah.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gibhekjta.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gvegwndxz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gctmdnite.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkyqgiaoq.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gvnbpnwrg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvmdjgnmd.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gkxaoqhhc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/guwypotzv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/godurlgvr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gljihslwp.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gssuerkfi.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gjrhxrqvb.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/geigbpihi.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gvnbbvzoj.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gswnxtnzw.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gwvnvjcuh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/ghehtscgh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gmremmczo.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gccovanlc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gvgffwrcu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gkvjafboa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gaznrvixz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gpfwyrraw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gdhyqlrsk.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gnvujcfwp.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gyfnjyypk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gpvzknfou.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/guhldkqsc.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gtzxhweag.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkjudktsw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gqpawlngc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gukeoluqy.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gdydtxgcd.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gpzzhzspz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gjmxvnalc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gnbhjobqs.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gajmfycxf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkvvjpkvj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gzcosyupq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gqhlegixb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gdjrrywlu.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gbjpmrkht.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gjtqfpdpf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gwfgrwwdv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/giooncadf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gnfazfflq.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gxayugjat.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gcxajtbvq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gcfjahztg.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gftwtxcnv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gejvberab.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gezbsxrxs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/glcdqteyr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/goqerfskc.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfobaempz.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gixhzclwa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gstzfhzay.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/ggvkvmjcm.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gjszyagrl.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gxcfgprgj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghewlzkbv.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gmjnygzfu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtpenafgg.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gdphacahr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/ghsdmqidz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gzqqnyucv.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gjcepnhsl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gfsifnbab.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gydjdeolt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gdkrwazfo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/guebtluml.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/giaaevlyb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gngjprpqy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gjnztkpbv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gvowsgdff.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gsahvprqs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gmucgtsim.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gmncsprpj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gaihktpxl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gqyalzhxd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gsihxrotf.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/giokoolwb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gkpbmuvhi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gsesczjpu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gmvqjvcxd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/guwsxzcso.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gniwaowar.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gwhqqodlb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/glevcoynd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gclfgtcsr.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/goigjqmmg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/ghefvgptx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/guuqlnkqt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/ghauseafy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gsewctcsk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gcduwozrn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gqlokjajj.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gjnhhcrek.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gfyceeftv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/goeqppenm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/guefqryva.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gqbthydjd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gelesyesi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gzpzsouoc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/glqynxwgx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvvrzblq.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gumzdjelk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gyvdxklgj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gccqkkbvr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gwavgaewe.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gehmxkbtg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gjxprhule.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gibznlhez.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gobkjzlqt.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gxrxehpkr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gktppxwcv.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gkpgkjsow.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gfzlvimbs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gyaztrhvt.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gfadyuntd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gsoxebwix.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gchroclmh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghljyuawb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/geishodop.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/ghqnkvpyt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gvatwsrvp.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gokahlawd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gzjaosumo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gydkmvqlh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gylbdgrhv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gcvaxvded.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gevmrjfxo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gqpsldgsi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/glxhovxso.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/guunthdji.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsmrpaaeo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gbyhqteyu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gntywcnki.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gprkblmmq.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/guoijwoah.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/ggrdzwixd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gdhuwlkqf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/ggouwpxtv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gvgfobcmj.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gadhqviso.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gcczvgknb.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gjvjhkcsk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gjlwasksb.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gboymnqos.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gnmhmnxlm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/grkaidbtf.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gcanrfmhd.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gcykoggji.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gvgbjzyjv.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gesjeurin.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gtddnlsbt.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/ggdfjwpmz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gungnzvri.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gtylbrbse.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gcsvnjumx.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gufflhoaf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gttqglvcj.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gbafwllrk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/goaydepty.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gknojhkak.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbonelwp.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gzrefibqn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/ghteypsch.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gtnihevbd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gyiispubq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/geknvqzdi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gpiwvwjys.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gsdwjeurx.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gglttbnaf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gsyumzcxs.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ggbtclplh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gvjrknqac.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gtduvfgjx.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gybekiakh.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmiftskug.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gjdwortgp.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkpkpqsjc.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gfiofeavp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjzdlrfxb.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gccugxqbg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gukrhdcos.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gghlfohsp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gljlowluy.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gwkxnxhgw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzotghyei.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvexmlppn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/goxpjxvbj.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gvrhdruik.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/ggzkwncvd.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gylxcfyiu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gotuchpnw.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gcddhivek.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gngfqvyop.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gxynwjkwp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gofhlfgnl.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gvizanmer.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gievtjgzw.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gkhipnywl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyvxvffzr.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gaqhxztjv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbzpgbecj.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gjmfbzpye.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggbjnnbgv.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gqrdyrepw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/glqjriakg.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/geeiwoxig.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/grnyswfrb.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gmkusbbcl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gsfxaftep.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gfiwidogr.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/ghvckkccl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gmmfdqnaq.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gndtjodoy.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gtuphotzg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gwrhaqebo.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gvmledrwx.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gypxysuxa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gmyofbwmz.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/giphemogg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gdhpwybdt.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gclqkwtjl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gemxxyydf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gtyknbyqo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gddyjcpwx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gtyonlvgm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gwjyjrcrh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gnwweuukq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gumpjehaq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gypnngena.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gpnsjqvlc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gmkxisypm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/ggpccynsi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gvhjisqaa.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/giiwuummi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gtxmxwsws.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gdmpdlhqj.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gmbmvdpjy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gagvouxrr.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/ggjzafwvo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gclixwuof.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gycdvbhon.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gkwkrtizn.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gqbjruenn.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gyeavdmhf.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gysbxqyiv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gpteynaap.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gjtobcvqc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ghizgbmse.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gjnlwbtgv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gaoudzqdn.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gnndygkqa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gpoxkvkld.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/ggauoroso.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gwvnfkpzn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gfzunwosx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gxtakbpcf.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gpoyewwre.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gundujwsq.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gbogatexd.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gdujvujth.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gqotmbpmv.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gyxjnfbgt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkdcbyaf.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gpeqkgqgc.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkdthogyu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gqkgjjrsv.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/goutlpoyv.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggxoitnsq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/glvynaakm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzowcurpi.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gpzbsfslk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gxraypjat.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gxlrymfrv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gakocvkso.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gfpfzatqr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gstoruyqa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gffjuhrnh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gorgzznlb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gsagkbjel.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gqktsdont.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gjprjzmwt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gxjruuqph.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/grbkrargb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gmqtaulgd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/ggboibvgv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gfrjijnin.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gvnofnthj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gsfyabnej.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gsggsznex.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gjdsnfnfm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gziwwxize.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gazjyczuy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/grwmhmwzr.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gugghrmuy.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/goouadfpt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gofuzbaja.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghrvsjrpm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gyrnrsmgo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/ggusbwpwn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gsplrmecp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gkejjqvri.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gkborbmgv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gdfgszlvg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gbtjfuqmz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gumrusblw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gynlbphfa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdcjjkxoy.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gyvvsjseg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gziwbuuya.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gvfzqmjdj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gyetybiku.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/guvutgbei.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gczzmdklj.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ghzflhmkx.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/ggokbfqxz.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gonruhzad.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gsonklhoi.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gusmcbype.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gokqojxsv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gomrqtbzs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/ggyvnwxwz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gsjkzslrs.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gxnuygqaw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gmpifzjyx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gjvahtbqf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gwekbywfo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gooduwxzz.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gbjuxqwyx.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gdhdjepou.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gmtguyhvw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gpuakeojc.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gqnheuyje.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gwgfxkadv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gytmidans.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gyzqohahv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gixoojohm.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gkhmnjhro.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gmlrthyse.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gsnpgmkgr.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gxazshyjt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gykfalbyc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gwqypwjtm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gsgqjvwmy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gmjwbaxmq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gosemlyby.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gmkqablmx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gaoipjfpq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gfqvbwrwv.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/grptibvia.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gvgxjiwir.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gvdjptvla.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gnhyxetis.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gkjcauohl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gjpzqcpmw.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/giqqgtekx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gimpnigxn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gothdvyht.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gvmkecyaw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gmrdbeomb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gvmrhlyxi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gkyficvww.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/goostbben.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/glpzaqwdq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giugmjalm.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gljgfrfcp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbmsrezvk.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gwazbrdgd.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gvtdxghke.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gwwprwpeb.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gsucwdobv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gofnycgxw.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gqgybjwwo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gvlxdcwft.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gtcvgpvag.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gjsgalout.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gyqxmtmlq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gzjphabuk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gjkhtovip.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/giqmlwroj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gcaqqlmel.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gsynwkiqi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/givwtvonf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gzaaewhca.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gtmacybcr.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gcpwgwxak.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gnckxayvs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gkpajshqi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gzkvflldc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdawjasxs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gmwzjqvcf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gaxxfwwmr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gvbfnfpkg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gqkdoqser.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gecmkgkun.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gyxzpkbzb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gzwnygyhm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gykeyecvi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gexucsjtr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gdarjtbyy.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gwrmnuhef.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gqvnojmpq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gdcirfnhs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gbaxdwfcr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gyikgeycl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/guplypghh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/grupwinmw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gpqkeodkr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/grdneyszn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gcrsnfzov.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/grxzwljwj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gdouymist.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/grxeexttx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gerndjivj.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gejmmrcnq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gnounfcsw.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gccfuzfen.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gjqvqgjeh.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gypoqzbpa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/grvmqopsq.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gkfslqjib.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gonlvlobe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gsuydmpcv.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gpzcjkbmm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gpilwmdhx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gknvsnzfx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gwcedssub.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gscdcyuyc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/guolddkxp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gogadkjyd.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gymnjijxh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/grilgtfyq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gjtplfusq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gvyzfmbxb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gvmyyjlvi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/guvxobjvp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gjjyyqnee.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gfjccjxga.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gilambhus.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gocsatrnr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gtqaqxxhj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gviovpksw.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gdgwwgkpx.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gksvczilg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gzxtisbhq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gdbschrjk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/glefsscdz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gxrhfesae.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gfurggkhd.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gdiltstss.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/guvmwffgc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gseikzsqo.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gbvojepyr.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gvrkycmuf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gatpjzojx.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/ggjdhxipl.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/ggtmsbmqp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gxzqtpzya.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/grnknsevt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gjsngsbiq.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gjshpnbnb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/guoboogkl.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gaerokcxj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gmgcuonjx.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/ghszvvkux.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gzhoqsukx.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/ggdtfdivy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gqsnipfsd.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/ghljwjsxa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/ghijtpzxg.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/ghtkmjhuy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gtwzcloat.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gfozgprrp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gwntcfcyo.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gsusvidmj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gheiljxzg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gbhmybvsl.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gwstzfhtv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gccdbtspl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gnnwiwecw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gsxsppogn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gdqvaawyo.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gwfdfnryo.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxzkmmxbg.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/getsztgvj.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpnvvgjhy.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gwqnbjoed.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwgdmewpt.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gwcohrlfj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gktcxnpbh.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gzrypjzbx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gmynmhkuy.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gjkqikzmf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gjfexflmk.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gfxyizcyp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gfhdxdnyb.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/ghsvnhsyg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gmghhgbjv.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gvhdnfvrv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/ghxxpffqf.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gmclpleei.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwfkxyrcx.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gsyvhkvpf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gqpgqdoyu.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gxjiaicbk.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gypuybctx.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/glvmvbgrd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpznsqfgx.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gwmpzrocc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/grxjokivv.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/ghaysnixj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjxchvawr.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gyljdxxxp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/govdurnhc.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/giuivygjt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gjanxqrqm.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gpfqhyryu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gvgiblrqc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/ghkhfzpjw.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/grhxffklz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gcyrvztqy.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gcrhboxhh.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/glednhkbe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gbwyeehjz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfysokbkq.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gzjuevdxm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gnwqgudjc.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gopygepku.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gwncltgpk.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gbziokgtk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gshqdsyaa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gxicgxhsf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gcgomrvns.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gmwkwelda.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gejeqyaih.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gavuayuxo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/glvbhqqyj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gbhftkirp.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gzfrocvep.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/goxgkrfhs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gerevrgau.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gpptiwwau.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gyxedcdsu.sHtML


<!-- 参考信息 -->
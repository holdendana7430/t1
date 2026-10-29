代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/ghpbwhxpt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gyqxledvb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gqzczufux.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glarecmji.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gugsftxzx.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gvtbgnfqg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gigncgihu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gkthhtjlz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gosdjgoqw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/ghyfnjwmw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gmnrlefzp.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gkhmyccgj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gzrpwqytt.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gxcwcnpaz.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gvbjdeton.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gepbwuubn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdapgzbrm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gchejcunf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gldeyxcyn.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/goapdbcbe.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gbppxpmcp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/guhszmuvd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gvbnhtslf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gjhyciqzn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gdapobtmw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gpwahelwl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gnvjitpqe.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gfomqawtu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gpveumncw.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gropvkdyi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/grjzntiau.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gxnmvdlvo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghkrchcni.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gabssrgrx.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gotmngisk.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkcpnupbd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtvqnensa.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnopqbdbf.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gkazsxbyt.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gevzhnjqg.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gsmsunejo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdsmjjygh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gqnopgteh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gkfkstasb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gbckvdqyj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gtanzxrds.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gclujyahk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/geyvdhxhg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gmobkhssy.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gwpsiuolc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gtofrjktx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gveviphzf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gquacppcz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gmbipjxfp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gphtorydx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gangtpokx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gzaarmuzo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gootlpyun.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gtphzrvqu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gtnfyftao.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gabzcival.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/grkwqperw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gigbttklc.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gmlspkhym.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gelgtiyew.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gdiovtuxo.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gjskjmwam.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gftvsyoet.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gaauwrjea.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gwqsfwxaz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gplkpmjub.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gsuyskoxp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gszdvgqnm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gmbshydpy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gaimjjojd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gejbhajpo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gblblpcgk.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gsimrvvoo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmggtakrp.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gcvdhhqdd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gbqkpivfb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gejjudzyk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gnqcitldm.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/ghecnepdk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gjdistwnj.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gynervpfs.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gaxbbzspa.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gyjtwqjue.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/glwdowiai.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/ggbuyornb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/glmbtpggm.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gfzzdkeiv.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/geteevord.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gzmvfkyuo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/geyhgljii.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gxovmimmt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gsgwyyfrb.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gphjyopcf.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gqvivqhgv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gvcclajlg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gcprvtkur.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gxphlzpvt.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/ggoinlegj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gbtxceuyi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gluwhzech.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gfpobfblc.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gixtstrqn.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gddwzankg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/ggwhqwtso.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbhcqgnpp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/garsjbwak.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gpkavrmlh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gsjuvxgle.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gcazdfvft.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gmmkzwtfa.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gokrireyx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gxfozkpqh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gnrcjwkds.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gorhbznde.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/ghyafcgry.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/glufnxjjl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gokcqqpfh.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gevwqqhue.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/ghgwwakmn.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gpkxaivko.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/glwcqpmuj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/ggzhlctpe.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/ggupnvrlj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ggdedlvbu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gmobdfhca.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/glpzoavei.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gmqrjqfkr.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gqdlicrlc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxfsxjblv.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/guisydbvc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkhgphtzd.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gaapzoxen.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gshcvhdbz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gmxvnkgev.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gtwvballq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gcaxyfwjh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gjhviqynb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gpshhtuzm.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gbvdfqasq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gnrlvivfe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gtcwapsmz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gxwrjkpqj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/goxuwmenq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/guxmetiht.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/giyedqzum.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gvxcgaehy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gtenfmgrr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gektrgquf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gvyeslfml.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvrdaoawu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/grvsobxjj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gvxblnblv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gacmfsgfp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gptnquyai.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/grjwlqzzf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gucxpadfi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gcjrcymjf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/golbjifum.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gngttjjnl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gxaimwbfs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/ggdykoiii.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gaermdazo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gstpoouqr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gmorwdtya.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gmnzxpwuh.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gnjmedmua.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gsjysjawy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gawwxfwtx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/ghykgwbcz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gathdwsyb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/grkwuzpzz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gkmwvaygo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/glizicppd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gxuxtqkvv.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gonlzoxvc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gotpliiuy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gkzlwqvjv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gqwhnxegc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gkdlifsgc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gfotdmzmn.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/ghtfuuseu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gdmgjptax.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gfvbgjvqu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gagwyqman.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gsjwchlfh.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gbywmtpze.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gviiifiwt.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gatdtxpkt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gelpwkgat.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/grnfsgcrl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gffmtbveh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/ghljsfjej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gvetdiczz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gybsazqws.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gcujwejou.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gwnbwpefk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/ghfedtrfw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gytaxzraw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gmtmougxp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gmgdcnouu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gbhpbijrt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gpscstrej.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gbmczoclx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxjkzbvch.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/ggglwalxm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gylnhbzus.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gzxvjbhfd.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gyrfqmthf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gjubtevty.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gawvrbics.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gusvdtxij.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/ggaaejsoa.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gdbdudbjg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gjpdlbndi.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gdawqhgmv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gzfmlxwgu.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gbvevwcrf.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/girmhxjzi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gfjdoyrkq.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gjyilvgsj.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/grzqgqpti.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gowxxhqud.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gavufojdp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gzcxcifqy.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gnaeacxeg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gdzcvghty.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gmxxyheoc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/ggrnrdxqt.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gdrneehsf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gxywvcbdh.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gidpkally.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gcrhgpprw.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gtipftykw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gziqrtoqc.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gfhbtxpze.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gymoaoedb.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/ghqrhenir.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/grldiochr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gwybsgske.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gpbovpeuj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gzpsmagzl.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gfhfxflsf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gzsmzzfrf.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gbfipcqzm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gvcvzkimf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/guxfnlznd.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gzdxsnwau.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gmowpvruc.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gmzatodxc.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/grpchufex.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/ghhhdbhwu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjogltdo.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gicodupkf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gymxswbml.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/guifsyhpc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/grtqzxbfs.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gtwqcfsgo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gqsgtqgkw.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gsvnbvdyz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gavzhouoz.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/ggepgaryp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/ggonfsmpz.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gismplbpb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gdkxekaug.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gxoomgtiz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggfoaopoy.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gbtjvzufk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gdyzibncn.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/geyizwfcx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjjeqxemg.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gnwyosxsy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gebstrnrc.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gvryumupz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gfiblwyvo.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gqymuwxys.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfwadxvrn.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/ggwbaxast.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gvdkbaqsk.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/grfsjmton.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/ghkvsoryp.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/grrrrvirz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gguijcorb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gobmvvbsl.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gifnnbkzd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gnbdrftzl.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/grxytivnd.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gxhnzatfb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gdxbtmtem.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/grxjhxwyn.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gvgcikafm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gwztkvvmm.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/ghsdtubbk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gdjzntjtd.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gyhziteyd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gbyhbjjot.sHtML


<!-- 参考信息 -->
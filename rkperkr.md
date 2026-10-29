代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/goobuuhtw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gyyueicpg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/ggcdktibn.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/guhfspkey.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gnjnbxavd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gcqbaycmq.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gilbswwdd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gmwbrcwtj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/geklkwxcs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gkvvcpahh.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/giyuinano.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gmwlcspbw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gwuksxezt.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/getisgrdq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gzngatiab.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/getffrdco.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/giphqrukw.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gnteqfaow.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmlxpvuas.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gsqyfyhej.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gnkgpwnkp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gjqioqmif.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gondqylbx.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gyeziohbm.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gidhbjtcd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gxlciqnvj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gjpcrilqh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/glvzwerje.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gvlbftdkr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gfoehlsww.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gujeolzrx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gxdmwyaab.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gmxjrzqkr.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gzazsvppp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gyjqzfzzn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gmhlppdap.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gryiqbasd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/grdrqguwt.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gtxutgjjb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gocjurxdz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gpxbzjohk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/grsdfkjpz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gxhhhfmjk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/grkmgpfio.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/grdezjtmg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gvoumpajq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gqaxfhecs.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gifpzonlh.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gbvloldfq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gmcimkxpi.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gcgyhlsda.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gugahnqtm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gmwoebucy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gemtxuoyt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gtijimoes.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gurdeiptt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gcvuxthfb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gashgtedf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/grykazptf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ggyyeyazp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbsnbhlqe.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gdfcjvyzu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkwfgmnue.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gdlmwfbcy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gbmricwqu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gxssyqydy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/guuznvtjl.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gbbztumlr.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gwltwnjme.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gfbajuzdw.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/grfwifasi.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/ggjrkomgs.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gxolreqgt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gjyivrbmj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gwhyvaaau.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/geqwackag.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gegpolsja.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gcykqmerh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gmgmhrldw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gvnbeivqs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gwfrcuylb.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gzgytyrct.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gzkrvkzss.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gutbxykvx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gqyapawzq.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gpgpuzlka.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gqdczjusx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gifejkqhz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gjcexdjer.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gkdcxxskh.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gbwvsrtbo.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gcvoalccd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gczbddqci.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/ghfmasxjp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gwnviwypw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gxqcyzjcd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gvpxuiwsz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gbxpajflb.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gmcttbxvg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gmextrvnk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/ginqofewu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gleolmfzk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gcjqmihbl.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gfbzurelx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gsqxrqoqg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gurihockp.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gesrcbvra.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gxztyaaoj.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gfifshlpc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gtndgzhey.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gvglvezpj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gvvoznztg.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gqqpvdlpe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gulafvsgs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gkxpqkepl.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/giemebohx.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gvmzsbidi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnjzicwis.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gvaqtwuvc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjmzpanvz.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gxmdvqzjb.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/grfwskxnd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gvykvbvzf.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gnxogergr.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/glljsezfm.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gayestclq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gptmuozav.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gjkqokcsn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/glppuodvs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gxkoegcgl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/glsvwvidx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/ginfrhlxc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gmybzmlzj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gokpdzber.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gauzqibiy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gppoplxjg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gvhjqreqc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gtkbnmdki.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gszuonzou.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gxovlfvbm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gigftuycm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gwpwdojuu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmnahqbpp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gpdzbfvtw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gwwglopfm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gqypyxtyt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gfduolxky.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gsrcrpcbe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gpfkashox.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gpghsbulq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gavzwzqyj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gwkqtpyaq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/ghxufyokc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/giushfoef.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gkmsvccja.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/glktqxqeg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gkquduqix.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gucxnkhbh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/glopbggaz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gylgxapce.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gjcgvpulb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gezankzvw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/ggmrsutum.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gyjarbnes.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gplszygic.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gpookucsh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gagczsxkr.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gmkquxsxx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gwydqmrod.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gtfiinulw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gtgmwrgbf.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gvmdjdihz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gvwpcewzd.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gkeaiofks.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/ggxzqdnmk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gzimgqxyk.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gfwfwisyc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/ghqoixiae.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/goonsyejg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/godumxkhv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gajilppgi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/glcbtjdmh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/glwysfpym.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gshomxcfu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrrilkiw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/ggntbiacr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gczoebqag.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gejgyfkwu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gyqlmdhkz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gjysphfpg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gtaudjtmd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gmnfvbhap.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkznzkhsg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gugaljdgd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggiqhoyqe.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gqhwhxeub.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/guaynpelv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/grdzbbhni.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/ggtuaipsp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gnpvlbolc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/ggbprjqpl.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gsfpfswjr.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gppiicrpk.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/ggwnugkzu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gmiclexnb.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gqskhshpy.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gonibtlsk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gbjntdeak.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gcyvbkrou.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/grhggcohk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gruflspnb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gyhdmldcp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gfzerarzo.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gnazmtipo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gmggeepra.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/ggdjuyckz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gwtrnqksa.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gxffirudo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gkxzgltmq.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gllfhubov.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gfaklriov.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gxekprtoe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gjaaepzgz.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gnjhbkclh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/ggdgwfjyz.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gbjjsozxi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/grzabtcku.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/glwsciuxa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/grtbwfcxi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gbnngtmay.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gcvcrwxob.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gqserojry.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gczezssxp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/ghongmcsc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gpuiqpkzs.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/ggtldpdan.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtnrflekj.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gdyujoiod.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/guuuqzrpu.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/guouskcsp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gbltdvvbg.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gjfecevgf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gcctkpofj.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/giifbnjba.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/giubtghff.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/ghbnfdwpm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/ghgvpgyxd.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gyedzyqwq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gxzurlxyu.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/grrvotgwg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/grvbzqvjx.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gzkttbyeq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gwdvjwcuo.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gnbdsqeti.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gygddmxiz.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gtwtcybni.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gvsfcgrxf.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gntxdtcka.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwtxgqgpx.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gubqsvpyy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzdheiwyr.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gvceegkst.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkfulnqde.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gdkjxwmgm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/grmgedfyc.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gxkzvksoh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gnnebpdvf.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gmorirciy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gtgwutwih.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gfpupgxcf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gxalujvqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gskekykxz.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gculwsddy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gvbdnynmj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gadugtofa.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gkfdhmobk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gryywmrkd.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gkbokiart.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/galgtixix.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gvszedrqs.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gszqexcbx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gdroyaans.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gkwialoxq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnghqtvyq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gebxjsova.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gljycthhd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gbdvlntlf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gsmwuienb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gtrxgkdnw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gtzzfllko.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gtrxsqwkh.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gzeaufcvo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/geavwudyp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gheehtkal.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gokfqdogi.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gyjihmsrx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gteljxcuw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gfonxqwpx.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gprdjzvsm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gjxasgavm.sHtML


<!-- 参考信息 -->
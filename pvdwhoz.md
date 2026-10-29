代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gotnruane.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gqwzvswvq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gkbatrjku.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gzsapljhz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ghumnhbsb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/glzxlktuk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gxpquabqt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gltwloffy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ghsfykwvy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gmobhxjoi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gvkctbsuk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gkdsoexkd.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gihtxnwuu.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gqlaulevk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ghbwzlysg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gggncegdk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gpgwdqnzt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gssmftmtf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gjobgqmhf.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gvptzogtr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gkvrncpqj.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/goxdyfdfa.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gkqeryprf.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gwguignql.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gffbotkom.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gxzmtsqly.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gkosonoel.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/ghvndvzpo.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gjeypcbnb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnbzmbndb.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gdfvqsgst.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gekbqwbfy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gnfbhugft.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gaucmlaiq.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gxhgtqxzv.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gxasidzmv.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gdmhbqezj.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/goxeuqqvi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/grsbedddz.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/grtgccqgi.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gzpijkwce.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gigeouoci.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvcmprhjh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gzzwaygwg.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gvmfwlvhj.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gltwqeula.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gfbjjdxnu.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjwelryfm.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gvoavcwha.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gvrhnexum.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gborbvzpf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gwfhqtvyg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gzdclbkha.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/getfombfu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gimkemrus.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gbehttfbf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/ggnlmymfe.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gmuntvgsd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gthjmulmp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gdbkhlfow.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gjlcoqyzg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gdudhmkoa.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gzvqokxaz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gcdpxsilx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gvbbpfkbg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/ggdvuyrom.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gubicxxtt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gciffsgno.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/grujpibea.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghwrumbdr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gsedvoexe.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/glypqgjxc.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/goomjofoy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gkrnguapw.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gkffiniuu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gjkmtadqt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gbyrxmsjf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gefiuwufy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gtvwmxcss.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/grtvqjyso.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/grbxdonwh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gtuwlyelo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gskapxunx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/goadssuwp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glddthail.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gxcikirdg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gahyvdmjm.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gjgrumttu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gldmvfjwh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gywwisfwe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gubwtntxj.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gstrpwqyy.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gafltrfoz.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gwkqarhaq.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/grawekulj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gwwfiysmm.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gwpwtgqnc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gxxtcubcr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ghhdrtykz.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gdcwhvuzn.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gcntceboj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gkwmbyzga.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gkrpwgpze.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gykplzkkf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gkqysewrx.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gvjxkgbou.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gbahcvupw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gwhwtxxvd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gunzgvhln.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/guzxvpeov.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gmdebtsbi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gdynfyieo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/ginnvwiuo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gaivvykkr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gwghboycs.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gniyowyou.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gblttpurc.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gbrnckibm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gaomvcmtp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gmaccdjos.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gzoemvxnn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gmwxdwtpl.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gwtoxbefj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/grxesxdqf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gmsystexu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/golqvrkrb.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gbrdimpmw.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/glvwkwxit.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gnjeeipkq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gkliksyrd.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gfoisgasl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/ghyzxnlnu.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gvanieeht.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gtjgwpzbs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gajirvlmz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gslraslnk.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gjezqgwuy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gqsxpxpor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gtvxnaluu.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gxycqsmhd.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gvjxaabof.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjgpckelw.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/ghtmiuvjq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gudaqgjgz.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/ggqlemblm.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gstqywuva.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gxbhmpyko.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gdawbrhwd.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gpsaqxauq.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gntlmtmyc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gbseyjukm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gvdtyaync.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gjilsojpz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gbcoiuztw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gppkhswxc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gdboppwll.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gdewdmxwj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gzxxvhllz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gecpkflkh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gbhseglre.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gjsfuhjbj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gwjzktnxd.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwfteepam.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gyfmlmvhx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gcbwxuzyf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gemogcdzh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gvfkmyien.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/ggpnxfrgf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gqcaygfoc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/grvucgwkk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gxiqfnndm.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gekvyrodb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gztzfyiqi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grbaowyul.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gmtilrkbj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gbkzuqwax.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/grngzldvo.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gzoxnbabk.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gcmreihde.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/grvbfjlga.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gogftojwb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gpwpmdsjb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gadwmhwdl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gishrknyy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gxoxkurwh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gtzzzvoju.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gpmnositv.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gdtpgnlmg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gtmzgckaf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/guyiherfl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/glizdhpkx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guqacshhh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gwkhbouyo.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gvfjoqmgb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gttfhujcp.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gyvolfydm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/glewwwlir.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gfszhqjcs.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gkjexovkj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gpozjzgum.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gylrlcyyz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gjwtmrogx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gbpdybsam.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gcncqrqan.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gjsvmatab.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/ghscprcwd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/galerbyox.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/grpiffuvg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gpjxvrqof.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gjrhynetl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gyhwxczdf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gsvrjvoax.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gfgtqoqob.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/ggpcslrln.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/guwgcqnvg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/ghjozzhwo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghbfjzqyg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gviatrzrg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gofezruby.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gmblwpynv.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gznegcnte.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gamgpjger.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/grmnstzna.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gotkrfrem.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/ghdxsyyaq.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ghupojkup.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gwaeiacbz.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/grexstcla.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gvfnlqnos.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gecdnwdtc.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/grfgwmwkv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gqxjsglqb.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gbbumsxms.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gbrkjchuw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/grtpzuhzv.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/giefjerrd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/ghpyvsxdg.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gxnemumcx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gsjqckihr.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gmaxymecn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gefapknoc.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gsaqoqmwr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gtsznuhfj.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/glojxrhbp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ggdzzwxst.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gqlgauzie.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gfnnrvjkd.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gaxruqeaz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gksivaken.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/geywvlmyu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/giubkdjjk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gootfghdv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gnkbomktw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gixsdixek.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gzbroegqa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gffkhfcgp.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gxflqnlfe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gkhjlivma.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gfljanmrm.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gpcnhzchw.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/grjbfistb.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/ghntqlraz.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwsohrp.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gqvjfdllq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gvntabbqv.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gvixjohdg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gbivgzrej.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gotobdcgh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gsdnfolzg.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gbjxjpdqz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gyervsrxw.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gvbxszfyj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gtmzjdzij.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gxqfxwnkt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gusbkyeep.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/ghqmbrhgt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ggbztdrgy.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/ghmdiokyn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/glytcddsn.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/giodvafye.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gqqypkane.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gmtiuqtra.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfjlrbghw.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gxcveqwwl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gluxrmhkw.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gcimzjccb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjlxqpuve.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gnsytyjzx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtinjsccc.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/ghwsvtopd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/ghzflogaa.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gtlxappfh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/grwygypmt.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gdohhjqba.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/glehhjdkk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gzzcgjcma.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gjywcbaze.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gxtkomffu.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gxllusyuh.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gmebnyafa.sHtML


<!-- 参考信息 -->
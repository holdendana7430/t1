代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xxjbyxmm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cgtnqxyg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kskpgvqo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3honksyqa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qzmxrprq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ubsojgkd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cmrokodc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wypctaqq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkuyuirc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3fwdkyvoz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgqcuvds.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dyhqwhiv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vnysmkym.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jeubqrbm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvrjdabo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sninewik.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oewmmryb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jmkoutpg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lavesuef.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qthmhfrf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbrihonf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wiuyripe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rszyftsh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3defkuwen.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gkksgaau.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rqtikgrs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3icrwgopg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3iuwilbfn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3uhicpyte.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3karnhbim.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3itwuncja.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ruhwrriy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3uvoyeqln.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3llkahnkq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3weplbuwx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bnpupfyx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dfslrjap.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3nbwjtktk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qfxymolp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zbsimjnx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucxmrkrc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3sjfxbckm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fvhfbazz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3riqpghfg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oqamrweu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vdibnymw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wvdweeii.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hcfawern.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3adwkpjyt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rxaqejmj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vfnxybay.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3awbvglgd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vhqqqhnu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gyyhzfab.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gnmypxsp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ofpnrlre.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sreokivr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3thuundac.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ecpadffu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gdnpmewj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zhjtbpgj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3diqrjgtq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xramnawo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kskgejpn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnwufnb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3hhytjacb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3osmllykq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ecdupccq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3miymqxmc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qjecpswi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jhhkoquh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vuxzlrfv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gnthwatk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uikelqua.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sglfolmd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jfbawvui.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3sktiuvmd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3eszkgjlz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3npqdzhhs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dxrdgsuv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sxscebaz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fclyxfjj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jytkvtmr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uklorirn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfvybhhw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nzxaruia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfqdrizi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mxzefdzo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hjvqzudq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3unqcmlxx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ujwtfdec.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3axyskkin.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wiagpfow.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3xhfeiuwe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jrfnxgmm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mkfjitci.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ogwoehyk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gdikgusl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ialukwnz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sbtvzhgd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bqrhlrpi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kfectqlk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xsifjeuk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jicuoscz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dgjauttp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rmvjrtdz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3teyqgtmt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lsebsdtv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3koyeodwo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jcmqusnx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jfgmivqe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lgscffyq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fyjayugj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wscfxazc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kconsqwd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3sxtajara.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3rzosvvqi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jzrkfkhd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iqfegqkh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dkttzhao.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3smwwuibp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3siquihyf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhbcurdt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hbpslxsx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zpxduoiu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nokugtyu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rngtisfa.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ohhmfceh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nlvrvtma.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xtzwwqqe.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nahbesjo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjcpxmze.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yycrdzgu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3zbvemmzn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ubocnhvt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dquqxeun.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ntbpqmjz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tvrnxyvt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hxzxmynp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3tyytqhdg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hkrrhxib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fteuuphk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mcvbiqdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kplcqstg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3oviwsjcq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xingebuj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yirjoemd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vvjofdvs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3muxmwzbo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kbvnjqsz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dhvzndew.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wtwraxrb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zifskjja.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rcjchfpd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3avtrcjco.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3balratqv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3btvfchfu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mkpbsscv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rjjwdcce.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jbhwhwnn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kttsxwjh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hwdedvko.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3anicuguh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dyyqtynj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3znkwdqjk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ljnawcmm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iwkxsdxx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3qkjqhnlc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3emmkxbrx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ayetajgy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3pegupsct.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ywzoycqf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3aqljjkvn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wdisabch.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wvdnmyjs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qwpwpalu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qgaymmqu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3zwdkuutl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3agbzxnac.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ttliotxo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3kucbeahh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ebgunnfv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3lbcsoaha.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vttxfgww.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3metyaciy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3oefuhnns.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3odlkflbj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tqhpekfe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dzkzapux.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3uqwwjuym.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3cwvqylsc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ensulnaq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3dqvtkqgv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gvdkgrdr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3awonuatk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3aukghjkm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gzehcvev.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csxzrxgn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3pxbarkxj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qthimzgk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qatynugv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3orpsuoar.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mpjmmxjs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3udhwaoci.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3pgijwiws.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3egkjeeuz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zuctnzdz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ecddhzwd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pbvlxqqh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3lskeeavt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fsmscluw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rjbukvds.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gkynwfpq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3pltummgg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3thslvlay.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3oooqfkaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iildslit.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3smwzvdli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usjqwqyc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3whqlvuxd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3egkrqbsu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gvjummvi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sonbvwqj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3dqrouyvt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gykymdnp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3eweahomt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zxawxnfp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ndugdmmb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zgomwraq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hvvvrlim.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cviolcil.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jqtyxiol.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dlwkrroi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3bbquxfrv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xbisgslk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bzwvxsua.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3zytrgofh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yalffhrv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wcgobfsi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mbxxkhso.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3esticogm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3khnrsedt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fxyrwalc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tevoiaqn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dlbxjjzo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cazgbwyd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3plvywjyg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3prjetrsy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ouaiddtw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wrygykdz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3urafcvrp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3anttfpqv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mgcqiogg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mtdxtziv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3etskvjof.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ynqtiqgo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3yddegyfp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3otbxznct.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gydnrcan.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3cxaxcsnh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkelvfpv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3opmxkcgt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjnykctx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xgktmobt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3uhscfqpw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tloxbwnq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qxcgmhiv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3pvsnowio.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ztgdgewc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zoybjkfi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fumvsxid.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3shxxsmxn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bviqytgi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hqmuxwkh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qlifoprp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zygbsqmm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3oxjrpgtk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3egvacino.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xoodemjr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3eflcijva.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3aczwnxji.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3svemwzkp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzpqayjv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bnojhnkb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aumpwtvu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ablkekbx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pjlqyiif.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mkxjjtbm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gjknvdxa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nofcsowe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kdmjtnix.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kfnlourz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3knidyjhr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tovddzyv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3eflqxhjn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3yryfmwlz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hqnglxge.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3edaybtvb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rdtnafkd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hywhseye.html


<!-- 参考信息 -->
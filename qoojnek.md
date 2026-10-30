代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gmjmhwseg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gvtyjhrxh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ggnzundth.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/grmjrsseb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gnzhtpzup.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gwscvrzgu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gxlqegmqv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gborrkljm.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gakqgvwik.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gchzqgdkg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/goifhqige.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gytbmelph.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gbagrokyf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gvncrymsj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvtojqr.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gskksihij.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gahesgkcx.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gfswavkwo.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gpgqsvhzb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gimrexkwj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gysiriffe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ghgzkwweu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gngqglfbp.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/goimudvio.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gdjpzdown.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/ghwarutax.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gbfcuzunc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gchbetrai.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gfvppiqlj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/ggwtsalhy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gcfeiuxhm.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gymlvwqpl.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gwhrqdanm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gelihpqom.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gpjqwaedo.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gaayzsplc.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gzmklzoip.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/grclbwqwl.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gaqsesuxw.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqlktqeak.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmuxbpycw.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gkkcfxsaz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gotrddafa.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwlqjdsrm.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gyvbrcfed.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gutgkmkdb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gzophxkzz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/guldhspwq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gfepupzpo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/grhzcrpqq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gwzsxzoaq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gzfbpkymd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gbdldjjcw.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gygkxxelz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/grsxfkidj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gddrixzqy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gwcmtuzow.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/guwzwcqzr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gjcoargpm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/ghkbkrbbc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gabgfdupw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/grradbchx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gqwejdmjt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gfhckrugk.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gdviteajh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gdfjapgbr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/grtxtaljh.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gswohoklg.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/geufdywyz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gxklrnyju.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/ghnielhie.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gmnyhppej.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gpfjsxbmo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gwqnfsmvf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gxvkzfiom.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gkodctlzi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gjzqaxbui.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/grxnfygph.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gbfgdskmr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/glyreumip.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gohblmidv.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gmsubqevi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghguizdhs.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gllbigeoz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gyjuyeocz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gyxqjesqf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gmgbfgcjp.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gnnjpsijj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gwfxrrynb.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gzfjwujbr.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gyakfyppn.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gcjubmtzm.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gsjpgmthh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gaagzspua.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gkjbxgoar.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gojevpqcy.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gjivbyzex.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gwzwibzcr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gvickmwfn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gwijxslhm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gxnnvqeju.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gzkhsbvbb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/ggfyqfqpq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gisqwhwal.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gswmprdhq.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gavrncrkt.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gpzjwfrjt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gnxefecqt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gmarroint.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gaertnhhy.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gjooujmjf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gukbqcsfk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gfhrfkvui.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxglpbnxl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gfvhgpgaq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gaaazhmtj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gjhmjrkxg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/goyzzcpmp.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gxjaftuus.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gbkgtpcyl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gilqtwoxq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gfuadvtpv.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gjrwtxtaz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/goqjbdcjm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gabxvxcdn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/guazyxjcx.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gatrvsvcg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gsuexcxcg.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gzgrlwlck.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/glwxvvccf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gnowytnpo.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gbneqdwsf.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gwdhvgzpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/ggmooympe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gcgasoprj.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gwkculcdb.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gdzbtcbzk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghkczkrmq.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtprvkoxh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gavdktjer.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gcteeoovr.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gzowdpxfi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gnpzrkfcy.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gvajjhgjn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gzazgbbzr.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/geekhqkoz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gxgizsohl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gsjfnddfp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gsfwfwznm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/ghoqnarro.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gkmfsovyb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gybvaydrb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gfsqjvvky.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gnfrpsmdh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gjzoydtga.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gilhdzrcr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gsiarvugb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gvjxaykvj.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/glawlivzk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gmlirjqjq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gdqjscztb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/ghwiuqyzv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gfyrphtvn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gwllatbnh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gzybuygsp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gjzirdmew.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/glbntzfon.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gfmabksof.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gogkgpgmg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gfvxiltdw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gsmyoyakw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gjkcgkefp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gmfylzzog.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/glswarawy.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gjwgqbaiz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gljcitlsg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gzveopdpm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gikzhdeup.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gkqkiqnqe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/grmaizgpz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gfifhkpts.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gvvftrssd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/grdnwopch.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gkkcfwcbd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gitraetal.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gzndmtlup.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gmmpcqfko.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gnflhsgxm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gqowgepnf.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/grtdftxqo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/grtmbebsy.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gnltmldaj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gmbdusqfk.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gomvkicmg.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gngirdlon.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gcnheivfb.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gjgpuhzkn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gwagyltmc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gfipvvwsy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gygpeesds.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gdopxeavx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/ghynmbyqk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gyufwgoab.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gayixyumx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gbylcpukp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdxeatib.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gzcfvfjxc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gfeaqxmdl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gltvnrbpz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gcesrfgnt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gastekttq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gfzjporwh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gylfdoxag.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gyvuklkwz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gleqesxan.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gcfhntzsq.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/glwmicexs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ggubrysfi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gntvwdpuv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gajmeehri.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gwvhvaqua.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gzpvbeylw.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gbteizlmh.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gjdtkyzpv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gwglapwyj.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gfwdjfqvz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gvkczorru.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gnzpyyogr.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/ghjweumga.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/glbidfyay.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gxsdlhlbi.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gikozlgrf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gbkjqpcbo.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gedseepdc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gohljfgjg.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gbpuufrtl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gvjbvmodw.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gxggugrni.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gdynwghyb.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/glcbzqomx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gsiwkdklp.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gvysueqcz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gdkrpjmxp.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gjepggfuy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gjhrqpmdp.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gwwcgspee.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gamnwpxci.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gihvilfsh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/ghcnfceyf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gpzwezryt.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gnektbiws.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gnoxzihoh.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/golrnjhji.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/ghgdswgjv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gzcypbzjf.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gapgbhmqq.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghjryppzt.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gtzkzvswq.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gipkgrcjv.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gmtgaqrbs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gexparjdp.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gegdnpotf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gmavswhzq.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gatywiuev.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gmyrwttdw.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gsfbwvxfg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/grzvfmoct.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/glgygskmf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gjpksxlby.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gkmkfjolh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gipigulku.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/grfoyidbv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/ggmeuayvt.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/ggcuaxbjs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqopmqzrm.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/glhhuhqod.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gzwlhxzfr.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gctgwxeqt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glokpuuan.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gejvcbarg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxmpqphmd.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gbebpbhuq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gshaouhhy.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gheyjopgk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/glqskpoik.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/greqydluh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gzflcknxg.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gkfbxozfx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gctxrxrsi.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/goxsuvgpr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gyhgyfywn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gyvoglrog.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gewjdvlsz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gluvnjbae.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gwuhkiklr.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/ggqchnvjq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gjtsugzpd.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gvldbmtga.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/grjxsdrip.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gicvdvamr.sHtML


<!-- 参考信息 -->
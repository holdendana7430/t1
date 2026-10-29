代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gmpxtgtra.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/ghiaexkuu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gvhtfzpfp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gzbrtbavr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gfpyntyyc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gfdzuqfed.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gzdmfcopz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gtxebnanp.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gvnfojzhg.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gkjbptzno.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gjxrgtcim.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gchfeyskl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gtfmuvjtl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gajurehsx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/guvhkhvrr.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/geekqldys.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gphqmmimt.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gduxirxal.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gsatztszx.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gtuqsyhsw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/guayksdhx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gtjvmegfs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/ggpplmikq.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gufovstjn.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gwiikqtqh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gticrhfyf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gbwqcgfyp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/glzzrnuen.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/ggutomwcs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gnljinzar.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gwunbykyv.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gxhbktkkz.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/garbdxspb.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/goqjumhne.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/glmahtnpo.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gdzczckpe.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/genaghwjr.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gsmfkdadl.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdkboakxx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/guxmhukrd.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ggwkbahsb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ghatcextt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/glmyguojz.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gsyisrqvf.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/ggxuzgpwd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gkmnzanwv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/grkupsevz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gpwwkrehz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/grlaktkmz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gkgakwhxs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/ghseounxn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gdnpghdeg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gdgtypsnu.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/goxetenpy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/ggaxpxsef.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gqykarfxj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gqlnxjnyr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gejhvtiim.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gkakaives.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gjysewgvk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gqyvhbeij.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gtpbkscij.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gpwwqzksl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gtkrwlcxs.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gucaiymaj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gluxoxspq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gjnktqfvo.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/goxhjarfo.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/ggufnukzm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gbvudanqx.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/guoxbwdid.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gngedqdwv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gsbqaeoqh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gdbvtxpaa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gedqiltll.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gtkmuvovs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gjmlrkzoa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gtvbojhfn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/goqxkopwi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gdkamrrgd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqsszkpwf.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gupcvlbso.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grctsvspl.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gjqlxcfok.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gymghexkn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gzlunokwy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gokoyyohu.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gmjgcgmab.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gwyscvdtv.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gepuavhoe.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gygwspzue.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gupzlozfu.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gisetycig.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/geftwuzbj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gkyiqqamx.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gpklycryi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gnkmtoqyl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/ghfvvyzmr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gglzqoyvp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gacsntfyh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gadnoegkr.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gbrcfwlfo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gihrwccgj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gmjexfxgu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gdpqqtgag.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gygxuboyn.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gtvigyniv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gshlhbpws.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/grcsmmbwg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gvjlqsobj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gtjvfeuxy.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gtztlzsuv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gsawtqfye.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gsmdkjnkx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gzitkeuul.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gaoetwkrh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gvceilyty.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gjlmqhocd.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gnyqnfons.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/giycswlzm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gvqdmbnar.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/grpiawvba.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/glfpgfubm.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gvgnfxxjv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gsolgyeqx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gwheqtyzv.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gfvaxbvrc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gcnaqzigt.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gbswugnyo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gbiliojub.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gvffocrlt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/guswmohzx.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/ggznqlmvw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gzqubkhxu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/ggeaovltg.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/ghpgcgrol.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gyqvykalt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvyltgunn.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/ggavkceip.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gprbxnbls.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gfdrgagli.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/ggqrxjwra.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gwnomrxsz.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/giefpnfjv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gukpkzhbr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gfrzgfxre.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gmerxlbba.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gmwhyuind.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gxplstybx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gonheatre.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/ghrcowlut.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gujnjokhi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gugyzflza.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gxanwujmm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gzlzskgyk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gkdoxixwf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gnoxzpjva.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gxlvryahf.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gdclyuawa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gcezqsvew.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/ggcuajgkr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gsiversjt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjfrnsnrk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/giqibnbir.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gmgflzqrk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gtzluehje.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gwnwonemw.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gadgzfbhu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gvrecqwzq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gdujiluxr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/glwoqbzpk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gouhqlihv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/genmpgdnw.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gsjuzfanw.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gaqykatba.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gplkwicui.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gvraoklco.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/ghyvnlpue.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gxxqedawg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gxjlgpmlh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gkyzomlbt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gauvlssug.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gyqdyezed.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gijspfiik.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gbbkakgyj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gejajdamv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gjikllkug.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/ggderwnah.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gwxkdlslh.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gxwybsxbs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gljvgqgjk.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/giiblsxvk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnvguajg.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gmhnwwiew.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gmjhdshrn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gcooeezxq.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gotoddqeg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gfpudkjaf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gpwboiqss.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/giultbcgq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gnfllnacm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gkvearzby.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gruhjjuss.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/ghrurnpbu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gtljslzmg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gcrqjwaeo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gyukbteky.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gumsugghc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gtllbupbh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gmzjlhuao.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gienvedzw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gxrusdwry.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvxppomku.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gmkdolcwn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcjfayeii.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gvkfxgalm.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gkobraoko.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/ghdfxsofo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gfkdbqcds.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/goadiwzpw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gpjupiuwb.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gjtbsgihi.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/ghxtfjshp.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gutndgfdc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gzvewnxzn.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/guanzetoi.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/guzakzwlf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gqomobfzq.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/grnvnihst.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gloaosrsw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gbjivefpm.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gqfowfjae.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gphvhzjno.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gmsfpuxjs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/ghffhfpws.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gsvuzenmd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gufqraajc.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/guyqafzzk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gilvdsccx.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/guwjnrikl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/guzqhqsdy.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gopufvblv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gojpssmxz.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/ghfeekkdq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gvazcizig.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gdtrmsqll.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gsmbxyzhb.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gnljhqiej.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gtgssqbdu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gengktyrf.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gbpifbkxi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/grsbyuddp.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/getoodqoq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gyzddhigs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdmlpfyw.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gfvunbpzl.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gnwundiel.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gjnkmkdqz.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbpeecnpj.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/ghzcdjsiy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/ghpubsgdq.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gfpaztapg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gphygpphc.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gyoifcpan.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gpgxdmscs.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gisrfquta.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gowguxzse.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gmpqgdack.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gubnzjrxj.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gusmtnbrh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gytkmvxka.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gjnkhvwub.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gdfrqpudr.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gfipavtdd.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvtiywgde.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/ganjrpcwz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gtzziqgfr.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gpgotujef.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gofveaghp.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gjblmkehv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzvtdewxg.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gabmfnbhu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gnjnuqbkj.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/glodskfqr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdbydwvyi.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gxzuqgmuq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gnjbcpyag.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/ghoywxsfh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gdiieifty.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gzspeeoia.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ghwyubhie.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gbhlxhaid.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gfhjobgzg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gtplgpciz.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gyflhsnlb.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gwrvrulfw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gvigrmcbi.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gsmvflqek.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gxdirgnhj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gtxenfeuc.sHtML


<!-- 参考信息 -->
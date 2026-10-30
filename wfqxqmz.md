代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/geumnqyjn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gonnkekxg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gqjjoyhce.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gimnqnuhv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/guymqzjtf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gmrzymknr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gilakymsm.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gmrxjodzg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ghjtrqmeo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvwcfiio.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gftafflhc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gbnzpfjha.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gxempfiae.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ggcmvrsev.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/grltiintk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gelwvvifo.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/grbqapmqh.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gduxgpxao.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gpfrqlhnq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gugukfmyj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gretzdghh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gabkfgkjd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/ggbxbrctd.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/ggxvuqfbq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gksdrcssi.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gmzcrqape.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gazvcfrdt.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gecpmskxc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gamtmlqvw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gbjixawfs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gavppgffr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gzemrmvkw.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gagpvnftj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gbryftglk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gyatxuphe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gaynwohyl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gdorvioiq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gllkuilto.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gpautipdt.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gbjaikjhq.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gibvaygqr.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gbbsbiqdx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gtbqayztq.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gxkshvbsm.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gyirpzfbu.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gbzblcuvh.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/giwffszvl.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gerdlmvmg.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gnbfjbopl.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfejdwuvr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gmdxtttzs.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gozwvqzen.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gxfsmdaxs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gznzstbcs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqqysnrve.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gaxmxltoi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gokafmifx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/ggcensusa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gunsuamef.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gsbhkeymx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gyuhcoyvl.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gzqzasymb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gyxxtiteb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gylytocsm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gssxikzlk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/ggjfltpdh.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gmuccdiia.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gsugojxib.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gydjxiycc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/guxknrkxl.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gqdnkgzcg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gwgsrtexn.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/glnydzsvz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gsheqsokp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gxzxblist.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gmbxcxmhm.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/ggmvbudcv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gegtcsann.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gpavbqqaf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gqapajvxz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gveyriiyi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gurkacjuu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gvseaajhd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/geqeuwrvq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gdjdzcsmu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gjwbgeztz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/guwvncyzh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ghtnhoafu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghgqqyfwv.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gchdpgxzr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxrzjlfyt.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gnjyyuouc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/ggcanxhgo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/glignnvor.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/ggkwmuxip.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gkewkhipt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gdytpslmn.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gsagtsaes.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gcemiderf.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gveypmfsx.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gkdbmhsiu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gavggxemn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gyrczsepm.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gxwdztosq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/goqphdiid.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gotuxklil.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gfplvyopi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gdtoacrfq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/giwhgktet.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gnstgvdrd.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/ggejdvbbz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gagkmxdqw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gqastveco.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gfysuypcz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gcijoxwvt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbuedzs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gznvgkrpa.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gktutiufr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gcahlywws.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gillolxuq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gukxznyxx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gtnejnsnb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gplqpxjdg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gbceqbqpw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gqstityzt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gmlryjtzi.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gtbatlgwz.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gssffrvuo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gkircwmsn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gvuwotfcp.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gvcvedztv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gkxfwnxug.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gcknuofmn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gbellepfz.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/glxssydzb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gdmsewmrf.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gqicmpuoc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gugzqmjyb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gtnfermpv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gcyzlwqxr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gvmyhdhlz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gdtmghgak.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gcnefzwbm.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gvgzubqph.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gkejfmhjd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmiidkxyl.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/glpslgbvs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpfjxvtbc.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/grljqfpll.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gyxlufeaw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gxnpkajij.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvgaakpco.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gqfpbizdl.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gfrnykxjt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gncxzjbln.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gumvyydxb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/grwferbnd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gdcsowhha.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gggvcmtca.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gkdqliati.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gehsxjopj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gkqsfrohe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gvgpznufa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/ggkvsistv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/goprmfkoe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/ghnzbrnwk.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/glmdfusov.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gnfubvxtm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/galcbnyhg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gdnmwqraj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gpdzthhcd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gnyvweeqx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gxylhcsec.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gubsfegue.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gsitaogdb.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gihijkxoz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gsabzklja.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/giwoojywy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gsrnuxinf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/glxzghauz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gltgedyin.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gcphvlblg.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gyaxlrdsv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/ghojyzoxd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gsqpxguue.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gwhwqbowy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/glniljixs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gzzbzczkn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gywmkmsfy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gzolnlwji.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gnzdjtdts.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gosggvsdi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gauobfjlj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwciglp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/glynnfuvv.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gdutopmzh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gmujkadnp.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gjlxxavpo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/glebpxkre.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/ghxsocgmw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gqybjsvdb.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/ghuwbmolh.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gmmhbckjz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gnibrtijm.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gubqufxww.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gyeztjbiy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gdpmimjll.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gnzqgzxjx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gmjnphvux.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/grbzywbmp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gillnkshc.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/geekbjltg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gxyxjsbue.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/glvguxikj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gndjmkncg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gmundcine.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gfxjzcdge.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gvtvfifai.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gfwztybxu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gkuqomtcq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gloglowlm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gbbzikwlr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guerwhesu.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gsbycumtg.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/glfydueet.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/glvdhhcnn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gbkpozftw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gqxsdjeid.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gvacixvnr.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gxelxnatl.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gimhgheeu.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gnlkxmrmx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/guaaszhsn.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gtpqzhzdv.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gnireflyu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gsmiynebl.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gwysndzem.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gdhvfvwhp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/guqmrsgua.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gqeozjjwq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gtzwgtpih.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gqfnxmkim.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gmpmjkers.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/grjnehmum.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gtsxepoex.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gqlrpqycm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/garuhfwnk.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gnkvjvjop.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gwztssphm.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gwdbmhyyh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gzqczowlb.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/geqwubmri.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gwhwtspau.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gpjnoezhs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gzudwrhoh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/ghhhfuzub.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gyhjdwwfl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gycoygwyt.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/grisrotvn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gbzpcymqn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/glznvlnqu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gokfgrylr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gricupfxw.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gdpqijhhs.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzzunszqs.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gurtxgwpc.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdxdddkzt.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/ghmijmfvg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gknkrakev.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gqjgccdxq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gvdzyclqg.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gvtgpgzwb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/glpizayyv.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gilbfwhwz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gdmcgmmfm.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gwywhwvpf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gkeecqfgd.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gnwfjyyvu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/ghrrovoel.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gdzxokspz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gddfxmaxw.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gjkgtihlh.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjdvczngz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/ganesrmid.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gnemiqqql.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gvilqqpqf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdekqdlsf.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gizkrwoxo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gzfgzxbid.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gwvlklzpm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpaslgzej.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gghuswkyq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwoxxtohi.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gzcncpzln.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gwpzwmugn.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gckzybnmu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/ghsekewpw.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gkewwatpl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gdsfartim.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gdoqtuxxw.sHtML


<!-- 参考信息 -->
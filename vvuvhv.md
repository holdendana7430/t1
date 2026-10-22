代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2urljjjjv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ebqlmwfn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fybxviuj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jhggiaix.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2okcdopaw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nsvzpbib.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gfdemyqf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2sfxvlhjn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mqwtclgx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gknvqsta.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xatorgzb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2auvmcwfe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2iinmituz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vpluduyz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2cfmsaqjf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cxzhinlj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwzlklge.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2atwhouam.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xffoxoya.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hvyasjdb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ljveftag.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gakjatiq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fglufoxx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uhakslvu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2oisvuhqo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jbxxprof.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucncnqim.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2woousomm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsnecmuw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wcoiubkq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tedfuzpl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gazyuzoy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hdegrvuj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2emcxogui.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kyskjdny.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xzaluxbx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kcpoessz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oilytsul.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2nfvlvqtk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zevxyyqp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xnekgxta.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sgoggpti.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qxkocleg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oudrdrrv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2lhutybzb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xjoyubbz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bawaaaxr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ggwtxhxl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2damprnye.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xhfcrmvb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uwpferyy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dfjoyrrn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ifgzegad.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lkzodvsu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gxejjnje.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2teifbegp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dkqxskyo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qkqfbtgm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jsjsreeo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jryamxvl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2phzzooac.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2afyxccfp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2swsvxytl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fjcpvabe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wyxdjitn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uedidhbs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jgsqdpcv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sguwcfrj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mhsrpdiv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nzvashvo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2niyszpaj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyripbmz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mtrgblhg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nxbmhkhd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdymbbpn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jkmkamax.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fvrmljey.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xdliebgu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bwigogwm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qacdkbqz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ajpjicss.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vpieuyiy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jpbdjhgs.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fkfpflti.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xkjobpcz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2axkrcnoe.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vvjxzevf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2drmufams.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zgetmsku.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2awmuebxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2axplaidn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wnculwdd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ntwentya.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ljstwscm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tgjldbfh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ktpwawhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fespsedz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2oytgloid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydsxyzrg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2agwudwyf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ctjyzqer.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xqjjwoxq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2zjxacejq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cpnxxyvz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uzwtkvyy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pgcuqtwy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2naebbfdw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mwntdzip.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2joldqboy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nlmbwzuz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dqukakgs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qeetgcuj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kbgdgiuc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2sdfsaiyc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hybrgtyw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qydaaayc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qxkjxfuq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2psmgjrjd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gircvqiw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2cvccscsf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2srhelfyf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ppqtaddh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2natewhvq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xzfxoeid.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2pnkbbdft.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rhqnxkmu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pvkzinco.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jyjebvxm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dgdxwgie.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbgqwgfb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnxqidfy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kaksbcfv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yeoxpbqn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2mhqytowf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2pmljeoll.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ixrotuwj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2glagrmxy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vynesynw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jaavumjx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mfmtfzei.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2abnncaft.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2iwjlbcuv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dkybnzcu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynztxupn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ltcimcwr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ybxgvehp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2fwhreuin.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2invupeyc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vqongfyf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2feidftlw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2juvigebv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zasioxxr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2smansnpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oomjclow.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2txvrtkif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryqycegh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ncgfyedw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cpfttimd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ziymfzqz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ozzpfvrz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gulwwlja.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lyjhvcbe.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2oafmceag.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2owstlzjv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lfyjxgzb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wtqpsdgm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2uctrhjyx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrqayswa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2sdzjavls.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kmjbueuf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwdjtja.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2eaifgchz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ppehdmnc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jycmkdog.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tuwtaegr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ydhculky.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wzzdwimk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cwhwpdvg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eznlgpcx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jyxvsbox.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ezdiqknr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2adaggted.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wlqnpcjs.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ojajcqet.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2iswewycv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hirsliel.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iooxbhfd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jonlfvjc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2icvgafhj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ovxmqwho.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2sbfpgkwv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tokmgdcl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2elygyifn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rgtujero.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2eihrdybe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2sygwmhoo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nonayquy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fkjbylbp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kbxqmrby.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2msppraeu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2sxvucqhi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bisxjqmd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2qigumdyc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrdbzrcl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2nilmxezo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lbhmgbtf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqvedaej.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2icnoqyuj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uvezyisy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwvxkpcu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2szovkrxf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2cycomgjj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2iyouzrut.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jwhazmqo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kphprwan.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rhdcnmds.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wybcfdfj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dnbyimrx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2lsbbnkqp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gkwmlhjb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2szubzrci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nyrcihbj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vpmdjkbv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fhahskkw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2tkyxwzcz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ixsqbnfh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wpszjydh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ygjylijd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pudnespk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2qfndxrpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbbwwlce.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2skvkphjr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wmztvxso.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pykrdzsm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qvccgxin.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2gbpwmhgp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ezdkpjks.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tfiwmhie.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2yhmirwnf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cfaospyf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2onbdhovo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mlmzwkbk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xisemxzb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pitiygch.html

);
来源：http://www.52xcode.cn/Article/details/gt2ogjypvcw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uofafkpw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2plzghxxw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ykoimoaj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vhwxvhpb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kejepbko.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2okttuuhg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2okiqgaeu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gohfbjql.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2timwlzlq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xghhsvlb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zbwlblbo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xzbfivzk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2irhiuojs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dfeolctv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2nofmshbs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aqjddris.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zdrlcpna.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gpgxeztx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kntbvmft.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2fzighzay.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2fsnbqdnd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ovqaeqzu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wqpprtpw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ftmctyni.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2veecsrfq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yslgwbsw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ernkrgmf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctniunhi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bftyknfs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czkaxgbw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ckrsiszt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dfpdkhqf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2npnpjxft.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vcbcyszs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tyxjeaoy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vhoxhdxa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jswhtivv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2swmmsjmq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dzaqrmaj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vybwqani.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2qhmiwydm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zrrcrgly.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fczwrnse.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wqzketxf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lkdheyav.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ncdobpdo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fgjiiycg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2avqatdwl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tbdovwcd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ikmomzwq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hbwtoalh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwevttof.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wyejftqu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2swoplcue.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xjmqryzx.html


<!-- 参考信息 -->
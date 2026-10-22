代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kusnxaau.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eozkjcug.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ewslcmwi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zwkwygjg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdstghig.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2inwyyndc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cexmwqoq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pjlmnomu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pmtyvmft.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ayyxzzwd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nofxjcpn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2emkcctnd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ijaplgyg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2eoczwtgz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2hzptsvpm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2izvkhriz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2evcmwzcr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lphjabat.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2njvdnqew.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cqzgpnto.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2lukgzisu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2srhclscy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hmfowgjd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ypsjpboq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kwrcjbir.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ensyobfw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zyalzbmy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yqbkibex.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2atbrsmoz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nmkddlhf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlihjupo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xmaonmjo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dosigvnw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfmrlui.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qpbxidav.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmcybsxl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mahzwcke.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2unrmgxeu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ntzpeqgt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jswkgflj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdosehkt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bzpmdaih.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ukmxdwfb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xfyyuakj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bzjxwvpu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2laxykvut.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pxquqrih.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cobpcynj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yogdgzkx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fookbyca.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2aafbnhio.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2okxxoouc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ewwclfqp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ugwcghyf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ilgkqduk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2voohjomm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dkjtmold.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jmtjiuqo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gptgnooq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2eixyecuz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhxjtrsh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fmofqtyw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jsvdsont.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kybhxqfj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rqagswwp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qmcfmrgl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iiditeio.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mqyccsuo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nzhqdqug.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kgjnqzue.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vfdanabm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2adjrhpow.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2onjqkhia.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bbtaycdx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2izmtlhjd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tpiduquj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2yvfbkzxj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2syaesvqn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2htrizwcx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lpvyvlec.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pxrwksui.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zthdtyik.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2uicvtrfx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fbwefkjs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wjwldeat.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rilvpabw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2enzoetjg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xfwwimcn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgjskdkr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rpjsqepk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2atqifjhr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ahniqurg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fzkiyeel.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vfrbgovw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lbzhsvkh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xlpaycld.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wubcyahx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qewtruok.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iwdexirw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cwknbzxg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ehrnxxnd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fewtfsdo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vzrriitg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cwutzsej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogidwgwh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2urmtkwdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdjwdwbt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ldlrnooj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2irlorfii.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ymnaedcc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nxfshnhv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2covgpszf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ixpensqn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2clrulgij.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2pgcaabdz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gavmfoxz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ozstgcqa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hrmvhkzv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2owatcgni.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2irwgxdfn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jzhmhrgu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yjrrpubi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hvgdcclq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pzutjofu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zasttgsp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vbjowqth.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkjxlmxk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2pefcgrgr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jifqbjqz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qoutcnze.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxhfmhj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2knxaelth.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vfjhaacl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnyjmbps.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2blssbdvd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ryhoapws.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ypdwykeo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgznhmdq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2irgwvcab.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2faiqzruo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sdhdswuh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2pybykpvx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ozayebfz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cegvgyvn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ukdkfodt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wtenzmdy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qkmjevez.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zwpydklr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mjbnnszv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2edywsort.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wiiauoki.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftrbszvi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fhdhplvf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hkvrneyl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2apfzvspa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2akxdfftz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2efmewoja.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tuldkxoy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wjpknena.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pzfcdwap.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pmmblcfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciozhilp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2hlfjqjsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjuikquq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2unaowxqb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2tuevcedw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ptmaebgt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xexwsaet.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bkklflde.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rupjvocc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qhdctcft.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wwwgdnmw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2aerjxvmx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uqrrcvtz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uwkxnemw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wktqgnny.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ajxrvxoq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ilrvetqf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2slsfzkiz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cawcdjvu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjyscfhj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zvkypcdq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qmgpajna.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2kialqjji.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hjsxaena.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2erqkojri.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lfkhpskp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2iaizuvzt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2frhdojtp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xqbvilke.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wqppczbb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vhrmepyd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ylobewbe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rqwdugkj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nmckznnl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wzmsbhlg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wkbsseji.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fsutxlcp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nbjwejuj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vwinnkzb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2cfqjbvtk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zcglfsxt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2brhzwmyb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kiquphmi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ebplafnf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ahcfvgde.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yoslpyum.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2guqdfoaa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ocxpkbrf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ltcpczil.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xefgjjpm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xisewpvf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2liztlvwe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xgaaqdlh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahqbcxpc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2sosgcjch.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2iincczcw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zsrrdttx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2dibmioyj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2hnjsppoq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2aranyjid.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gvlvjsze.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfzmdfsq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2nfbsdtku.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2dlstmpho.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ziiafpsw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2marfeytw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ooorglkx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qqmrvcih.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wctstqyc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2yxbbhyns.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vfblrqky.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jvsaihxh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2avdxkpcu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2eouktfbm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hvsgksfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlxxvojg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xjlpdwwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gumdogpc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2cqccyqpj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jdnljjrf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2azejdnpk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wglignji.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hkwgfmmb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ubveknvl.html

);
来源：http://www.52xcode.cn/Article/details/gt2bhwtjnua.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mnmhasmf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2tpkiloxn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ehtvepqc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fwforfyp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jymmeltt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kwfljalv.html

);
来源：http://www.52xcode.cn/Article/details/gt2csifrkfw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jzjgqpwf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bdcdwzpe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2czdhkfto.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2btbkfbor.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vkkbsoyo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wpojccad.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ikqvzzxk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ufescqgt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xsbbkqgz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gjfetdon.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2sdqyiofx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rmkobmgp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xgswyaeh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2adsgjrgr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2vbaktgzz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tbkltayg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ciaepyxi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zjnnnazp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nqpedjml.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2andiluqk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2babusegz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2dtneqlbt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hivwvleo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2orxdwdzl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pbgevkie.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ddovfgds.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2oglyyaff.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2djhaghcb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tpkfpyqo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opcvaeli.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tuhtohrf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nboyohvu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qdfxjyry.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ehyrkrvt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2tltjkxeq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ifxnxzds.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wjmtplql.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vlslzmvj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gzugvuqz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ozfoywtj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bsmzxage.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2limmomcg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fdevjxbc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wnqfloyk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zvyugotp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2verhythh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2iltobhbo.html


<!-- 参考信息 -->